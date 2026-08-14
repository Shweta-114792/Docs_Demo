# Create Dynamic Variable Action Failing

**Summary**: The **Create Dynamic Variable** action fails if an attempt is made to create a variable name that is already defined in the current execution scope. When this error occurs, the test execution stops, and subsequent steps fail to execute.

### Error behavior

When this issue occurs, you may observe the following behavior:

* The test execution stops at the **Create Dynamic Variable** step.
* The following error message appears on the **Avo Assure Client**: `Create Dynamic Variable action already exists`.
* Subsequent test steps are not executed.

### **Possible Reasons**

This issue may occur due to one or more of the following reasons:

* **Duplicate Variable Names:** The script attempts to use a variable name that has already been assigned in a previous **Create Dynamic Variable** action.
* **Identical Variable Definitions:** Multiple instances of the same variable name exist within the script, causing a naming conflict during execution.

### Resolution/Solution

To resolve this issue and ensure successful execution, perform the following actions:

1. **Use Unique Variable Names:** Assign a unique name to every variable created using the **Create Dynamic Variable** action to avoid conflicts.
2. **Audit Existing Variables:** Review the script to identify any existing variables with the same name and rename them to maintain uniqueness.

Following these steps ensures that the system correctly allocates memory for each dynamic variable without encountering naming collisions.

### Additional Notes

* Always ensure that each dynamic variable is assigned a unique name to prevent naming conflicts during execution.
* When using a **Create Dynamic Variable** action inside a **For Loop**, the action may fail after the first iteration because the variable is created initially and subsequent iterations attempt to recreate the same variable.
* To prevent this error, place the **Create Dynamic Variable** action outside the loop or delete the created object using a delete action before the next iteration begins.
* **Example of loop management**:
  * **Method A**: Define the variable once outside the **For Loop**.
  * **Method B**: Use a cleanup action to delete the variable at the end of the loop before the next iteration attempts to create it again.
