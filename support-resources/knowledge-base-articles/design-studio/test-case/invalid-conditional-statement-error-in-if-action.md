# Invalid Conditional Statement Error in IF Action

**Summary**: The **IF** action fails during test execution if the conditional expression provided in the input is not written in the correct format. When this occurs, the step stops executing and an error message appears in the **Avo Assure Client** log. Ensuring that the conditional expression follows the correct syntax prevents execution failures.

### **Error Behavior**

When this issue occurs, users may observe the following behavior:

* The **IF** action step stops execution during test execution.
* The test case execution does not proceed to the next step.
* The following error message appears in the **Client log**: `Invalid Conditional Statement`.

### **Possible Reasons**

* This issue may occur due to one or more of the following reasons:
  * **Invalid syntax**: The conditional expression contains characters not supported by the engine (e.g., semicolons `;` used as delimiters).
  * **Incorrect operator placement**: Misplaced logical operators (**AND**/**OR**) or comparison operators (e.g., `>=`).
  * **Improper use of parentheses**: Unbalanced or missing brackets in the expression.
  * **Incorrect formatting of logical operators**: Using lowercase (e.g., `and`) instead of the required uppercase (**AND**).
  * **Extra spaces**: Whitespace inside variable braces (e.g., `{ Val }` instead of `{Val}`).
* **Example of an incorrect conditional expression:**\
  `(({Val};>=;150);AND;({Val };<=;300))`\
  &#xNAN;_&#x54;his fails because it uses semicolons and extra spaces._

### **Resolution/Solution**

To resolve this issue, ensure the conditional expression follows the correct syntax and logical structure.

* Correct syntax rules are:

| Component             | Requirement                                          | Example                          |
| --------------------- | ---------------------------------------------------- | -------------------------------- |
| **Variables**         | Enclose in `{ }` without extra spaces.               | `{Val}`                          |
| **Comparison**        | Use standard operators (`>`, `<`, `==`, `>=`, `<=`). | `{Val}>=150`                     |
| **Logical Operators** | Use **AND** / **OR** (uppercase).                    | `({Val}>=150) AND ({Val}<=300)`  |
| **Parentheses**       | Must be balanced and properly nested.                | `((Condition1) OR (Condition2))` |
| **Delimiters**        | Do not use semicolons (`;`).                         |  `({Val};>=;150)` is invalid.    |

* **Correct example**:\
  `(({Val}>=150) AND ({Val}<=300))`\
  &#xNAN;_&#x54;his ensures the **IF** action evaluates the condition correctly._

### Example

**Scenario**: A user configures an **IF** action to verify whether a value falls within a range (150–300).

* **Incorrect Condition**: `(({Val};>=;150);AND;({Val };<=;300))`
* **Result**: Execution fails with the error: `Invalid Conditional Statement`.
* **Correct Condition**: `(({Val}>=150) AND ({Val}<=300))`
* **Resolution**: After correcting the syntax, the **IF** action evaluates successfully and the test execution proceeds.

### Additional notes

* Always ensure that conditional expressions follow the correct syntax before executing the test case.
* When combining multiple conditions, use logical operators such as **AND** or **OR** with proper parentheses.
* Verify that input values and operators are correctly defined to avoid syntax errors.
* **Example of multiple conditions:**\
  `((({Val}>=150) AND ({Val}<=300)) OR ({Val}==200))`\
  This structure ensures that multiple conditions are evaluated correctly during execution.
