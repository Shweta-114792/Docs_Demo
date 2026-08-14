# Textbox Value Not Getting Entered Properly During Automation

**Summary**: During automation, a value is entered into a textbox and appears visible on the screen. However, the application does not recognize or save the value, leading to failures in subsequent steps

### Error behavior

When this issue occurs, you may observe the following behavior:

* The textbox displays the entered value, but internally it is not considered as entered. As a result, the application does not proceed to the next step or trigger expected actions.

### **Possible Reasons**

This issue may occur due to one or more of the following reasons:

* The value appears in the textbox, but it is not actually entered into the system.
* The necessary actions, such as typing or pressing keys, are not triggered.  &#x20;Because of this, the application does not treat the value as valid input since it was not entered in a normal way.

### Resolution/Solution

To resolve this issue and ensure successful execution, perform the following actions:

1. First, use the Set Text action to enter the value into the textbox.&#x20;
2. If the value is still not properly entered or saved:&#x20;
   * Use Send Keystroke value.&#x20;
   * Enter the same value as if typing manually.&#x20;

This method ensures that the application correctly recognizes the input and that the value is properly entered and saved.&#x20;

### Additional Notes

* **Set Text**: used to copy-paste the value&#x20;
* **Send Keystroke value**: this sends the value one character at a time, similar to typing from a keyboard&#x20;
