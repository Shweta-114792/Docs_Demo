# Managing File Path Setup for Runtime Data Operations

**Summary**: This article explains how to resolve the issue encountered while writing data to an Excel file during runtime execution, where the process fails due to a missing file path configuration.

### Error Behavior

When this issue occurs, you may observe the following behavior:

* The test step fails during execution when attempting to write data in Excel. &#x20;
* The error message displayed is: **File path not set None** \
  &#x20;

### **Possible Reasons**

This issue may occur due to one or more of the following reasons:

* The file path for the Excel file was not set before performing write operations. &#x20;
* The required step to initialize the file path is missing in the test case workflow.

### Resolution/Solution

To resolve this issue and ensure successful execution, perform the following actions:

1. Add a prerequisite step before Excel operations:\
   Ensure that the file path is defined before attempting to write data.
2. Configure the step correctly: &#x20;
   * Select Element Type as "Element" &#x20;
   * Choose the action "Set Path for File" &#x20;
   * Provide the correct Excel file path in the input value field
3.  Use the correct syntax for setting file path:&#x20;

    \<File Path>;\<SheetName (optional for Excel)>&#x20;

    Example:&#x20;

    C:\Users\vijayalaxmi.desai\Downloads\Fund Transfer.xlsx;Sheet1&#x20;

    * If a sheet name is provided, the system will operate on that specific sheet. &#x20;
4. Verify the sequence:\
   Make sure the "Set Path for File" step is executed prior to any Excel write actions in the test flow.

### Additional Notes

* This step is mandatory for Excel operations and must be added before write action. &#x20;
* For Data Table operations, this step is not required, as the data table does not depend on an external file path configuration.&#x20;
