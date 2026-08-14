# Creating APIs Test Case

## Creating Test Step Group

To add a Test Step Group in a Test case, perform the following actions:

1. On the **Home** page, select the required project and select **Design Studio**.
2. Go to the **Test Case** tab and select the created Test case.

{% hint style="info" %}
**Note**: To learn more about how to create a new Test Case Folder and Test Case, [click here](../../create-and-execute-tests-with-design-studio/working-with-test-case-section/create-test-case/).
{% endhint %}

3. Select **Create Test Step Group** and select **Add new test step group**. The **Test Step Group** dialog opens.
4. Enter the name in the **Test Step Group Name** text box.
5. Select **APIs** as an **Application Type**.
6. Select **Create** to add a new Test Step Group. This creates a new **API Test Step Group** inside the Test case.

{% hint style="info" %}
**Note**: You can also add a **Test Step Group** from the [**Reusable Library**](../../create-and-execute-tests-with-design-studio/working-with-test-case-section/create-test-case/create-test-step-group/add-test-steps-group-from-reusable-library.md).
{% endhint %}

## Creating Test Steps

To create APIs test steps, use one of the following methods:

* **Add from Repository**
* **Add Manually**

<details>

<summary><strong>Adding from Element Repository</strong></summary>

Add from Repository is used to add key–value pair steps required for an API request. The Element Repository stores API elements such as JSON keys, XML keys, form-data fields, and URL-encoded parameters. You can select these elements from the repository and add them directly to the test steps.

To add APIs from the Element Repository to the Test Step Group, perform the following actions:

1. On the **Test Case** tab, select the created Test case.
2. Select **Create Test Step Group** and select **Add new test step group**.
3. Select **Add from Repository**. The **Element Repository** page opens.

<figure><img src="../../.gitbook/assets/image (5043).png" alt=""><figcaption></figcaption></figure>

4. Drag-and-drop the **APIs** from repository into the **Test Step Group**.

{% hint style="info" %}
**Note**:

* When you drag and drop elements from the **Element Repository** in a **APIs Test Step Group**, all **JSON** and **XML** keys, including parent and nested keys are available in the **Element Name** dropdown. The **Element Name**, **Action** (Keyword), and **Input Value** automatically populate in the test steps.
* When you drag and drop elements for **form-data** or **URL-encoded** from the **Element Repository**, their **key names** are available in the **Element Name** dropdown, and the **Action** is automatically set to **Set Tag Value**.
{% endhint %}

3. (Optional) Add the required validation steps using appropriate action (for example, Get Header or Get Body) to verify the API response.
4. Select **Save** to save the test steps.
5. Select **Debug** to run the test step group.

{% hint style="info" %}
**Note**: To generate reports for the Test Steps, you can create an [**Execution List**](../../create-and-execute-tests-with-design-studio/working-with-execution-section/execute-execution-list/).
{% endhint %}

</details>

<details>

<summary><strong>Adding APIs Manually</strong></summary>

The **Add Manually** is used to create and add the required test steps for an API request directly within the test case. This option allows you to manually define the request details, such as JSON keys, XML keys, form-data fields, or URL-encoded parameters, without using the Element Repository.

To add APIs manually to the Test Step Group, perform the following actions:

1. On the **Test Case** tab, select the create Test Case.
2. Select **Create Test Step Group**.
3. Select **Add Manually** to add a new Test Step.

<figure><img src="../../.gitbook/assets/unknown (260).png" alt=""><figcaption></figcaption></figure>

4. Select the **Add Step** (**+**) icon and choose **Add Step Manually** to add more steps to the Test Step Group.

{% hint style="info" %}
**Note**: You can add test steps using the **Add Step (+)** icon in two ways:

* From the top corner of the Test Step Group to add a new step.
* By hovering over an individual step, where the **Add Step** (**+**) icon appears next to the **Output Value** column to insert additional steps within the group.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (5044).png" alt=""><figcaption></figcaption></figure>

