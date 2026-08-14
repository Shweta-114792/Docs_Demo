# Textbox Value is Not Reflecting During Automation

**Summary**: During automation, a value is entered into a text box and appears visible on the screen. However, the application does not recognize or save the value, leading to failures in subsequent steps. This usually occurs because the application’s internal event listeners are not triggered during the input process.

### Error behavior

When this issue occurs, you may observe the following behavior:

* The text box displays the entered value, but internally it is not considered entered.
* The application does not proceed to the next step or trigger expected actions (such as enabling a **Submit** button).
* Subsequent steps that depend on this value fail during execution.

### **Possible Reasons**

This issue may occur due to one or more of the following reasons:

* The value appears in the text box, but the application's back-end or database does not register the input.
* The necessary triggers, such as JavaScript events (e.g., `onchange` or `oninput`), are not activated.
* The application does not treat the value as valid input because it was not entered through a standard keyboard interaction.

### Resolution/Solution

To resolve this issue, perform the following actions:

1. **Use the Set Text action**: First, attempt to enter the value into the text box using the **Set Text** action.
2. **Use the Send Keystroke Value action**: If the value is still not properly recognized or saved, use the **Send Keystroke Value** action instead of **Set Text**.

Using **Send Keystroke Value** ensures that the application recognizes the input as a series of keyboard events.

### Additional Notes

* Always ensure that the application correctly recognizes the input to prevent failures in subsequent steps.
* When the **Set Text** action does not trigger the necessary application events, then use the **Send Keystroke Value** action.
* Verify that the value is correctly saved by checking if subsequent steps or "Next" buttons become active.
* [**Set Text**](../../../../actions/web/textbox/set-text.md): Used to copy-paste the value into the field.
* [**Send Keystroke Values**](../../../../actions/web/textbox/send-keystrokes-values.md): This action sends the value one character at a time, similar to typing from a physical keyboard.
