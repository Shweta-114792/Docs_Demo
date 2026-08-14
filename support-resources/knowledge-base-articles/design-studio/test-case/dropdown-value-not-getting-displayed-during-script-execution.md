# Dropdown Value Not getting Displayed During Script Execution

**Summary**: This article addresses an issue where a dropdown value does not appear during script execution, even though it works correctly when performed manually. It also provides guidance on the appropriate action to use for such scenarios.

### Error behavior

When this issue occurs, you may observe the following behavior:

* The dropdown value is not displayed or selected during automation execution. &#x20;
* The same steps work correctly when executed manually. &#x20;
* No explicit error message may be shown, but the expected value is not reflected in the dropdown. &#x20;

### **Possible Reasons**

This issue may occur due to one or more of the following reasons:

* The Set Text action may not interact correctly with dropdown fields. &#x20;
* Dropdown controls often require keyboard-based input rather than direct text entry. &#x20;
* UI behaviour during automation can differ from manual interaction. &#x20;
* The control may depend on events (such as keypresses) that are not triggered by the Set Text action.&#x20;

### Resolution/Solution

To resolve this issue and ensure successful execution, perform the following actions:

1. Identify the step where the dropdown value is being entered. &#x20;
2. Check if the Set Text action is being used. &#x20;
3. Replace the Set Text action with the Send Keystroke action. &#x20;
4. Enter the required value using the Send Keystroke action. &#x20;
5. Execute the script again. &#x20;
6. Verify that the dropdown value is displayed correctly.&#x20;

