# Account Admin Mapping

Account Admin Mapping in Avo Assure follows the Role-Based Access Control (RBAC) principle, where access is managed through roles rather than individual user assignments.

Account Admin Mapping is a feature within Avo Assure that allows an Account Admin to assign Active Directory (AD) security groups specifically to the Avo Assure Admin role. This is done by clicking on the directory icon next to the role in the Account Admin Mapping section. Once a security group is assigned, all users within that group are automatically granted admin-level access in Avo Assure. This eliminates the need to manually assign roles to individual users and ensures that administrative access is linked directly to directory-based group memberships.

### Roles of Account Admin&#x20;

1. As account admin, user can create Verticals and map security groups to Avo roles&#x20;
2. As account admin, user can create project and map it with verticals&#x20;
3. As account admin, user can add/remove agents from verticals&#x20;

### &#x20;Steps to map AD security group:&#x20;

1. Login to Avo Assure using valid credentials&#x20;
2. Navigate to the Admin section on the left pane of the landing page&#x20;
3. Navigate to Account Admin Mapping window in SSO Management&#x20;
4. Click directory icon&#x20;

<figure><img src="../../../.gitbook/assets/image (358).png" alt=""><figcaption></figcaption></figure>

5. Select Security Group from list and click Add

<figure><img src="../../../.gitbook/assets/image (360).png" alt=""><figcaption></figcaption></figure>

6. Click Save to save the mapping

### **Example:**&#x20;

Consider John is user who belongs to the group **AccountAdmin** as shown in steps above, since group is now mapped as Account Admin, he will be able to&#x20;

* create and map verticals&#x20;
* create and map projects&#x20;
* add and remove agents&#x20;
