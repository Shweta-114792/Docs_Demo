# Capturing SAP Elements

SAP element capture identifies the User Interface (UI) components from the Application Under Test (AUT) and adds them to SAP element repository. The captured elements help you interact with UI components during SAP automation test cases. Use this article to understand how to capture SAP application elements and add them to an element repository in Avo Assure.

## Prerequisite

Ensure that the Avo Assure Client is connected.

## Capturing SAP Application Elements

To capture SAP elements, perform the following actions:

1. On the **Home** page, under **Projects**, select the required Project.
2. Select **Design Studio**.
3. On the **Element Repository** page, select the **Create Folder** (**+**) icon.
4. Select **Create main folder** to create a new element repository folder. A new folder appears.
5. In the **New Folder** text box, enter the element repository folder name.
6. In the newly created folder, select the Ellipsis (**...**) icon next to the repository name, and then select **Create Repository** > **SAP** to create the element repository.
7. Select **Capture Elements**. The **Avo Assure Client – Capture** window opens.
8. In **Step 1: Enter SAP Application Path** box, enter the SAP Application Path. The path must include the application path, server name, and window name. \
   **Example**: &#x20;

```
C:\Program Files (x86)\SAP\FrontEnd\SapGui\saplogon.exe;SAP HANA;SAP Logon 760
```

In this example:&#x20;

* **Application Path**: C:\Program Files (x86)\SAP\FrontEnd\SapGui\saplogon.exe
* **Server Name**: SAP HANA
* **Window Name**: SAP Logon 760

9. Select **Launch**. You are redirected to the application.
10. In **Step 2: Capture Element**, select one of the following capture methods:
    * **Actionable**: Captures only the interactive elements in the AUT. Hidden and non-interactive elements are not captured.
    * **All**: Captures all elements in the AUT for every Capture Type, including hidden elements.
    * **Manual**: Allows you to manually navigate to AUT and capture elements.
11. Depending on the selected capture method, perform one of the following actions:
    * **Actionable** or **All**: From the **Capture Type** dropdown, select the element types to capture.&#x20;
    * **Manual**: From the **Delay** dropdown, select a delay duration to capture the elements with longer loading time.
12. Select **Capture** to start the element capturing process.
13. Select **Add**. The selected elements are added to the element repository.

{% hint style="info" %}
**Note**:

* Select **Locate** to highlight the corresponding elements in the application UI.
* Select **Delete** to remove the selected elements from the capture list.
{% endhint %}
