# Performing Post Upgrade Activities in Avo Assure

**Summary**: After upgrading to a new version of **Avo Assure**, some users may not be able to execute tests or use the platform features if the Avo Assure Client is not updated, installed, or connected properly. Post-upgrade steps ensure that the client application is correctly configured so that the latest updates, fixes, and improvements function as expected.

### Error Behavior

Users may experience the following issues after upgrading:

* Avo Assure Client fails to connect to the Avo Assure instance.
* Test execution cannot start from the client machine.
* Client shows connection or registration errors.
* Updated features or fixes are not reflected in the client.

### Possible Reasons

* The existing Avo Assure Client is not updated after a product upgrade.
* The Avo Assure Client is not installed for new users.
* The client is not connected to the Avo Assure instance using a valid token.
* The client registration process is incomplete.

### Resolution/Solution

To ensure smooth operation after an upgrade, perform the following steps based on the user scenario.

#### 1. Updating Avo Assure Client for Existing Users

If you already have Avo Assure Client installed, update it to the latest version.

To update the client with latest version, perform the following actions:

1. Open **Avo Assure Client**.
2. Select the **Help** tab.
3. Select **Check for Updates**.
4. In the **Update Available** dialog, select **Update**.
5. After the update completes, the **Update Complete** dialog appears.
6. Select **OK** and restart the **Avo Assure Client**.

{% hint style="info" %}
To learn more about updating the Avo Assure Client for Existing Users, refer to [Updating Avo Assure Client](../../../avo-assure-client/features-of-avo-assure-client/monitoring-and-managing-client.md#help).
{% endhint %}

<details>

<summary><strong>Automatic Avo Client Updates</strong></summary>

The Avo Client now manages updates automatically. When a new version is available, the client downloads and installs it for you. This helps you stay up to date with the latest features, improvements, and fixes without any manual effort.

To enable automatic updates, perform the following actions:

1. Open the **Avo Assure Client**.

{% hint style="info" %}
**Note**: If you are using an older version of the **Avo Client**, download and install the latest **Avo Client** to enable automatic updates.
{% endhint %}

2. Select **Configuration** > [**Settings**](performing-post-upgrade-activities-in-avo-assure.md#settings).
3. Select **Update Check** setting as **Yes.**

{% hint style="info" %}
**Note**: The **Update Check** setting must be set to **Yes** for automatic updates to work. To learn more about [**Avo Client Updates**](../../../avo-assure-client/features-of-avo-assure-client/monitoring-and-managing-client.md#automatic-avo-client-updates).
{% endhint %}

</details>

#### 2. Downloading Avo Assure Client for New Users

If the client is not installed on the system, download it from the Avo Assure portal.

To download the Avo Assure Client, perform the following actions:

1. On the **Home page**, select the **Profile** icon.
2. Select **Downloads**.
3. Select **Download Client**.
4. The **Avo Assure Client (.exe)** file downloads to your system.

{% hint style="info" %}
To learn more about downloading the Avo Assure Client, refer to [Downloading Avo Assure Client | Avo Assure.](../../../avo-assure-client/downloading-avo-assure-client.md)
{% endhint %}

#### 3. Installing Avo Assure Client

After downloading the client, install it on your machine.

To install the Avo Assure Client, perform the following actions:

1. Open the **Downloads** folder.
2. Select **Avo Assure Client.exe**.
3. In the **Setup – Avo Assure Client** dialog, select **Next**.
4. Choose the **Destination Location** and select **Next**.
5. Select **Finish** to complete the installation.

{% hint style="info" %}
To learn more about the installing Avo Assure Client, refer to [Installing Avo Assure Client | Avo Assure](../../../avo-assure-client/installing-avo-assure-client.md).
{% endhint %}

#### 4. Generating Token and Connecting Avo Assure Client

After installation, the client must be connected to the Avo Assure instance.

To generate token and connect the Avo Assure Client with Avo Assure instance, perform the following actions:

1. On the **Home** page, select the **Profile** icon.
2. Select **Token Management**.
3. The **Avo Assure Client Provision** dialog opens.
4. Select **Generate** to create a token.
5. Copy the generated token.
6. Open **Avo Assure Client** on your system.
7. Select **Register**.
8. In the **Avo Assure Client Registration** dialog, paste the copied token in the **Token** field.
9. Select **Connect** to complete the registration.

{% hint style="info" %}
To learn more about managing token, refer to [Managing Avo Assure Client Token | Avo Assure](../../../avo-assure-client/managing-avo-assure-client-token.md)
{% endhint %}

### Additional Notes

* Use a valid and active token when registering the client with the Avo Assure instance.
