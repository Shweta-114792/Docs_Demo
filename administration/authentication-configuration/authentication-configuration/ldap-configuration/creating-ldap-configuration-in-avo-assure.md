# Creating LDAP Configuration in Avo Assure

## Configuration Fields

Following are the configuration fields which are required while establishing the LDAP Configuration:

* **Server Name**: Name to identify your LDAP server.\
  Example: Corporate AD Server
* **Server URL**: The LDAP server connection string.\
  Format: ldap://\<hostname>:\<port> or ldaps://\<hostname>:\<port>\
  Example: ldap://ad.example.com:389.
* **Base Domain Name**: The root Distinguished Name (DN) of your directory where user searches begin. Example: DC=example,DC=com.
* **Secure Connection**: Choose whether to use a TLS secured connection when configuring the connection settings.
  * **Disable**: Plain connection (not recommended).
  * **Enable**: Secure connection (recommended).
  * **Enable Insecure**: Use Start TLS without verifying certificates.
* **TLS Certificate**: Upload your LDAP server’s TLS certificate if using Enable secure mode and ensures encrypted communication between Avo Assure and LDAP.
* **Authentication**: Defines how Avo Assure binds to the LDAP server.
  *   **Anonymous**: Connects without credentials (only works if LDAP server allows anonymous

      search).
  * **Simple**: Requires Bind Principal (username) and Bind Credentials (password) to authenticate.
    * **Bind Principal**: The account used by Avo Assure to query the LDAP directory.\
      Format: CN=ldap-user,OU=ServiceAccounts,DC=example,DC=com.
    * **Bind Credentials**: Password for the above bind account.

### Data Mapping Settings

Data Mapping Settings is also a part of Configuration Fields which ensures user details from LDAP are correctly imported into Avo Assure.

Use these dropdowns to map LDAP attributes to Avo Assure user fields:

* **Username**: Typically sAMAccountName or uid.
* **Firstname**: Maps to Name.
* **Lastname**: Maps to Surname.
* **Email**: Maps to mail.

## Creating LDAP Configuration

To create a LDAP configuration, perform the following actions:

1. On the **Home** page, select **Admin** option. The **Account Management** page opens.
2. Select **LDAP Configuration** tab.

<figure><img src="../../../../.gitbook/assets/Screenshot 2025-10-15 150911.png" alt=""><figcaption></figcaption></figure>

3. Enter the LDAP server details: **Server Name**, **Server URL** and **Base Domain Name**.
   1. **Server Name**: Name to identify your LDAP server.\
      Example: Corporate AD Server
   2.  **Server URL**: The LDAP server connection string.\
       Format: ldap://\<hostname>:\<port> or ldaps://\<hostname>:\<port>

       Example: ldap://ad.example.com:389.
   3. **Base Domain Name**: The root Distinguished Name (DN) of your directory where user searches begin.\
      Example: DC=example,DC=com.

<figure><img src="../../../../.gitbook/assets/Server name.png" alt=""><figcaption></figcaption></figure>

4. Select **Secure Connection**.
   1. **Disable**: TLS Certificate is not required when **Disabled Secure Connection.**
   2. **Enable**: Select and provide **TLS Certificate** from the system when **Enabled Secure Connection**.
   3. **Enable Insecure**: Select and provide **TLS Certificate** from the system when **Enabled Insecure** Connection.

<figure><img src="../../../../.gitbook/assets/Secure connection.png" alt=""><figcaption></figcaption></figure>

6. Select **Authentication** mode:
   1. **Anonymous**: No credentials are required when **Anonymous** mode is selected.
   2. **Simple**: Enter **Bind Principal** and **Bind Credentials** when **Simple** mode is selected.
      1. **Bind Principal**: The account used by Avo Assure to query the LDAP directory.\
         Format: CN=ldap-user,OU=ServiceAccounts,DC=example,DC=com.
      2. **Bind Credentials**: Password for the above bind account.

<figure><img src="../../../../.gitbook/assets/Authentication.png" alt=""><figcaption></figcaption></figure>

7. In **Data Mapping Settings**, form **Username** dropdown, select username.
8. From **Firstname** dropdown, select first name.
9. From **Lastname** dropdown, select last name.
10. From **Email** dropdown, select mail id.

<figure><img src="../../../../.gitbook/assets/mapping setting.png" alt=""><figcaption></figcaption></figure>

11. Select **Create** button to create the LDAP configuration.
12. Try login with a user account which is now configured in LDAP.

## Notes and Best Practices

Here are the notes and best practices which you should follow while configuring LDAP:

1. Always prefer secure LDAP (LDAPS, port 636) to protect credentials.
2. Use a service account for Bind Principal with read-only permissions.
3. Confirm with your IT/AD team regarding the correct attribute names for mapping.
4. If your organization primarily uses SAML for SSO, LDAP can be avoided.