5. A new test step is created. Select the **APIs List** as an **Element Type,** and then action from the **Action** dropdown.\
   \
   The following example demonstrates how to configure a APIs request by setting the endpoint URL, request method, required headers, and executing the request using APIs List actions.\
   \
   To create the test steps required to configure the API request, perform the following steps:
   1. Select **APIs List** from the **Element Type** dropdown.
   2. From the **Action** dropdown, select **Set End Point URL**.
   3. In the **Input Value** text box, enter the required API endpoint URL.
   4. Add another test step and select **APIs List** from the **Element Type** dropdown.
   5. From the **Action** dropdown, select **Set Method**.
   6. In the **Input Value** text box, enter **GET** to specify the request method.
   7. Add another test step and select **APIs List** from the **Element Type** dropdown.
   8. From the **Action** dropdown, select **Set Header** (if the API requires headers).
   9. Provide the required header details in the **Input Value** text box (for example, Authorization or Content-Type).
   10. Add another test step and select **APIs List** from the **Element Type** dropdown.
   11. From the **Action** dropdown, select **Execute Request**.

{% hint style="info" %}
**Note**: This action sends the configured API request to the server and returns the response based on the provided endpoint, method, headers, and other details.
{% endhint %}

6. (Optional) Add the required validation steps using appropriate action (for example, Get Header or Get Body) to verify the API response.
7. Select **Save** to save the test steps.

{% hint style="info" %}
**Note**:

* After creating the test steps, you can debug the Test Step Group to verify the execution.
* To generate reports for the test steps, you can create an [**Execution List**](../../create-and-execute-tests-with-design-studio/working-with-execution-section/execute-execution-list/).
{% endhint %}

</details>

## Add Element

The Add Element feature is available only for APIs test step groups and is used for form-data and urlencoded requests. It helps you manually add keys inside the test case, where each key is considered as an element. This is useful when you create manual scripts, so you can directly define and use key–value pairs without depending on the Element Repository.

{% hint style="info" %}
**Note**: This feature only works for **form-data** and **urlencoded**.
{% endhint %}

To use **Add Element** in Test Case, perform the following actions:

1. On the **Test Case** tab, go to the **Test Step Group.**
2. In the **Elements** column, select the **+ Add Element**. The **Add element** dialog opens.
3. Enter the **Element name** (Key name) in the text box.
4. Select the **Input Type** (**Text** or **File**) from the dropdown.

{% hint style="info" %}
**Note**:

* **If you selected File**: In the **Input Value** text box, you can provide the file path directly or choose the file from a Segregated Avo Storage location.
* **If you selected Text**: In the **Input Value** text box, you can provide the text.

To learn how to add Text or File as an Input Type, [click here](element-repository-interface-and-functional-flow/about-the-request-tab.md).
{% endhint %}

5. Select **Add** to create the element.

<figure><img src="../../.gitbook/assets/image (5045).png" alt="" width="375"><figcaption></figcaption></figure>

6. Enter the tag value in the **Input Value** column.

{% hint style="info" %}
**Note**:

* After you add the element, the system automatically selects the **Action** (**Set Tag Value**), and it is not editable.
* You can update the parameter name and its value by selecting the **Edit** icon.
{% endhint %}

<figure><img src="../../.gitbook/assets/image (5046).png" alt=""><figcaption></figcaption></figure>

7. Select **Save** to save the created test steps.

#### Key Points to Know

* You can directly create a Test Case and perform API testing without executing any API request from the **Element Repository** page.
* To automate APIs in Avo Assure, there is no need to capture application elements as APIs work in the backend.
* To automate APIs successfully, it is important to understand the correct actions applicable to your application. For a detailed list of supported **APIs List** actions, [click here](../../actions/apis/).

**Other Related Links**:

* To learn more about how to create and execute an execution list, [click here](../../create-and-execute-tests-with-design-studio/working-with-execution-section/).
* To learn more about how to view the API Test Case execution Reports, [click here](../../create-and-execute-tests-with-design-studio/working-with-reports-section/).
