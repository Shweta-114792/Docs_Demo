# Vertical Mapping

Mapping Vertical indicates adding Security Groups (users) against Avo Assure roles in vertical&#x20;

{% hint style="info" %}
**Note:** When user is not mapped with any vertical, they won’t be able to login through SSO&#x20;
{% endhint %}

**Security Groups**&#x20;

In Avo Assure, Security Groups are used to manage user access control and permissions efficiently across projects, modules, and folders. They help ensure that users can only access the parts of the system they are authorized to, based on their role and responsibility.&#x20;

{% hint style="info" %}
**Note:** These roles will be considered primary roles, while project-based roles may vary depending on project requirements.&#x20;
{% endhint %}

### Steps to Map Vertical with Security group&#x20;

1. Navigate to Verticals window in Vertical Management section&#x20;
2. Hover mouse in empty column to get the Map button&#x20;
3. Click Map button to bring up Vertical Mapping window&#x20;

<figure><img src="../../../../.gitbook/assets/image (369).png" alt=""><figcaption></figcaption></figure>

4. Click Directory icon to get the list of Security Groups

<figure><img src="../../../../.gitbook/assets/image (370).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Note:** Adding Security Group to Admin and Quality Manager role is mandatory&#x20;
{% endhint %}

5. Select Security Group and click Add button&#x20;

<figure><img src="../../../../.gitbook/assets/image (371).png" alt=""><figcaption></figcaption></figure>

6. Click Update button located in bottom right corner to save the mapping

<figure><img src="../../../../.gitbook/assets/image (372).png" alt=""><figcaption></figcaption></figure>

### Example:

1. Consider Jack, a user who belongs to the AvoAdmin group as shown in the steps above. Since this group is now assigned the Vertical Admin role, he will become the vertical admin with access limited to that specific vertical, where he can perform the following actions

* manage assigned verticals
* create and map projects
* add and remove agents

2. In the above steps, the AvoManagers security group is assigned the Quality Manager role in Avo Assure, so all users within that group will have the Quality Manager role and its privileges when they log in.<br>
