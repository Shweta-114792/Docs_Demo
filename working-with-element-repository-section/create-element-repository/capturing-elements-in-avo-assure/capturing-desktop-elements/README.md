# Capturing Desktop Elements

Capturing desktop elements allows you to identify and store UI elements from desktop applications in the Element Repository. These elements are used while designing and executing automated test scenarios in Avo Assure. This topic describes how to capture the desktop elements using the Avo Assure Client.

## Prerequisites

* Ensure that the target desktop application is installed on your system.
* Ensure that the Avo Assure Client is connected.

## Capturing Elements from Desktop Applications

To capture desktop elements, perform the following actions:

1. ​On the **Home** page, under **Projects**, select the required Project.
2. ​Select **Design Studio**.
3. On the **Element Repository** page, select the **Create Folder** (**+**) icon.

<img src="../../../../../../.gitbook/assets/unknown (262).png" alt="" height="210" width="624">

4. Select **Create main folder** to create a new element repository folder. A new folder appears.
5. In the **New Folder** text box, enter the element repository folder name.
6. In the newly created folder, select the Ellipsis (**...**) icon next to the folder name, and then select **Create Repository** > **Desktop**. The desktop element repository is created.
7. Select **Capture Elements**. The **Avo Assure Client – Capture** window opens.
8. In **Step 1: Enter Window Name/Process ID** box, enter the window name or process ID of the desktop application.

<img src="../../../../../../.gitbook/assets/unknown (353).png" alt="" height="330" width="520">

9. Select **Launch**. The specified desktop application is launched.
10. In **Step 2: Capture Element**, select an element capture method.\
    The following capture methods are available:

| Capture Method | Description                                                             |
| -------------- | ----------------------------------------------------------------------- |
| Visible        | Captures visible elements in the AUT.                                   |
| <p><br></p>    |                                                                         |
| All            |                                                                         |
| <p><br></p>    | Captures all elements in the AUT, including hidden elements.            |
| Manual         |                                                                         |
| <p><br></p>    | Allows you to manually navigate to AUT and capture elements.            |
| IRIS           | Captures elements based on screen coordinates and positions in the AUT. |

<details>

<summary><strong>Configuring Capture Settings</strong></summary>

* **Capture Type**: Select the specific element types to capture.
* **Method**:
  * **UI/UIA**: Use for modern applications that support Microsoft UI Automation. This method identifies elements with standard UI structures.\
    **Note**: Use the UI method by default. If it does not work, use UIA.
  * **Win32**: Use for legacy applications that do not fully support UI Automation. This method uses Windows API-based identification.
* **Option**: Select the type of capture option.

</details>

11. Select **Capture** to start the element capturing process.
12. Select **Add**. The selected elements are added to the element repository.

{% hint style="info" %}
**Note**:

* Select **Locate** to highlight the corresponding elements in the application UI.
* Select **Delete** to remove the selected elements from the capture list.
{% endhint %}
