# Migrating Java Selenium Scripts to Avo Assure

This section explains how to migrate Selenium automation scripts written in Java into Avo Assure Test cases.

## Prerequisites

Before you migrate Selenium scripts to Avo Test cases, make sure the following requirements are fulfilled:  &#x20;

* **Selenium Environment**: You must have a configured Selenium development environment (such as Eclipse) to execute the scripts.&#x20;
* **Interceptor Setup**: You must set up the interceptors in your project.&#x20;
* **Script Status**: Your Selenium automation scripts are up to date.&#x20;
* **Error-free Execution**: Ensure the Selenium script runs successfully without any errors before using it in Avo Assure.&#x20;
* **Avo Assure Access**: You must have access to the Avo Assure server.&#x20;

## Known Limitations

* **Maximum Supported ZIP File Size**: The maximum supported size for a ZIP file is 50 MB.
* **Duplicate Variables in Excel File**: If the Excel file contains duplicate variables (the same column name defined more than once), the migration process may fail or produce inconsistent parameter mapping results.
* **Logical Conditions Support**: Currently, the migration feature supports selenium script or Test case, logical conditions such as IF statements and loops are not supported.

## Best Practices

* **Data Parameterization** (**Excel file**):
  * Make sure each variable name (column name) in the Excel file is unique.
  * Do not define the same variable name more than once in the data sheet.
  * Validate the Excel data before executing the Selenium scripts.

## Migrating Selenium Scripts

To migrate your Java scripts, you must first set up the interceptor in your project, generate the scenario file, and then import it into Avo Assure.&#x20;

The interceptor allows you to execute code before and after your automation logic without modifying the core functionality of the scripts.&#x20;

{% hint style="info" %}
**Note**: &#x20;

* During migration, Avo Assure considers only Selenium actions performed on the browser. &#x20;
* Avo Assure maps Selenium test data automatically. You should review the migrated data to ensure it is correct. &#x20;
* During migration, Avo Assure normalizes all Selenium select actions. The following actions are migrated as selectByValue in Avo Assure:&#x20;
  * selectByValue &#x20;
  * selectByIndex &#x20;
  * selectByVisibleText &#x20;
{% endhint %}

### Downloading and Configuring Interceptor

To download and configure the Interceptor for Selenium scripts in Avo Assure, perform the following actions:

1. On the **Home** page, go to **Utilities** and select the **Migrate To Avo** tab.&#x20;

<figure><img src="../../../.gitbook/assets/image (4888).png" alt=""><figcaption></figcaption></figure>

2. On the **Selenium to Avo** page, select **Java** as the programming language from the **Select Technology** dropdown.
3. Select **Download** to save the interceptor package file (java-intercept.zip) to your local machine.&#x20;

<figure><img src="../../../.gitbook/assets/image (4889).png" alt=""><figcaption></figcaption></figure>

4. Extract the downloaded **java-intercept.zip** file.
5. Copy the extracted interceptor folder into your Selenium project’s Java source directory (the directory that contains your Selenium framework classes). For Example, \<Path to your Selenium project>/src/main/java OR \<Path to your Selenium project>/src/test/java.

{% hint style="info" %}
**Note**: The interceptor folder must be placed inside a Java source root to ensure it is included during project compilation.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4890).png" alt=""><figcaption></figcaption></figure>

6. Configure the Interceptor:  \
   Configuring the Interceptor allows Avo Assure to capture Selenium browser actions and data parameterization during execution, ensuring accurate migration. \
   \
   To configure the interceptor, perform the following actions:&#x20;

{% hint style="info" %}
**Note**: This configuration is a one-time setup.
{% endhint %}

<details>

<summary><strong>Enabling WebDriver Interception</strong></summary>

In the **BrowserFactory.java** file where the WebDriver is initialized (for example, in a factory class, base class, or any custom setup file), update the driver configuration to use **InterceptWebDriver.**

&#x20;1\. Add the following import statement to the file:

```java
import intercept.InterceptWebDriver;
```

2. Locate the line where the browser driver is created (for example, new ChromeDriver() or new FirefoxDriver()) and replace it with **InterceptWebDriver**.
   1. If your code creates the driver with options:

```java
//Before
WebDriver driver = new ChromeDriver(options);
//After
WebDriver driver = new InterceptWebDriver(new ChromeDriver(options));
```

&#x20;         b. If your code creates the driver without options:

```java
//Before
WebDriver driver = new ChromeDriver();
//After
WebDriver driver = new InterceptWebDriver(new ChromeDriver());
```

