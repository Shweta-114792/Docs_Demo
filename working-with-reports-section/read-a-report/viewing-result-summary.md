# Viewing Result Summary

The Test Report Summary provides a detailed view of test executions, including individual test case details and their execution status.

To view the Test Report Summary, perform the following actions:

1. On the **Home** page, under **Projects**, select the required **Project**.
2. Select **Design Studio** and select the **Reports** page.
3. Select the **Testcase Details** icon <img src="../../../.gitbook/assets/image (273).png" alt="" data-size="line">. The **Run Details** tab opens.

<figure><img src="../../../.gitbook/assets/image (290).png" alt="" width="375"><figcaption></figcaption></figure>

4. Select the **View Reports** icon <img src="../../../.gitbook/assets/image (303).png" alt="" data-size="line">. The **Result Summary** tab opens.

<figure><img src="../../../.gitbook/assets/image (309).png" alt=""><figcaption></figcaption></figure>

5. In the **Result Summary** window, you can view the following details:
   * **Test Case Name**: Displays the name of the Testcase being executed.
   * **Project Name**: Indicates the associated project name.
   * **Execution Mode:** Refers to how a Testcase was triggered or initiated.
   * **Start Date/End Date Time**: Specifies the start and end timestamps for the test execution.
   * **Execution Through:** Displays machine name or user details in reports to identify where and who executed the Testcase.
   * **Run Result**: Displays the overall execution result of the test case, such as **Pass**, **Fail**, or **Terminate**.
   * **Time Elapsed**: Displays the total time taken to complete the test execution.
   * **Executed Browser:** Shows the name of the browser on which the Testcase execution was triggered.
   * **Failure Reason**: Displays the reason for the execution failure.
   * **Overall Status:** Reflects the Testcase execution's final outcome.
   * **Progress Bar:** The progress bar visually depicts the percentage of passed, failed, terminated, in-progress, or queued steps.
6. **Expand** the first step arrow from the **#** column to view the detailed analysis of the execution, including all the test step details for the selected test case.

<figure><img src="../../../.gitbook/assets/image (310).png" alt=""><figcaption></figcaption></figure>

7. Explore the corresponding **Test Case** to view the following details:
   * **Run Result:** Displays the overall status of the Test Step Group and the execution result for each Test Steps in different colors.
     * **Green**: Indicates Test cases are passed.
     * **Red**: Indicates Test cases are failed.
     * **Grey**: Indicates Test cases are terminated.
     * **Yellow**: Indicates Test cases are executing (In Progress).
     * **Blue**: Indicates Test cases are in queue for execution.
     * **Orange**: Indicates Test cases are skipped.
   * **Time Elapsed:** Displays the duration taken to execute the test step.
   * **Step Details:** Displays the Test Step Group name along with detailed information about each step performed during execution.
   * **Error Details:** Displays the reason or error message for the failed test step.
   * **Remarks:** Displays additional information or comments related to the execution of the test step.
   * **Time Elapsed:** Displays the time taken for execution
   * **Found By:** Indicates the identifier through which it has been recovered
   * **Defect:** Indicates the option to log a defect in the defect management tool.

{% hint style="info" %}
**Note:** When a test case uses a captured element that is deleted, the execution stops automatically, and the Testcase is marked as Terminated in the Status column of the Reports section, and the Error Details column displays Deleted element found, instead of leaving the Testcase in In Progress.

**Example:**

If a test case contains a captured element like Submit Button and this element is deleted, execution stops immediately. The Status column shows Terminated, and the Error Details column displays element not found.

To learn how to add test step details, [click here](../../working-with-test-case-section/create-test-case/create-test-step-group/add-step-details.md).
{% endhint %}

8. Select the **Eye** icon <img src="../../../.gitbook/assets/image (315).png" alt="" data-size="line"> from the **Action** column to view the screenshot of the individual element captured from the Application Under Test (AUT).

<figure><img src="../../../.gitbook/assets/image (312).png" alt=""><figcaption></figcaption></figure>
