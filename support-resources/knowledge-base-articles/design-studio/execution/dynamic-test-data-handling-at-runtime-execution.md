# Dynamic Test Data Handling at Runtime Execution

**Summary**: This document explains the process of handling data during runtime from different test cases across various folders using variables&#x20;

### Error behavior

When this issue occurs, you may observe the following behavior:

* The data from the variable is not passed to different test cases at runtime.

### **Possible Reasons**

This issue may occur due to one or more of the following reasons:

* The correct variable names are not provided to dependent test cases&#x20;
* The variable declaration format is incorrect&#x20;
* The E2E flow is not created before adding test cases from different folders to the execution list&#x20;

### Resolution/Solution

To resolve the issue, perform the following action:  &#x20;

1. ​​Check the variable names and formats passed across different test cases. &#x20;
2. Create the E2E flow and include all test cases from different folders.&#x20;

