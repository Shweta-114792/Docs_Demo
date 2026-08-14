# Test Case

Use this section to learn tips and tricks for creating and managing Test Cases. These help you to organize test cases clearly, reuse steps where possible, and use test data effectively to make automation easier to manage.

<details>

<summary><strong>Speed Up Test Design with Add from Repository</strong></summary>

Use **Add from Repository (Drag and Drop)** to quickly add elements to your test case and automatically map the relevant actions, reducing manual effort and accelerating test creation.

</details>

<details>

<summary><strong>Use Agent or Grid Execution for Large Test Suites</strong></summary>

Run large test cases using **Agent** or **Grid Execution** to execute multiple test cases in parallel and reduce the overall execution time.

</details>

<details>

<summary><strong>Use Scrollbar Elements for Reliable Grid Scrolling</strong></summary>

For Microsoft Dynamics 365 grids, use the **scrollbar elements** with **Verify Exist** followed by **Click Element** instead of the **Scroll Vertical** or **Scroll Horizontal** grid actions to achieve more reliable vertical and horizontal scrolling during automation.

</details>

<details>

<summary><strong>Verify the Tab State Before Interacting with Dynamics 365 Tabs</strong></summary>

Check whether a **Dynamics 365** tab is expanded before interacting with its fields. If the tab is collapsed, expand it first to ensure all required fields are accessible and prevent execution failures.

</details>

<details>

<summary><strong>Use Get Specific Object for Dynamic Web Elements</strong></summary>

Use **Get Specific Object** to dynamically locate and store web elements as reusable reference objects, enabling reliable interaction with dynamic grids and complex UI structures without creating custom XPath expressions.

</details>

<details>

<summary><strong>Validate UI Table Data Against Downloaded Excel</strong></summary>

Use **Excel Actions**, **dynamic variables**, and **loops** to compare UI table data with downloaded Excel data row by row, ensuring accurate and scalable data validation.

</details>
