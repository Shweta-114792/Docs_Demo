# LDAP Configuration

The Lightweight Directory Access Protocol (LDAP) allows your organization to connect Avo Assure with your corporate Active Directory (AD) or LDAP server. This enables centralized user authentication that is secure, consistent, and easy to manage.

Integrating Avo Assure with your organization’s Active Directory (AD) or LDAP, users can log in using their corporate credentials. This removes the need for separate Avo Assure accounts and makes login easier.

Onboarding and offboarding users in Avo Assure is easier because any changes made in the directory are automatically applied, allowing users to be granted or removed access promptly.

## Key Features and Benefits&#x20;

Here are the key advantages of using LDAP in Avo Assure:

* **Single Login with Corporate Credentials** \
  Users can log in to Avo Assure using their existing organization's username and password, so they don’t need separate accounts.&#x20;
* **Centralized User Management** \
  Administrators can manage users, groups, and access permissions directly from the corporate directory, which automatically applies in Avo Assure.&#x20;
* **Enhanced Security** \
  Passwords are not stored in Avo Assure. Authentication happens directly via the LDAP server ensuring corporate security policies are enforced.&#x20;
* **Simplified Onboarding and Offboarding** \
  When a user is added or removed from the directory, their Avo Assure access is updated automatically reducing manual work and error.&#x20;
* **Audit and Compliance Support** \
  Authentication events are logged through the LDAP/Active Directory, helping track access for audits and compliance.&#x20;

## Terminologies

* **LDAP (Lightweight Directory Access Protocol)**: Standard protocol for accessing and authenticating directory services such as Active Directory or OpenLDAP.&#x20;
* **AD (Active Directory)**: The system where your organization stores user accounts, groups, and permissions. Avo Assure uses it to verify user identities.&#x20;
* **TLS (Transport Layer Security) Certification**: A secure LDAP (LDAPS) connection typically requires an SSL/TLS certificate to encrypt communication. If you want LDAP over TLS, a valid and trusted certificate is mandatory to ensure secure and verified connectivity.&#x20;
* **DN (Distinguished Name)**: The full path to an object in the directory. Example: \
  CN=ldap-user,OU=ServiceAccounts,DC=example,DC=com.&#x20;
* **CN (Common Name)**: The name of an object (e.g., a user, group, or device).&#x20;
* **OU (Organizational Unit)**: A logical container or folder within the directory that groups objects.&#x20;
* **DC (Domain Component)**: Part of the domain name. For example, DC=example,DC=com = example.com.&#x20;
* **Bind Principal**: The service account that Avo Assure uses to connect and query the LDAP directory.&#x20;
* **Bind Credentials**: The password for the Bind Principal account.&#x20;

## This Document Includes:

[Prerequisites](prerequisites.md)

Prerequisites for configuring LDAP in Avo Assure.

[Creating LDAP Configuration in Avo Assure](creating-ldap-configuration-in-avo-assure.md)

Description of LDAP configuration feilds and steps to perform LDAP Configuration.
