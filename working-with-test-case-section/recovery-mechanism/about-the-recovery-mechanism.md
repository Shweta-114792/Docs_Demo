# About the Recovery Mechanism

This section explains the **Recovery Mechanism** in Avo Assure. It allows you to define recovery steps at multiple levels within the test hierarchy. These levels control the scope on which recovery steps are executed when a failure occurs. This flexibility helps to handle both common failures and test specific issues effectively.

Recovery steps can be defined at three levels for **Test Case** page in Avo Assure:

<table data-header-hidden><thead><tr><th width="137"></th><th width="206.86669921875"></th><th></th></tr></thead><tbody><tr><td><strong>Priority</strong> </td><td><strong>Level</strong> </td><td><strong>Description</strong> </td></tr><tr><td>1 </td><td>Test case Level </td><td>Executes recovery only for the particular Test case.</td></tr><tr><td>2 </td><td>Sub Folder Level </td><td>Executes recovery for the particular sub folder.</td></tr><tr><td>3 </td><td>Folder Level </td><td>Execute recovery for the entire folder.</td></tr></tbody></table>

1. Test case level
   * Test case level recovery applies only to the chosen Test case when the Test case fails. Avo Assure executes only the recovery steps defined for that Test case and ignores recovery steps created at higher levels.&#x20;
   * Where to Use: Use Test case level recovery for scenarios that require unique or custom recovery steps. This level applies when a Test case has independent dependencies, maintains its own data or execution state, or generates temporary files or artifacts that require cleanup specific to that Test case.
2. Sub Folder Level
   * Sub Folder Level recovery applies only to the Test cases within a specific sub folder. When a Test case in the sub folder fails, Avo Assure executes the recovery steps created at sub folder level and does not execute the folder level recovery steps.&#x20;
   * Where to Use: Use sub folder level recovery to handle failures related to a specific group of Test cases (sub folder). This level allows you to apply targeted recovery steps to Test cases within the sub folder and ensures that Test cases in other sub-folders remain unaffected.
3. Folder Level
   * Folder level recovery applies to all Test cases inside a folder, including Test cases in all its sub folders. When any Test case under the folder fails, Avo Assure executes the recovery steps defined at the folder level recovery.
   * Where to Use: Use folder level recovery to handle failures that affect the overall Test case. This level suits situations where multiple Test cases depend on common setup, or other scenarios.

<figure><img src="../../../../.gitbook/assets/unknown (202).png" alt=""><figcaption></figcaption></figure>

## Recovery Mechanism Execution Flow with Priority

This section explains how the **Recovery Mechanism** execution flow works and how priority determines which recovery steps run first when a Test case fails.

<table data-header-hidden><thead><tr><th width="96.3333740234375"></th><th width="130.5999755859375"></th><th width="212"></th><th></th></tr></thead><tbody><tr><td><strong>Step</strong> </td><td><strong>Priority</strong> </td><td><strong>Action Performed</strong> </td><td><strong>Description</strong> </td></tr><tr><td>1 </td><td>— </td><td>Test case fails </td><td>The system detects failure during automated test execution. </td></tr><tr><td>2 </td><td>High </td><td>Check Test case level recovery </td><td>The system checks whether recovery steps are created for the failed Test case. </td></tr><tr><td>3 </td><td>High </td><td>Execute Test case level recovery (if available) </td><td>The system executes the recovery steps defined at the Test case level and skips lower priority levels. </td></tr><tr><td>4 </td><td>Medium </td><td>Check sub folder level recovery </td><td>If no Test case level recovery exists, the system checks recovery steps created at the sub folder level. </td></tr><tr><td>5 </td><td>Medium </td><td>Execute sub folder level recovery (if available) </td><td>The system executes the recovery steps defined at the sub folder level and skips the folder level. </td></tr><tr><td>6 </td><td>Low </td><td>Check folder level recovery </td><td>If no sub folder level recovery exists, the system checks recovery steps created at the folder level. </td></tr><tr><td>7 </td><td>Low </td><td>Execute folder level recovery (if available) </td><td>The system executes the recovery steps defined at the folder level. </td></tr><tr><td>8 </td><td>— </td><td>Continue execution </td><td>The system resumes execution after completing the applicable recovery steps. </td></tr></tbody></table>

