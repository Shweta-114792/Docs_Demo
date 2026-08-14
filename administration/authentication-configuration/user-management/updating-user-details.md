# Updating User Details

This section explains how to update user information and manage client status in Avo Assure. You can edit a first name, last name, and password. Additionally, you can manage the client’s active status through the Avo Assure Client Provisions by reregistering or deregistering.

{% hint style="info" %}
**Note**: Only users with the **Quality Manager** role and **Admin** as a secondary role can update a user details.
{% endhint %}

You can manage user details and client status in Avo Assure using the following options:

* **Editing User Details**
* **Reregistering Avo Assure Client**
* **Deregistering Avo Assure Client**
* **Reprovisioning Avo Assure Client**

<details>

<summary><strong>Editing User Details</strong></summary>

{% hint style="info" %}
**Note**: You can edit or modify the user’s **Email Id**, **First Name**, **Last Name**, **Password**, **Confirm Password** and **Primary Role** of an existing user in Avo Assure. You cannot edit the **Configuration** and **User Name**.
{% endhint %}

To edit the details of an existing user in Avo Assure, perform the following actions:

1. On the **Home** page, in the left navigation pane, select **Admin** and select **User Management**.
2. Hover over the user you want to edit and select the **Edit** icon. The **Edit User** dialog opens.

<figure><img src="../../../.gitbook/assets/unknown (215).png" alt=""><figcaption></figcaption></figure>

3. Modify the required details and select **Update** to save the changes.

<figure><img src="../../../.gitbook/assets/unknown (216).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>Reregistering Avo Assure Client</strong></summary>

Reregistering an Avo Assure Client changes the client’s status to active.

To reregister an Avo Assure Client, perform the following actions:

1. On the **Home** page, in the left navigation pane, select **Admin** and select **User Management**.
2. Hover over the user you want to edit and select the **Edit** icon. The **Edit User** dialog opens.
3. Select the **Avo Assure Client Provision** tab.
4. On the **Actions** column, select **Reregister** to change an unregistered Avo Assure Client’s status from inactive to active.

{% hint style="info" %}
**Note**:

* After reregistering, the client’s status in the **Status** column changes to **registered**.
* After reregistering, Avo Assure generates a new token. Copy and paste the token in the client. To learn more, [click here](creating-new-user.md#registering-client-using-generated-token).
{% endhint %}

5. Select **Update** to save the changes and update the client provisions.

<figure><img src="../../../.gitbook/assets/unknown (217).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>Deregistering Avo Assure Client</strong></summary>

Deregistering an Avo Assure Client changes the client’s status to inactive.

To deregister an Avo Assure Client, perform the following actions:

1. On the **Home** page, in the left navigation pane, select **Admin** and select **User Management**.
2. Hover over the user you want to edit and select the **Edit** icon. The **Edit User** dialog opens
3. Select **Avo Assure Client Provision** tab.
4. On the **Actions** column, select **Deregister** to change a registered Avo Assure Client’s status from active to inactive.

<figure><img src="../../../.gitbook/assets/unknown (218).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Note**:

* After you select **Deregister**, it disappears from the **Actions** column.
* After deregistering, the client’s status in the **Status** column changes to deregistered.
{% endhint %}

<figure><img src="../../../.gitbook/assets/unknown (219).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>Reprovisioning Avo Assure Client</strong></summary>

Reprovisioning an Avo Assure Client generates a new client token and ensures the client is ready to register.

To reprovision an Avo Assure Client, perform the following actions:

1. On the **Home** page, in the left navigation pane, select **Admin** and select **User Management**.
2. Hover over the user you want to edit and select the **Edit** icon. The **Edit User** dialog opens
3. Select **Avo Assure Client Provision** tab.
4. On the **Actions** column, select **Reprovision** to refresh a registered Avo Assure Client token.

{% hint style="info" %}
**Note**: After reprovisioning, Avo Assure updates the token. Copy and paste the token in the client. To learn more, [click here](creating-new-user.md#registering-client-using-generated-token).
{% endhint %}

<figure><img src="../../../.gitbook/assets/unknown (220).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Note**: You can create multiple clients in the **Avo Assure Client Provisions** tab.
{% endhint %}

</details>
