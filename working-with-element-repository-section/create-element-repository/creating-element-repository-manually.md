# Creating Element Repository Manually

In many projects, the user interface (UI) is built in stages, and not all screens or components are available during early test design activities. To avoid delays, expected UI elements can be defined early by adding them manually to the element repository.

Use manual element creation when application elements are not yet available for capture or when you want to define element details before the user interface is ready. This feature lets you add expected application objects directly to the element repository so that test design and repository preparation can continue independently of application readiness. After the actual interface becomes available, you can update or map these manually created elements to capture application objects.

## Key Benefits

* Enables Shift-Left Testing
* Parallel Test Development
* Faster Go-to-Market
* Effortless Maintenance
* Higher Sprint Productivity
* TDD-Test Driven Development

## Creating Elements Manually

Creating elements manually helps to define expected UI components before the actual interface is available. This allows test design to continue in parallel with development, ensuring faster readiness when the interface becomes accessible.

To create an element manually, perform the following actions:

1. On the **Home** page, under **Projects**, select the required **Project**.
2. ​Select **Design Studio**.
3. On the **Element Repository** page, locate the **Create Folder** (**+**) icon.

<figure><img src="../../../.gitbook/assets/unknown (262).png" alt=""><figcaption></figcaption></figure>

4. Select **Create Folder** (**+**) icon, and then select **Create main folder** to create a new element repository folder. A new folder is created.

{% hint style="info" %}
**Note**: To create a new parent folder in the **Element Repository**, select the workspace (blank space), and select the **Create Folder** (**+**) icon.
{% endhint %}

<figure><img src="../../../.gitbook/assets/unknown (263).png" alt=""><figcaption></figcaption></figure>

5. In the **New Folder** text box, enter the element repository folder name.
6. In the newly created folder, select the **Ellipsis** (**...**) icon next to the repository name, and then select **Create Repository** > **Web** to create the element repository.

{% hint style="info" %}
**Note**: You can manually create elements only for Web and Desktop applications in Avo Assure.
{% endhint %}

7. In the **New Repository** text box, enter the element repository name.
8. Select the **Create Manually** button to create elements manually. The **Create Element** dialog appears.

<figure><img src="../../../.gitbook/assets/unknown (264).png" alt=""><figcaption></figcaption></figure>

8. In the **Create Element** dialog, enter the **Element Name** that you want to capture from the application under test.
9. Select the **Element Type** from the dropdown list.

{% hint style="info" %}
**Note**: **Element Name** and **Select Element Type** are mandatory details. All other element attributes are optional and can be added as required.
{% endhint %}

10. Select **Submit** to create the elements.

{% hint style="info" %}
**Note**:

* A **Manual** label appears next to elements that you create manually.
* You can edit and delete the manually created elements using the edit and delete icons.
{% endhint %}

## Mapping Elements Manually

Mapping aligns the manually defined element with the actual UI element, ensuring that Avo Assure can locate and interact with it correctly during automated tests. Use this feature to link the manually created elements with corresponding captured elements in the element repository.&#x20;

To map a manually created element, perform the following actions:

1. On the **Element Repository** page, select **Tools**.

<figure><img src="../../../.gitbook/assets/unknown (265).png" alt=""><figcaption></figcaption></figure>

2. Select **Map Element**. The **Replace custom elements** dialog appears.
3. Under **Manually Created Elements**, select **Link** to expand the list of manually created elements.
4. Under **Captured Elements**, drag and drop the required captured element to the corresponding manually created element under **Link**.
5. Select **Submit** to save the mapping.

{% hint style="info" %}
**Note**:

* Mapping is supported only between elements of the same object type.
* Select **Show All Elements** to display all available captured elements.
* Select **Un-Link** to remove an existing mapping.
{% endhint %}

<figure><img src="../../../.gitbook/assets/unknown (266).png" alt=""><figcaption></figcaption></figure>
