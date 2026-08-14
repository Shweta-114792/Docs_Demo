# Creating Execution List

To create an execution list in Avo Assure, perform the following steps:

1. On the **Home** page, under **Projects**, select the required project from the list.
2. Select **Design Studio** > **Execution**.
3. Select **Create new folder.**\
   Here are the ways to create a new folder:

<details>

<summary><strong>a.</strong> <strong>Plus icon</strong> (<strong>+</strong>)</summary>

1. Select Plus icon **(+)** from left panel of the **Execution** tab.
2. Select **Create new folder**.

<figure><img src="../../../.gitbook/assets/image (4301).png" alt=""><figcaption></figcaption></figure>

3. Rename the folder with appropriate name.

<figure><img src="../../../.gitbook/assets/image (4358).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>b.</strong> <strong>Create Folder</strong></summary>

1. Select **Create Folder**. It is located at the center of the **Execution** tab.

{% hint style="info" %}
**Note**: You can use the shortcut key **Shift+F** to create a new folder.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4376).png" alt=""><figcaption></figcaption></figure>

2. Rename the folder with an appropriate name.

<figure><img src="../../../.gitbook/assets/image (4377).png" alt=""><figcaption></figcaption></figure>

</details>

5. Select **Create Execution List**.\
   Here are the ways to create a new folder:

<details>

<summary><strong>a. Plus icon</strong> (+)</summary>

1. Select Plus icon **(+)** from left panel of the **Execution** tab.
2. Select **Create new list** option.

<div align="left"><figure><img src="../../../.gitbook/assets/image (4304).png" alt=""><figcaption></figcaption></figure></div>

3. Rename the Execution List with an appropriate name.

<figure><img src="../../../.gitbook/assets/image (4359).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>b.</strong> <strong>Ellipsis</strong> icon (<strong>...</strong>)</summary>

1. Select Ellipsis icon **(...)** from the folder.
2. Select **Create Execution List** option.

<figure><img src="../../../.gitbook/assets/image (4303).png" alt=""><figcaption></figcaption></figure>

3. Rename the Execution List with an appropriate name.

{% hint style="info" %}
**Note**: You can use the shortcut key **Shift+L** to create a new Execution List.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4359).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>c. Create list</strong></summary>

1. Select **Create List.** It is at the center of the **Execution** tab.

<figure><img src="../../../.gitbook/assets/image (4360).png" alt=""><figcaption></figcaption></figure>

3. Rename the Execution List with an appropriate name.

{% hint style="info" %}
**Note**: You can use the shortcut key **Shift+L** to create a new Execution List.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4359).png" alt=""><figcaption></figcaption></figure>

</details>

7. Select **Profile Type** from the dropdown. Select either **Functional** or **Accessibility.**

* **Functional:** This profile type is used for regular execution modules, and it focuses on application's function.
* [**Accessibility**](accessibility-test.md)**:** This profile type is especially created for people with disabilities to use applications easily parallelly ensuring the platform’s availability for everyone while ensuring a good experience.

<figure><img src="../../../.gitbook/assets/image (4299).png" alt=""><figcaption></figcaption></figure>

8. Select [**On Failure** ](on-failure/)from the dropdown as per your requirement. For example: **Continue Run**, **Halt Run**, **Re-Run**, and **Run next Test Case**.

<figure><img src="../../../.gitbook/assets/image (4305).png" alt=""><figcaption></figcaption></figure>

9. Select **Add Test Case**. The **Test Cases** window appears.

<figure><img src="../../../.gitbook/assets/image (4309).png" alt=""><figcaption></figcaption></figure>

10. Drag Testcase from **Test Cases** window and drop it in Execution List

{% hint style="info" %}
**Note**:

* When you add a folder to the Execution List, the system includes all Testcases inside that folder and its subfolders.
* If you have created E2E flows, you can add them to the **Execution List**.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4308).png" alt=""><figcaption></figcaption></figure>

11. In the **Input Value**, enter the new Excel file path or Data Table path to override on the test data on Testcase. (If needed)

{% hint style="info" %}
**Example**:

When you used Test data through Data parameterization and in case it got changed, you can directly provide the new Excel path in the Input value instead of updating it inside every Testcase or Test Step Group.

**Example**:

* You have 5 Test Cases that use OldData.xlsx.
* Your test data changes, and you now have NewData.xlsx.
* Instead of updating each Test Case file path manually, you enter NewData.xlsx in the **Input Value** field.
* The Execution List runs all Test Cases using NewData.xlsx as the **globally declared data**, which **overrides** the Excel file paths in the individual Test Cases.
{% endhint %}

12. Select **On Failure** from the dropdown according to your requirement. By default, it is set to **Continue Run**.

{% hint style="info" %}
**Note**: You can select the **On Failure** type for an individual Testcase or for all Testcases in the Execution List.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4313).png" alt=""><figcaption></figcaption></figure>

13. Expand **Configuration** window from the right panel. Select active **Client**, **Agent**, or **Grid** to choose the execution mode:

* **Client**: Runs the Execution List on the local machine.
* **Agent**: Runs the Execution List on a remote machine and can execute tests in parallel or distributed mode using an installed Agent.
* **Grid**: Executes the Execution List in parallel or distributed mode across multiple machines.

{% hint style="info" %}
**Note**: You can execute the Execution List through **Client**, **Agent**, or **Grid**.
{% endhint %}

14. Select **Browser** for execution to specify the environment where the Testcases run.
15. Select **Save** to save all the configuration.

<figure><img src="../../../.gitbook/assets/image (4312).png" alt=""><figcaption></figcaption></figure>

16. Select parent folder and select **Execute.** The **Execution Now** pop-up appears.
17. Select **Execute** to execute the Execution List.

<figure><img src="../../../.gitbook/assets/image (4316).png" alt=""><figcaption></figcaption></figure>
