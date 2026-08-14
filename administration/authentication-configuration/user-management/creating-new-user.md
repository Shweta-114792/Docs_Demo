# Creating New User

The Create User page includes the following options:

* [**User Details**](creating-new-user.md#adding-user-details): It is used to enter basic user information, such as login details and role configuration.
* [**Avo Assure Client Provision**](creating-new-user.md#generating-an-avo-assure-client-token): It used to assign and manage Avo Assure Client access for the user.

## Adding User Details

To create a new user in Avo Assure, preform the following actions:

1. On the **Home** page, in the left navigation pane, select **Admin** and select **User Management**.
2. Select **Create** to add a new user. The **Create User** dialog opens.

<figure><img src="../../../.gitbook/assets/unknown (209).png" alt=""><figcaption></figcaption></figure>

3. **Select Configuration**:\
   Configurations in Avo Assure allow you to manage user login using the following authentication configurations:

* **Default**: Select this option for standard authentication. Avo Assure creates a unique username and password for login.
* **LDAP**: Select this option to integrate with the Lightweight Directory Access Protocol (LDAP). This option allows you to log in using existing organizational credentials, such as Active Directory. To learn more, [click here](../authentication-configuration/ldap-configuration/creating-ldap-configuration-in-avo-assure.md).
* **SAML**: Select this option to enable Single Sign-On (SSO) using Security Assertion Markup Language (SAML). This option allows you to authenticate through an external Identity Provider (IdP), such as Okta or Azure AD. To learn more, [click here](../authentication-configuration/saml-configuration.md).

4. Enter the required details for the following:
   * **Username**: Enter a unique username for the user.
   * **Email ID**: Enter a valid email address for the user.
   * **First Name**: Enter the user’s first name.
   * **Last Name**: Enter the user’s last name.
   * **Password**: Enter a password for the user.
   * **Confirm Password**: Re-enter the password to confirm it.
5. Select the user role from the **Primary Role** dropdown.

{% hint style="info" %}
**Note**: When you select **Quality Manager** as the primary role, the **Secondary Role** option appears. Select the checkbox to assign Admin as a secondary role. To learn more, [click here](users-roles-and-permissions.md).
{% endhint %}

6. Select the **Create**. A success message appears: **User Created Successfully!**

## Generating an Avo Assure Client Token

Each Avo Assure user requires a unique Avo Assure Client Token to register with the Avo Assure Client. This token ensures that only the specific user can access and use the client.

{% hint style="info" %}
**Note**: After you create a user in **User Details**, the system automatically directs you to the **Avo Assure Client Provisions** to generate and manage the client’s provisions.
{% endhint %}

To generate a client token in Avo Assure, perform the following actions:

1. On the **Avo Assure Client Provision** tab, enter the client name in the **Avo Assure Client Name** box
2. Select **Generate** to create a new token.

<figure><img src="../../../.gitbook/assets/unknown (210).png" alt=""><figcaption></figcaption></figure>

3. Select **Copy** icon to copy the generated token.

{% hint style="info" %}
**Note**: You can also select Download icon to save the generated token.
{% endhint %}

4. Select **Create** to create a user profile.

<figure><img src="../../../.gitbook/assets/unknown (224).png" alt=""><figcaption></figcaption></figure>

### Registering Client Using Generated Token

After you generate the Avo Assure Client Token, you register the client to connect it to the Avo Assure server. You provide the generated token during registration to authenticate the client and enable access.

1. On the **Avo Assure Client**, select **Connect** or **Register**. The **Avo Assure Client Registration** dialog opens.
2. Paste the generated token into the **Token** box.

<figure><img src="../../../.gitbook/assets/unknown (213).png" alt=""><figcaption></figcaption></figure>

3. Select **Submit** to complete the client registration.

<figure><img src="../../../.gitbook/assets/unknown (214).png" alt=""><figcaption></figcaption></figure>

4. Select **Connect** to connect the client to the Avo Assure instance, execute the test, and view the status on the **Console Logs** page.
