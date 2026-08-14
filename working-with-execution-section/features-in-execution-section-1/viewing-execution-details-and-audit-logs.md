# Viewing Execution Details and Audit Logs

The execution details help you understand the key information related to an Execution list. You can view details such as the execution list name, description, status, creation date, time, and the user who created it.

The execution audit logs track the history of changes made to an execution folder or an execution list.

This document includes:

* [Viewing Execution Details](viewing-execution-details-and-audit-logs.md#viewing-execution-details)
* [Viewing Execution Audit Logs](viewing-execution-details-and-audit-logs.md#viewing-execution-audit-logs)

## Viewing Execution Details

To view the execution **Details**, perform the following actions:

1. On the **Home** page, from **Projects** list, select required project.
2. Select **Design Studio**.
3. Select **Execution**.
4. On the **Execution** page, expand the required folder and select the execution list for which you want to see the details.
5. Select the **Details** tab.

<figure><img src="../../../.gitbook/assets/unknown (273).png" alt=""><figcaption></figcaption></figure>

6. In the **Details** tab, you can view the following information:

* **Execution List Name**: The execution list name.
* **Description**: The execution list description.
* **Status**: The execution list status (New, In Progress, Under Review, Approved or Rejected).
* **Created On**: The execution list creation date and time.
* **Created By**: The username of the person who created the execution list.

<figure><img src="../../../.gitbook/assets/unknown (274).png" alt=""><figcaption></figcaption></figure>

## Viewing Execution Audit Logs

To view the execution **Audit Logs**, perform the following actions:

1. On the **Home** page, from **Projects** list, select required project.
2. Select **Design Studio**.
3. Select **Execution**.
4. On the **Execution** page, expand a folder and select the execution list for which you want to see the details.
5. Select the **Audit Logs** tab.

<figure><img src="../../../.gitbook/assets/unknown (275).png" alt=""><figcaption></figcaption></figure>

6. Select **Date Range** to view the actions performed between the specified dates.

<figure><img src="../../../.gitbook/assets/unknown (276).png" alt=""><figcaption></figcaption></figure>

7. Expand the month to view the actions performed in the execution list.

<figure><img src="../../../.gitbook/assets/unknown (277).png" alt=""><figcaption></figcaption></figure>

### Audit Log Inclusions

The following actions are captured in the execution audit logs:

* Creating Execution Folder
* Renaming Execution Folder
* Deleting Execution Folder
* Moving Execution Folder
* Setting Execution Trigger
  * Cancelling Execution Queue
  * Setting Scheduler
  * Executing via Cloud Test
* Executing Execution List
* Creating Execution List
* Renaming Execution List
* Configuring Execution List
  * Setting Execution List Profile Type
  * Setting On Failure
  * Selecting Execution Through Client/Agent
  * Selecting Client
  * Selecting Agent
  * Setting Browser
  * Selecting Execution Mode (Headless/Non-Headless)
  * Setting Integration
    * Selecting Test Management Tool
    * Updating and Selecting Relevant Tool Configuration Fields
    * Selecting Bug Tracking Tool (Jira)
    * Enabling/Disabling Auto defect Creation Toggle
    * Enabling/Disabling Genrocket Refresh Test Data Toggle
    * Updating the Records
* Enabling/Disabling Rerun Failed Test Case Toggle
* Updating Rerun Count
* Setting Email Notification
  * Enabling/Disabling Email Notification
  * Adding/Updating Recipients List
  * Enabling/Disabling Include PDF Reports Toggle
* Overriding ADV Excel Path (Including sheet name and ADV marker)
* Review (Including the comments)
  * Sent For Review
  * Approved
  * Rejected
* Adding Test Case to Execution List
* Setting On Failure per Test Case
* Changing Sequence of Test Case in Execution List
* Deleting Test Case

### Audit Log Exclusions

The following actions are currently not captured in the execution audit logs:

* Deleting Execution List
* Triggering DevOps
  * HTTP
  * Code Snippet
  * Cloud Execution
