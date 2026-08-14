# Viewing Test Case Audit Logs

To view the test case audit logs, perform the following actions:

1. On the **Home** page, from **Projects** list, select required project.
2. Select **Design Studio**.
3. Select **Test Case**.
4. On the **Test Case** page, expand a folder and select the test case for which you want to see the details.
5. Select the **Information Panel** (**i**) icon. The **Details** tab opens.

![](<../../../../.gitbook/assets/unknown (295).png>)

6. Select the **Audit Logs** tab.

![](<../../../../.gitbook/assets/unknown (298).png>)

7. Select **Date Range** to view the actions performed between the specified dates.

![](<../../../../.gitbook/assets/unknown (299).png>)

8. Expand the month to view the actions performed in the test case.

![](<../../../../.gitbook/assets/unknown (300).png>)

### Audit Log Inclusions

The following actions are captured in the test case audit logs:

* Folder Level Actions
* Creating Test Case
* Renaming Test Case
* Adding or Updating Details
  * Description
  * Tags
* Creating Test Step Group (Non Avo Genius and Non-Reusable)
  * Adding Test Step Group (Test Case Name, Application type, Add from Repository or Add Manually)
  * Adding or Updating Step Details (Description, Expected Result, Pass Result or Fail Result)
* Creating Test Step Group (Reusable Library)
  * Adding Test Step Group from Reusable Library
  * Removing or Detaching Reusable Test Step Group
* Creating Test Step Group (Avo Genius)
  * Adding Test Step Group via Avo Genius Recording
* Performing Actions on Test Steps
  * Skipping Test Step
  * Copy Pasting Test Step
  * Deleting Test Step
  * Reordering Test Step Groups within Test Case
  * Reordering Test Steps
* Creating Recovery Steps
* Deleting Recovery Steps
* Importing Test Case
* Debugging Test Case
* Reviewing of Test Case (Including comments)
  * Assigning Test Case
  * Sending For Review
  * Approve
  * Reject
* Actions on Test Case in Bitbucket (Test Case, Reusable Library and End-to-End Flow)
  * Overwriting Test Case
  * Creating Test Case
  * Creating Folder
  * Pushing Test Case
  * Pulling Test Case

### Audit Log Exclusions

The following actions are currently not captured in the test case audit logs:

* Export
* Detailed Report-level Audit for Debug Executions
* Reused Test Step Groups
  * Delete
  * Test Step Group Description
  * Add Test Step
  * Add/Update Step Details (description, expected result, pass result, fail result)
  * Skip Test Steps
  * Copy/Paste Test Steps
  * Delete Test Steps
* E2E
  * Delete E2E
  * Deleted Test Cases
  * Added Test Cases
* Bitbucket
  * Compare
