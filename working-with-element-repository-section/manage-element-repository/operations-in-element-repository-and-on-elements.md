# Operations on Element Repository and Elements

The Element Repository stores captured UI elements that are used during test creation and execution. This page describes how to manage repositories and captured elements, including renaming, copying, deleting, editing, and moving elements within the repository.

This section describes the following operations available in the Element Repository:

* **Operations on Element Repository**
* **Operations on Elements**

## **Operations on Element Repository**

Avo Assure provides options to manage repositories and folder. The following operations helps you to manage and organize the Element Repository efficiently.

<details>

<summary><strong>Rename Element Repository</strong></summary>

To rename an Element Repository, perform the following actions:

1. On the **Element Repository** page, select the required repository folder.

{% hint style="info" %}
**Note**: To know more about how to create Element Repository, [click here](../create-element-repository/creating-element-repository-manually.md#creating-elements-manually).
{% endhint %}

2. Select the **Ellipsis** (**...**) icon next to the repository name.
3. Select **Rename** from the dropdown list.
4. Enter a logical name for the folder.

{% hint style="info" %}
**Note**: You can also rename the sub-folder created under the repository.
{% endhint %}

![](<../../../../.gitbook/assets/unknown (306).png>)

</details>

<details>

<summary><strong>Copy Element Repository</strong></summary>

To copy an Element Repository, perform the following actions:

1. Select the **Ellipsis** (**...**) icon next to the repository folder.
2. Select **Copy** from dropdown list.

{% hint style="info" %}
**Note**: You can also copy the repository using the **Shift + C** keyboard shortcut.
{% endhint %}

![](<../../../../.gitbook/assets/unknown (307).png>)

</details>

<details>

<summary><strong>Paste Repository</strong></summary>

To paste a repository, perform the following actions:

1. On the **Element Repository** page, go to the folder where you want to paste the repository.
2. Select the **Ellipsis** (**...**) icon next to the folder name.
3. Select **Paste** from the list.
4. The system pastes the copied repository into the selected folder.

</details>

<details>

<summary><strong>Delete Element Repository</strong></summary>

To delete an Element Repository, perform the following actions:

1. On the **Element Repository** page, select the required repository folder.
2. Select the **Ellipsis** (**...**) icon next to the repository name.
3. Select **Delete** from the dropdown list. The **Safet to Delete** dialog box opens.

![](<../../../../.gitbook/assets/unknown (308).png>)

4. Select **Yes** to confirm the deletion in the confirmation dialog.

{% hint style="info" %}
**Note**: You cannot delete a repository if it is used in any **Test case** or **Test Step Group**. Remove those elements from the listed Test cases before deleting it.
{% endhint %}

![](<../../../../.gitbook/assets/unknown (309).png>)

</details>

<details>

<summary><strong>Assign Repository</strong></summary>

To assign a repository, perform the following actions:

1. On the **Element Repository** page, locate the required repository folder.
2. Select the **Ellipsis** (**...**) icon next to the repository name.
3. Select **Assign Repository** from the list. The **Assign Elements in Repository** dialog box opens.

![](<../../../../.gitbook/assets/unknown (310).png>)

4. Select the required user from the list.
5. Select **Assign** to assign repository to the selected user.

{% hint style="info" %}
**Note**: Only users with the **Quality Manager** or **Quality Lead** role can assign a repository to the user.
{% endhint %}

![](<../../../../.gitbook/assets/unknown (311).png>)

</details>

<details>

<summary><strong>Make a Root Folder</strong></summary>

To make a sub-folder a root folder, perform the following actions:

1. On the **Element Repository** page, locate the required sub-folder.
2. Select the **Ellipsis** (**...**) icon next to the sub-folder name.
3. Select **Make a Root Folder** from the list. The **Confirmation** dialog box opens.

![](<../../../../.gitbook/assets/unknown (312).png>)

4. Select **Yes**.

![](<../../../../.gitbook/assets/unknown (314).png>)

5. The system moves the selected sub-folder to the root level of the Element Repository.

{% hint style="info" %}
**Note**: This option is available only for sub-folders.
{% endhint %}

![](<../../../../.gitbook/assets/unknown (315).png>)

</details>

<details>

<summary><strong>Version History</strong></summary>

To view the version history, perform the following actions:

1. On the **Element Repository** page, locate the required repository.
2. Select the **Ellipsis** (**...**) icon next to the repository name.
3. Select **Version History** from the list.
4. The system displays the list of previous versions of the repository.

{% hint style="info" %}
**Note:** Version history lists are available only when version control (for example, **Bitbucket**, **Git** or **Assure DevOps**) is configured and changes are pushed to the repository.
{% endhint %}

</details>

<details>

<summary><strong>Send For Review</strong></summary>

To send a repository for review, perform the following actions:

1. On the **Element Repository** page, locate the required repository.
2. Select the **Ellipsis** (**...**) icon next to the repository name.
3. Select **Send for Review** from the list.
4. The system sends the repository for review.

{% hint style="info" %}
**Note:** Only users with the **Quality Manager** or **Quality Lead** role can send a repository for review.
{% endhint %}

</details>

## **Operations on Elements**

Avo Assure provides options to manage elements in repository. The following operations helps you to manage and organize the Element Repository efficiently.

<details>

<summary><strong>Rename Element</strong></summary>

To rename a captured element, perform the following actions:

1. On the **Element Repository** page, select the required repository.
2. Double-click on the name of the captured element.
3. Enter a logical name for the element.

</details>

<details>

<summary><strong>Delete Element</strong></summary>

To delete an element, perform the following actions:

1. On the **Element Repository** page, select the required repository.
2. In the **Element List**, select the element that you want to delete.
3. Select the **Delete** icon and then confirm the deletion in the confirmation dialog.

{% hint style="info" %}
**Note**:

* You can delete elements individually or delete multiple elements at once.
* You cannot delete an element if it is used in any Test case or Test Step Group. Remove the element from the listed test cases before deleting it.
{% endhint %}

</details>

<details>

<summary><strong>Cut and Paste Elements</strong></summary>

To cut and paste elements, perform the following actions:

1. On the **Element Repository** page, open the required repository.
2. Select the element that you want to move.
3. Select the **Cut** icon at the top.
4. Navigate to the destination repository.
5. Select the **Paste** icon to add the element.
6. Select **Save** to save the changes.

{% hint style="info" %}
**Note**: You can move captured elements from one repository to another using the **Cut** and **Paste** options.
{% endhint %}

</details>

<details>

<summary><strong>Edit Element Properties</strong></summary>

To edit element properties, perform the following actions:

1. On the **Element Repository** page, select the required repository.
2. Select the element that you want to edit.
3. Hover over the empty column next to the element and select the **Edit** icon. The **Details** pane opens.
4. Modify the required property values.
5. Select **Save Properties** to save the changes.

{% hint style="info" %}
**Note:** You can also drag and drop properties to change their priority.
{% endhint %}

</details>

<details>

<summary><strong>View Test Cases for an Element</strong></summary>

To view the test cases for an element, perform the following actions:

1. On the **Element Repository** page, navigate to the required repository.
2. Locate the element for which you want to view the test case usage.
3. Select the **View Test Cases** icon next to the element.
4. The system displays the list of test cases where the selected element is used.

{% hint style="info" %}
**Note**: You can view the Test cases in which a specific element is used. This helps you identify where the element is referenced in your Test cases.
{% endhint %}

</details>
