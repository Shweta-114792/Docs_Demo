# Re-running the Failed Test Cases

To Re-run the failed Test Cases in Avo Assure we have two ways

* [**Reports Tab**](re-run-the-failed-test-cases.md#re-run-failed-test-case-from-reports-tab)
* [**Execution Tab**](re-run-the-failed-test-cases.md#re-run-failed-test-case-from-execution-tab)

### **Re-Running Failed Test Case from Reports Tab**

1. Navigate to **Reports tab** and click on **Re-Run Test Case** option beside the Test Case Summary column, the failed test case pop-up will appear

<figure><img src="../../../../.gitbook/assets/image (3999).png" alt=""><figcaption></figcaption></figure>

2. Select **Failed Test Case** from the table which needs to execute again and Click on **Re-Run** button

<figure><img src="../../../../.gitbook/assets/image (4000).png" alt=""><figcaption></figcaption></figure>

3. The Execution Now pop-up appears. Select the desired options and enable the **Re-Run Failed Test Case** toggle button located below, and set the **Re-run Count** (any value between 1 to 5)

<figure><img src="../../../../.gitbook/assets/image (4001).png" alt=""><figcaption></figcaption></figure>

4. Click on **Execute** button

<figure><img src="../../../../.gitbook/assets/image (4002).png" alt=""><figcaption></figcaption></figure>

### **Re-running Failed Test Case from Execution Tab**

Navigate to Execution on Client page then click below link\
[Execution on Client](../../../working-with-execution-section/execute-execution-list/execution-through-client-agent-grid.md)

### Example

**Let’s say a test execution gave the following results:**

| **Test Case**          | **Result** |
| ---------------------- | ---------- |
| TC\_01 (Fund Transfer) | Failed     |
| TC\_02 (Loans)         | Passed     |

The **Re-run Failed Test Cases** option is enabled, and the rerun count is set to 3.

* Only **TC\_01 (Fund Transfer)** will be rerun because **TC\_02 (Loans)** already passed.
* If **TC\_01 (Fund Transfer)** continues to fail, it will be retried up to 3 times.
* The final report will show the latest result of **TC\_01 (Fund Transfer)** after the reruns.
