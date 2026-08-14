# Understanding Avo Assure Roles

In Avo Assure, different roles have different privileges and permissions according to that QM, QL and QE perform their tasks&#x20;

Go through the below screenshot to know the privileges:&#x20;

<figure><img src="../../.gitbook/assets/image (359).png" alt=""><figcaption></figcaption></figure>

### Primary Roles

**There are three primary roles defined within the system, listed here in descending order of hierarchy:**

<table><thead><tr><th width="153">Role </th><th width="323.4000244140625">Description </th><th>Hierarchy Level  (Highest to Lowest) </th></tr></thead><tbody><tr><td><p>Quality Manager </p><p>(QM) </p></td><td><p>Holds the highest authority in the quality </p><p>domain. </p></td><td>1 (Highest) </td></tr><tr><td>Quality Lead (QL) </td><td><p>Mid-level role overseeing quality tasks </p><p>and team members. </p></td><td>2 </td></tr><tr><td><p>Quality Engineer </p><p>(QE) </p></td><td><p>Entry or execution-level role responsible </p><p>for quality engineering activities. </p></td><td>3 (Lowest) </td></tr></tbody></table>

**Additionally, there is one Secondary Role:**

| Role   | Description                                                                             |
| ------ | --------------------------------------------------------------------------------------- |
| Admin  | <p>Support role with administrative </p><p>privileges, separate from quality roles </p> |

### Role Precedence across Multiple Assignments&#x20;

When a security group is linked to a vertical with multiple roles assigned to a single user, the role with the highest precedence will be considered effective.&#x20;

**Example:** If a user is assigned both QM and QE roles within the same vertical, the system will assign the QM role privileges because QM outranks QE.&#x20;

### Admin Role Combination:&#x20;

The **Admin role** can be combined only with the Quality Manager (QM) role at the vertical level.&#x20;

If a security group is mapped to a vertical with both QM and Admin roles, the user will have:&#x20;

**Primary role:** Quality Manager Privileges Additional role: Vertical Admin privileges&#x20;

### Project-Level Roles&#x20;

Project-level roles mirror the same three primary roles: QM, QL, and QE.&#x20;

The key difference from primary roles is that project-level roles are specific to individual projects.&#x20;

A user can have a primary role (instance-level) such as QM across the organization but hold different roles (e.g., QL or QE) for specific projects.&#x20;

Project-level roles define the user's privileges and responsibilities within the context of that particular project, which may differ from their primary role.&#x20;

### **Summary of Role Assignment**&#x20;

<table><thead><tr><th width="123">Role Type </th><th width="119.199951171875">Role Options </th><th width="152">Scope </th><th>Privilege Determination </th></tr></thead><tbody><tr><td>Primary Role </td><td>QM, QL, QE </td><td>User Level </td><td><p>Highest role takes precedence if multiple roles </p><p>assigned </p></td></tr><tr><td>Project Role </td><td>QM, QL, QE </td><td>Project-specific </td><td><p>Role assigned per project defines privileges for that </p><p>project </p></td></tr><tr><td><p>Secondary </p><p>Role </p></td><td>Admin </td><td><p>Account/Vertical </p><p>Level </p></td><td><p>Separate administrative </p><p>privileges </p></td></tr></tbody></table>
