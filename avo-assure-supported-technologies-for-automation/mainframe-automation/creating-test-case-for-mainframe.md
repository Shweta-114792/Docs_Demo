# Creating Test Case for Mainframe

To create test case for mainframe, perform the following actions:

1. On the **Home** page, from **Projects** list, select required project.&#x20;
2. Select **Design Studio**.&#x20;
3. Select **Test Case**.&#x20;
4. On the **Test Case** page, select folder and then select ellipses (**...**) icon.&#x20;
5. Select **Create Test Case** and rename it.&#x20;
6. Select **Create Test Step Group** and **Add new test step group**.&#x20;
7. On the **Test Step Group** dialog, in the **Test Step Group Name** text box, add test step group name.&#x20;
8. From **Application type** dropdown, select **Mainframe**.&#x20;
9. Select **Create**.&#x20;
10. Select **+** icon and select **Add step manually**.&#x20;
11. A new test step is created. Select the **Mainframe List** as an **Element**, and then action from the **Action** dropdown.&#x20;
    1. Select **Mainframe List** from the **Element** dropdown.&#x20;
    2. From the **Action** dropdown, select **Launch mainframe**.&#x20;
    3. In the **Input Value** text box, enter the emulator path and emulator type.&#x20;
    4. Add another test step and select element from the **Element** dropdown.&#x20;
    5. From the **Action** dropdown, select **Set Text**.&#x20;
    6. In the **Input Value** text box, enter the username.&#x20;
    7. Select **Mainframe List** from the **Element** dropdown.&#x20;
    8. From the **Action** dropdown, select **Set Function Key**.&#x20;
    9. In the **Input Value** text box, enter the **Enter** text.&#x20;
    10. Add another test step and select element from the Element dropdown.&#x20;
    11. From the **Action** dropdown, select **Set Text**.&#x20;
    12. In the **Input Value** text box, enter the password.&#x20;
    13. Select **Mainframe List** from the **Element** dropdown.&#x20;
    14. From the **Action** dropdown, select **Set Function Key**.&#x20;
    15. In the **Input Value** text box, enter the **Enter** text.&#x20;

![](<../../.gitbook/assets/unknown (305).png>)

12. Select **Save** to save the Test Step group.

{% hint style="info" %}
Note: To know more about Mainframe actions, refer the [Mainframe Actions](../../actions/mainframe/)
{% endhint %}
