# Prerequisites

Before configuring LDAP in Avo Assure Admin, ensure the following requirements are fulfilled:

1. **LDAP/Active Directory Server Details**&#x20;
   * Hostname or IP address of the LDAP server.&#x20;
   * Port number (default LDAP: 389, LDAPS: 636).&#x20;
   * Base Distinguished Name (Base DN) for user searches.&#x20;
2. **Service Account (Bind Principal)**&#x20;
   * A dedicated account in the directory for Avo Assure to query users.&#x20;
   * Preferably read-only permissions.&#x20;
   * Bind account credentials (username and password) if using Simple Authentication.&#x20;
3. **TLS Certificate (if using secure LDAPS connection)**&#x20;
   * Certificate issued by your organization’s Certificate Authority (CA).&#x20;
   * Ensure encrypted communication between Avo Assure and the LDAP server.&#x20;
4. **Network Access**&#x20;
   * The Avo Assure server must reach the LDAP server through the correctly configured port to ensure proper connectivity.
   * Firewall rules should allow LDAP/LDAPS traffic.&#x20;
5. **User Attribute Mapping Information**&#x20;
   * LDAP attribute names for Username, First Name, Last Name, and Email.&#x20;
   * Confirm with your IT/AD team to ensure correct mapping.&#x20;
6. **Administrator Access in Avo Assure**&#x20;
   * You need Admin privileges in Avo Assure to configure LDAP settings.&#x20;