{% hint style="info" %}
**Note**: Ensure that every **WebDriver** created in your project uses **InterceptWebDriver**. This applies to all browsers, file names, and initialization methods.
{% endhint %}

{% hint style="info" %}
**How It Works?**

**InterceptWebDriver** works along with your existing Selenium driver and captures the actions performed in the browser during execution. It does not change your test scripts. It only records the actions so they can be migrated to Avo Assure.
{% endhint %}

</details>

<details>

<summary><strong>Updating testRunner Configuration</strong></summary>

1. On the Editor, open **testRunner.java**.
2. Add `"intercept"` to the **glue** parameter.
3. Update the **glue** variable as shown below:

```java
glue = { "steps", "intercept" }
```

{% hint style="info" %}
**How it works?**

* Adding **"intercept"** to the glue parameter in **testRunner.java file** instructs the framework where to look for step definitions related to WebDriver interception.
* By updating **glue = { "steps", "intercept" }**, the framework can correctly link your test steps with the interception logic, ensuring smooth execution of tests with the new WebDriver setup.
{% endhint %}

</details>

<details>

<summary><strong>Enabling Data Parameterization</strong></summary>

1. Add the following code snippet to the **setTestData** function in your common Excel data reader file (such as CommonStepsForTestDataReader.java):&#x20;

```java
import intercept.AvoHooks;
AvoHooks.setExcelData(tableValue);
```

{% hint style="info" %}
**How it works?**

* **tableValue** is the variable that stores the test data from your Excel sheet. It can have multiple rows and columns, depending on your test.
* **AvoHooks.setExcelData(tableValue)** lets the automation framework use this data during the test, so your tests can run with different inputs automatically.
{% endhint %}

</details>

### Generating and Uploading Scenarios

To generate and upload Selenium scripts to Avo Assure, perform the following actions:

1. Execute your Selenium automation suite.

{% hint style="info" %}
**Note**:&#x20;

* The execution generates a **selenium\_testcase\_batch.zip** file at the following location: \
  \<Project Path>/target/avo\_intercept\_output.
* The ZIP file name must follow the format **selenium\_testcase\_batch.zip**. File names such as selenium\_testcase\_batch1.zip or selenium\_testcase\_batch2.zip are supported. Randomly named ZIP files are not allowed and will fail validation.
{% endhint %}

2. Go to **Selenium To Avo** page in Avo Assure.&#x20;
3. In the **Select Project** dropdown, select the Avo Assure project where you want to import the Selenium test cases.&#x20;

<figure><img src="../../../.gitbook/assets/image (4891).png" alt=""><figcaption></figcaption></figure>

4. Upload the **selenium\_testcase\_batch.zip** file generated in step 1.&#x20;

{% hint style="info" %}
**Note**: The uploaded ZIP file must contain only JSON files. Other file types are not supported.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4892).png" alt=""><figcaption></figcaption></figure>

5. After uploading the file, select **Start Migration**. The **Migration Status** dialog opens.&#x20;

<figure><img src="../../../.gitbook/assets/image (4893).png" alt=""><figcaption></figcaption></figure>

6. On the **Migration Status** dialog, the following details are displayed:

* **Element Repository Folder** and **Test case Folder** name.&#x20;
* **Test case Name** and migration **Status**.
  * **Status**: Shows whether a Test case is **SUCCESS**, **FAILED**, or **SKIPPED**. An **Info** (**i**) icon displays the reason for each status.
    * **Fail**: Migration fails due to an error, such as missing data or missing key in the Test case JSON file.
    * **Success**: The Test case migrated successfully.&#x20;
    * **Skipped**: Migration is skipped because the Test case fails during Selenium execution.&#x20;
* The system provides a downloadable Excel file that contains data parameterization details. Use this Excel file as a reference to review and correct the migrated Test cases in Avo Assure, if required.\
  The Excel file includes the following information:
  * Test case name.&#x20;
  * Test Step Group name.&#x20;
  * Step details, including whether data parameterization is present.&#x20;

{% hint style="info" %}
**Note**: To download the Excel file, the **Download** link is available only when Data Parameterization is configured in your Selenium code.
{% endhint %}

7. Select **Ok** to close the **Migration Status** dialog.

<figure><img src="../../../.gitbook/assets/unknown (240).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
&#x20;**Note**: After the migration is complete, verify the following:&#x20;

* Review the migrated Test cases for accuracy.&#x20;
* Verify that the test data is mapped correctly.&#x20;
* Manually validate business-critical test scenarios.&#x20;
* Data is parameterized only when you enable Data Parameterization. Otherwise, Avo Assure uses hardcoded values. &#x20;
{% endhint %}
