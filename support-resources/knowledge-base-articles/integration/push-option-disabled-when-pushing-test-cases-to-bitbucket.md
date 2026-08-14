# Push Option Disabled when Pushing Test Cases to Bitbucket

**Summary**: The **Push** option is disabled when a user (Role: **QE**) attempts to push a test case to **Bitbucket**. This occurs when project-level restrictions are enabled in the **Manage Project** section, limiting the actions available for unassigned or unapproved artifacts.

### Error behavior

When this issue occurs, you may observe the following:

* The **Push** option in the user interface is grayed out or inactive.
* The user is unable to initiate the transfer of the test case to the **Bitbucket** repository.

### **Possible Reasons**

* This issue occurs due to the following project configuration:
  * The checkbox **Limit Bitbucket pushes to approved or user-assigned artifacts** is enabled under the **Manage Project** settings.
* When this setting is active, Avo Assure restricts the push capability to only those test cases that meet specific assignment or approval criteria.

### Resolution/Solution

To resolve this issue and enable the **Push** option, perform the following steps:

1. **Verify test case assignment:** Check if the selected test case is assigned to your user profile.
   * If the Test case is not assigned, contact your **Quality Manager** (**QM**) to have it assigned to you.
2. **Verify test case approval**: Check the approval status of the test case.
   * If the Test case has not been approved, contact the designated **Approver** to complete the approval process.

Once the Test case is both assigned to the user and approved, the **Push** option will become active.

### Additional Notes

* Always ensure that the project configuration allows for pushing artifacts to Bitbucket based on your organization's workflow.
* When the **Limit Bitbucket pushes to approved or user-assigned artifacts** check box is disabled under **Manage Project**, any test case can be pushed to **Bitbucket** regardless of its status.\
  Verify that the test case status and user permissions align with the project settings to avoid disabled options.
* If **Limit Bitbucket pushes** check box is checked, then Artifacts must be Approved AND Assigned.
* This structure ensures that the repository remains consistent by only allowing verified test cases to be pushed to Bitbucket.
