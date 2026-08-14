# Unable to Update Test Cases

**Summary**: Unable to edit the test step group within the test case and unable to save the changes.

### Error Behavior

When this issue occurs, you may observe the following behavior:

* Editing option for the test step group is not working.&#x20;
* Save action fails after attempting changes.&#x20;

### **Possible Reasons**

This issue may occur due to one or more of the following reasons:

* Session has expired.&#x20;
*   Test steps are part of a reusable library.&#x20;

    &#x20;

### Resolution/Solution

To resolve this issue and ensure successful execution, perform the following actions:

1. Ensure that the test step group is not linked to a reusable library.&#x20;
2. If it is linked, either detach it from the reusable library or update the test case directly within the reusable library.&#x20;
3. To make changes in the Reusable Library, the test case must be assigned to the respective user. If it is not assigned, the user should first assign it to themselves and make the required changes.&#x20;

{% hint style="info" %}
**Note:** Only users with the required privileges (for example, users with the Quality Manager role) can assign test cases to themselves or to other users.&#x20;
{% endhint %}

4. If the issue is caused by session expiry, please refresh the session or log in again.&#x20;
