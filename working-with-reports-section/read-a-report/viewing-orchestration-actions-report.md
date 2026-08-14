# Viewing Orchestration Actions Report

The following report options are available:&#x20;

* [**HTML Reports**](viewing-orchestration-actions-report.md#viewing-html-reports)&#x20;
* [**Reports in Avo Assure**](viewing-orchestration-actions-report.md#viewing-reports-in-avo-assure)&#x20;
* [**Local Directory Reports** ](viewing-orchestration-actions-report.md#viewing-local-directory-reports)

## Viewing HTML Reports

After the execution is completed, you can validate the results from the **Reports** page. &#x20;

To view the HTML reports, perform the following actions: &#x20;

1. On the **Home** page, under **Projects**, select the required **Project**.&#x20;
2. Select the **View reports** button. The **Reports** page opens.&#x20;
3. Locate **Execution list**, and select the **Execution list** from the required folder.&#x20;
4. In the right pane, select the **Testcase Details** icon. **Run Details** window appears.

<figure><img src="../../../.gitbook/assets/unknown (31).png" alt=""><figcaption></figcaption></figure>

5. Select the **View Reports** icon. The **Result Summary** window opens.

<figure><img src="../../../.gitbook/assets/unknown (32).png" alt=""><figcaption></figcaption></figure>

6. In **Result Summary** window, you can see the following details:&#x20;

* **TestCase Name**: Displays the name of the Test Case that is executed.&#x20;
* **Project Name**: Indicates the associated project name.&#x20;
* **StartDate/EndDate**: Specifies the start and end timestamps for the test execution.&#x20;
* **Overall Status**: Reflects the Testcase execution status.&#x20;
* **Progress Bar**: The progress bar visually depicts the percentage of passed, failed, terminated, in-progress, or queued steps.&#x20;
* **Execution Mode**: Refers to how a Testcase was triggered or initiated.&#x20;
* **Execution Through**: Displays machine name or user details in reports to identify where and who executed the Testcase.&#x20;
* **Executed Browser**: Shows the name of the browser on which the Testcase execution was triggered.&#x20;
* **Progress Bar**: Displays a visual summary of test result in percentage:
  * **Green**: Passed steps&#x20;
  * **Red**: Failed steps&#x20;
  * **Yellow/Gray**: Shows Other statuses like Terminated, In Progress, or Skipped.

7. Select **Expand** arrow from the **#** column to view the details of the execution.&#x20;

{% hint style="info" %}
**Note**: In the **Result Summary** window, you can view the following columns:&#x20;
{% endhint %}

* **Status**: Indicates the execution result for each step.&#x20;
* **Time Elapsed**: Displays the time taken for execution.&#x20;
* **Step Details**: Provides detailed information about the steps performed.&#x20;
* **Error Details**: Shows the failed test step reason.&#x20;
* **Remarks**: It displays the step details.&#x20;
* **Found By**: Indicates the identifier through which it has been recovered.&#x20;
* **Defect**: Indicates the option to log a defect in the defect management tool.&#x20;
* **Action**: Indicates the eye icon to view the screenshot.

<figure><img src="../../../.gitbook/assets/unknown (33).png" alt=""><figcaption></figcaption></figure>

## Viewing **Reports in Avo Assure**&#x20;

To download the reports in Avo Assure, perform the following actions:  &#x20;

1. On the **Home** page, under **Projects**, select the required **Project**.&#x20;
2. Select the **View reports** button. The **Reports** page opens.&#x20;
3. Locate **Execution list**, and select the **Execution list** from the required folder.&#x20;
4. In the right pane, select the **Download** icon to download the reports. &#x20;

{% hint style="info" %}
**Note**: After downloading the report in your local system, you can access and validate it.&#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/unknown (34).png" alt=""><figcaption></figcaption></figure>

## Viewing **Local Directory Reports**

After Orchestration Testcase execution, Avo Assure automatically retrieves the reports in your local directory. The generated report retains the original format, layout, and structure defined by the respective automation framework, without any modification by Avo Assure.&#x20;

The supported report formats for each integrated platform are as follows:&#x20;

* **Selenium**: Downloads an **HTML** report containing detailed step-level execution results, including actions, element interactions, and status.&#x20;
* **Safal**: Downloads an **Excel** report capturing validation details, input-output comparisons, and overall execution status.&#x20;
* **Karate/Cucumber**: Downloads an **HTML** report with scenario-wise execution details and test outcome summaries.&#x20;

Avo Assure references the report file path configured in the **Get Orchestration Reports** action to identify and access these framework reports. The reports remain in their original format and are not modified or reformatted by Avo Assure. This allows you or teams to access and review the same reports directly from the local system whenever required. You can view the downloaded report in the file location defined in the respective framework. &#x20;

Here is the sample screenshot of Safal platform: &#x20;

<figure><img src="../../../.gitbook/assets/unknown (35).png" alt=""><figcaption></figcaption></figure>
