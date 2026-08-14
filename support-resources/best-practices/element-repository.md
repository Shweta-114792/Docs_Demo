# Element Repository

Use this section to learn best practices for working with the Element Repository. This provides recommended approaches for organizing repositories, structuring elements, and maintaining reusable components for scalable and consistent test automation in Avo Assure.

*   **Create folders map to your automation flow.**\
    Organize Test cases and related assets into folders that reflect the actual workflow of the application under test. Structuring folders based on the automation flow helps users quickly locate test cases, understand the sequence of actions. It also improves collaboration among team members by providing a clear and consistent structure.

    **For Example**: Common Workflow-Based Folder Structure\
    Create a main folder representing the overall automation area or application module. Inside this folder, create subfolders based on the major stages of the workflow.
* **Organize elements based on elements role in the flow.**\
  Organize elements based on their role in the automation flow. Use common module folders for setup steps like Login or Logout, Product Purchase elements for core actions like Add to Cart, and Payment Process for different payment methods. This improves clarity and reuse across Test Cases.
* **Rename elements immediately after capturing.**\
  Rename elements right after capturing them to avoid confusion. For example: If **Login** appears on multiple pages, rename it to something specific such as **Login Home**.
* **Regularly review and clean the repository.**\
  Regularly review your repository and remove unused or outdated elements to keep it clean, organized, and efficient.
* **Select the appropriate capture method.**\
  Choose the appropriate capture methods such as Manual, Visible, or All based on your application type and automation requirement.
* **Keep the Show Status Option Enabled**\
  Ensure that **Show Status** is enabled to easily monitor the review status of items in the repository. This helps users quickly identify whether an artifact is **Under Review**, **Approved**, or **Rejected**. Keeping this option enabled improves visibility and allows teams to track the progress of review and approval processes efficiently.
