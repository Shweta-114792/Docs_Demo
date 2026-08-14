# Overview

This feature supports multi-domain operations for users in an instance in Avo Assure and and restricts cross-domain component visibility and access. 

### Key Components in Vertical Management: &#x20;

1. **Security Groups:**  \
   Users are segregated into security groups, which act as the primary unit for access control. It helps manage user access and permissions across projects, modules, and folders.&#x20;
2. **Vertical Segregation:**  \
   Each security group is tied to only one vertical (domain).  \
   Security groups cannot overlap across verticals, ensuring complete separation between domains. &#x20;
3. **User Roles & Permissions:**  \
   Users within security groups are assigned roles such as: 

* Admin &#x20;
* Quality Manager &#x20;
* Quality Lead &#x20;
* Quality Engineer &#x20;

Each role has clearly defined access privileges, tailored to their responsibilities. 

### Key Entities - Functionality and Usage: &#x20;

<details>

<summary> <strong>Projects</strong></summary>

* Acts as the main container for all automation-related features
* Contains test cases, configurations, reports, and linked resources &#x20;
* Ensures access to a project is tightly controlled via RBAC policies

</details>

<details>

<summary>Users </summary>

* Are placed in Security Groups, each of which is mapped to a single vertical (domain) with no cross-vertical overlap allowed
* Users are assigned specific roles within the group: &#x20;

<table><thead><tr><th width="152.60003662109375">Role </th><th>Description </th></tr></thead><tbody><tr><td>Admin  </td><td>Full access including user, agent, and project management  </td></tr><tr><td>Quality Manager  </td><td>Manages project-level activities and reporting  </td></tr><tr><td>Quality Lead  </td><td>Oversees execution and quality checkpoints  </td></tr><tr><td>Quality Engineer  </td><td>Executes test cases, limited configuration rights  </td></tr></tbody></table>

</details>

<details>

<summary>Agents </summary>

* Are execution units assigned to individual users
* Support parallel and distributed execution of test cases
* Are controlled per user, aligned with their access and vertical assignment

</details>

## Understanding the Hierarchical Levels in Avo Assure :&#x20;

Avo Assure follows a **3-tier** to effectively manage automation assets like **Users**, **Projects**, and **Agents.** These tiers provide **granular control** over access and configurations, ensuring scalability, security, and flexibility across organizations. 

### Account Level Admin – The Super Admin &#x20;

1. **Top-most authority** in the Avo Assure hierarchy. &#x20;
2. Has **full visibility and control** over _all Verticals, Projects, Users, and Agents_. &#x20;
3. Can **create and manage Verticals** — which are logical groupings representing departments, business units, or teams. &#x20;
4. Responsible for **SSO integration**:  \
   a. Maps **SSO Organizational Units** (OU) with Verticals. \
   b. Links **SSO Security Groups** to specific **Avo Assure roles.**&#x20;

 **Key capabilities:** &#x20;

1. View and manage all Verticals. &#x20;
2. Create new Verticals. &#x20;
3. Edit existing ones. &#x20;
4. Delegate control to Vertical-level admins. &#x20;

### 2. Vertical Level Admin – Departmental/Unit Admin &#x20;

1. Manages a **specific Vertical** (a subset of the entire account). &#x20;
2. Can access and control **Projects, Users,** and **Agents** only within their own Vertical. &#x20;
3. Lacks access to view or manage resources outside their assigned Vertical. &#x20;
4. Users, Projects, and Agents **created within a Vertical are shared across all projects** of that Vertical. &#x20;
5. Also participates in **SSO setup at the vertical level:** &#x20;
6. Associates the Vertical with a specific SSO OU. &#x20;
7. Maps Avo Assure roles to SSO Security Groups within the Vertical.  &#x20;

**Key capabilities:** &#x20;

1. View and manage their assigned Vertical. &#x20;
2. Edit existing Vertical settings. &#x20;
3. Assign users and agents to projects within the Vertical.&#x20;

### Project Level Admin – Project-Specific Manager &#x20;

1. Manages one or more individual Projects within a Vertical. &#x20;
2. Only has access to Users and Agents that are specifically associated with the Project. &#x20;
3. Can control access for: &#x20;
4. AD Users (based on their group and mapped role). &#x20;
5. Non-AD Users (added manually by the admin). &#x20;
6. Cannot manage or modify the Vertical itself. &#x20;
7. Cannot assign users across Verticals. &#x20;
8. It has a limited scope but is sufficient for day-to-day project-level activities. &#x20;

**Key Concept Summary** &#x20;

| Level                     | Scope of Access                                                | Can Manage Verticals?      | Can Manage SSO Mapping?   | Resources Accessible                          |
| ------------------------- | -------------------------------------------------------------- | -------------------------- | ------------------------- | --------------------------------------------- |
| **Account Level Admin**   | Entire platform – all Verticals, Projects, Users, and Agents   |  Yes                       | Yes                       | All Verticals, Projects, Users, Agents        |
| **Vertical Level Admin**  | Single Vertical only – projects and assets within              |  No (only view/edit own)   | Yes (own vertical only)   | Projects, Users, Agents within the Vertical   |
| **Project Level**         | One or more specific Projects                                  | No                         |  No                       | Only Users and Agents added to the Project    |
