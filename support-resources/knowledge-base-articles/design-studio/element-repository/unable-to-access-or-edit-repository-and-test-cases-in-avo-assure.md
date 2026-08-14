# Unable to Access or Edit Repository and Test Cases in Avo Assure

**Summary**: You are unable to access or edit the test case repository and test cases in Avo Assure. The issue was resolved after the required repositories, and test cases were assigned to the user.&#x20;

### Error behavior

When this issue occurs, you may observe the following behavior:

* You are unable to access or edit test cases.
* Element repository access was restricted and editing options were unavailable even though the user was successfully logged into the system.

### **Possible Reasons**

This issue may occur due to one or more of the following reasons:

* The test case repository was not assigned to the user. &#x20;
* The element repository permissions were missing for the user.  &#x20;
* User account did not have sufficient privileges for repository operations.

### Resolution/Solution

To resolve this issue and ensure successful execution, perform the following actions:

1. Verify user access permissions for both test case and element repositories. &#x20;
2. Assign the required repository and test cases to the user profile. &#x20;
3. Ensure proper role-based access is configured for editing rights.&#x20;
4. Ask the user to log out and log in again to refresh permissions. &#x20;
5. Confirm that the user can now access and edit the assigned test cases successfully.

### Additional Notes

*   User Roles and Permissions in Avo Assure&#x20;

    * **Quality Manager**: Can create and manage projects. &#x20;
    * **Quality Lead**: Can create test suites, execution configurations, and perform impact analysis. &#x20;
    * **Quality Engineer**: Can create and execute test steps and generate/view reports. &#x20;
    * **Admin**: Can access the admin section to configure and set up Avo Assure.&#x20;

    &#x20;
