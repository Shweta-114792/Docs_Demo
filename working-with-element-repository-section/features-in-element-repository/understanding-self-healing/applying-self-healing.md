# Applying Self Healing

To apply self healing, perform the following actions:

1. On the **Home** page, from **Projects** list, select required project.
2. Select **Design Studio**.
3. In the **Element Repository** page, select the required element repository for which you want to apply self healing.
4. Select **Tools** > **Self Heal**. The **Self Heal** dialog opens.

<img src="../../../../../.gitbook/assets/unknown (322).png" alt="" height="306" width="686">

3. In the **Self Heal** dialog, choose one of the following options:
   1. **Enable Self Heal**
      1. Select **Adjust the broken elements attributes** to update the attributes of elements that were not detected during execution.
      2. Select **Preserve the properties of reprioritized items** for subsequent execution to prioritize the most stable properties for future runs.
   2. **Disable Self Heal**
      1. Select this option to disable self heal.
4. Select one of the following actions:
   1. **Apply for all repositories** to apply the selected option across all repositories.
   2. **Apply to current repository** to apply the selected option only to the current repository.

{% hint style="info" %}
**Note**: Select **Cancel** to close the dialog without making changes.
{% endhint %}

5. After you apply self healing to the repositories, the **Self Heal** icon appears.

<figure><img src="../../../../../.gitbook/assets/unknown (1) (2) (1).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Note**:&#x20;

* Self-healing is only applicable to elements captured through the Avo Assure Client. It does not work for manually created elements.
* Successful element recovery in Self Heal does not necessarily update the visible properties in the Element Repository. This is expected behaviour, as self healing relies on more than just the displayed locators to identify elements.
{% endhint %}
