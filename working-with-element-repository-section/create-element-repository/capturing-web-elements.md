# Capturing Web Elements

Web element capture identifies the User Interface (UI) components from the Application Under Test (AUT) and adds them to a web element repository. The captured elements help you interact with UI components during test creation and execution. This article describes how to capture the web elements using Avo Assure.

## Prerequisite

Ensure that the Avo Assure Client is connected.

## Capturing Web UI Elements

To capture web elements, perform the following actions:

1. On the **Home** page, under **Projects**, select the required Project.
2. ​Select **Design Studio**.
3. ​On the **Element Repository** page, select the **Create Folder (+)** icon.

![](<../../../../../.gitbook/assets/unknown (262).png>)

4. Select **Create main folder** to create a new element repository folder. A new folder appears.
5. In the **New Folder** text box, enter the element repository folder name.
6. In the newly created folder, select the Ellipsis (**...**) icon next to the repository name, and then select **Create Repository** > **Web** to create the element repository.
7. Select **Capture Elements**. The **Select Browser** dialog box opens.
8. Select the required browser, and then select **Capture**. The **Avo Assure Client – Capture** window opens.
9. In **Step 1: Enter URL** box, enter the URL of the AUT.

<img src="../../../../../.gitbook/assets/unknown (350).png" alt="" width="563">

10. Select **Navigate**. You are redirected to the specified URL.
11. In **Step 2: Capture Element**, select one of the following capture methods:
    * **Visible**: Captures visible elements in the AUT.
    * **All**: Captures all elements in the AUT for every Capture Type, including hidden elements.
    * **Manual**: Allows you to manually navigate to AUT and capture elements.
12. Depending on the selected capture method, perform one of the following actions:
    * **Visible** or **All**: From the **Capture Type** dropdown, select the element types to capture.
    * **Manual**: From the **Delay** dropdown, select a delay duration to capture the elements with longer loading time.
13. Select **Capture** to start the element capturing process.
14. Select **Add**. The selected elements are added to the element repository.

{% hint style="info" %}
**Note**:

* Select **Locate** to highlight the corresponding elements in the application UI.
* Select **Delete** to remove the selected elements from the capture list.
{% endhint %}
