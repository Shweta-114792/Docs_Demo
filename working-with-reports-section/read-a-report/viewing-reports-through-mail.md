# Viewing Reports through Mail

After you complete the execution, the generated **Test Execution Report** is automatically sent to the specified recipient via email.

{% hint style="info" %}
**Note**:

* If the execution PDF reports exceed 20 MB, Avo Assure converts them into a zip file and sends them via email. If the zip file size is still more than 20 MB after conversion, an error message **The report is too large to send as an attachment. Please download it from Avo Assure application** is displayed.
* To learn how to set the recipient email ID for sharing the report. To learn more, [click here](../../working-with-execution-section/features-in-execution-section/mode-and-notification.md).
{% endhint %}

### Viewing Reports in Detail

The Email consists of following reports:

1. [**Summary Report**](viewing-reports-through-mail.md#id-1.-summary-report): Displays an overview of the test execution including the total number of test cases executed, passed, failed, or terminated, overall execution status, and time taken for executing a test case. It includes an HTML version of the report.
2. [**Detailed Report**](viewing-reports-through-mail.md#id-2.-detailed-report)**:** Provides step-level execution details within each test step group, including status, duration, error messages, remarks, and screenshots. The report also includes overview details to give a complete view of the execution results.

#### 1. Summary Report

The Summary Report provides an overview of the test case execution results. It displays high-level information about the project, execution details, and overall test case status to help users quickly assess the outcome of the execution.

In Summary Reports you can view the following details:

* **Project Name**: Displays the name of the project under which the test case execution was performed.
* **Execution Profile Name**: Displays the execution profile associated with the test case.
* **Start Date and Time (UTC)**: Displays the exact date and time the test execution started, in UTC format.
* **Type of Execution**: Displays the type of execution performed. For example, Avo Client.
* **Total Test Cases Executed**: Displays the total number of test cases executed during the run.
* **Total Test Cases Passed**: Displays the number of test cases that successfully passed.
* **Total Test Cases Failed**: Displays the number of test cases that failed during execution.
* **Total Test Cases Terminated**: Displays the number of test cases that were stopped or terminated before completion.
* **Test Case Name**: Displays the name of the executed test case.
* **Execution Status**: Displays the final execution result of the test case. For example, Pass or Fail.
* **Time Elapsed**: Displays the total time taken to complete the execution of the test case.
* **Reports**: Displays the generated test execution reports in HTML format.

<figure><img src="../../../.gitbook/assets/image (4428).png" alt=""><figcaption></figcaption></figure>

### 2. Detailed Report

The Detailed Report provides in-depth information about each step executed within the test case. It includes data such as action performed, execution time, recovery mechanism, and error details, allowing users to analyze the execution flow and identify issues.

To view the Detailed Report from the email, perform the following actions:

1. Open the **Email** received after the test execution is completed.
2. Select the **PDF report** to view the detailed execution report.

<figure><img src="../../../.gitbook/assets/image (4429).png" alt=""><figcaption></figcaption></figure>

3. After selecting the PDF report, the detailed execution report is displayed in a new tab.

<figure><img src="../../../.gitbook/assets/image (4431).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (4527).png" alt=""><figcaption></figcaption></figure>
