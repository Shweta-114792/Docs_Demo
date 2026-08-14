# Execution through Client/Agent/Grid

## Executing Test Cases through Client

To execute the execution through client, perform the following actions:

1. On the **Home** page, select required project and select **Design Studio**.
2. Select the **Execution** tab.
3. Expand Folder and select **Execution List** for configurations.
4. From **Configurations** page, select **Client**.
5. From **Client** dropdown, select active client.

{% hint style="info" %}
**Note**:&#x20;

* A single instance does not support running multiple clients on the same machine at the same time. This gives an error as **Array** **variable has incorrect number of subscripts or subscript dimension range exceeded**_._
* The **Configurations** page displays all configured clients, along with their respective status indicators for easy identification.
  * A **green** indicator indicates that the client is **Available**.&#x20;
  * A **yellow** indicator indicates that the client is **Unavailable**.
  * A **red** indicator indicates that the client is **Do Not Disturb**.&#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4307).png" alt=""><figcaption></figcaption></figure>

6. From **Browsers** dropdown and select **Browser**.
7. Select **Save** to save all the changes.
8. Select parent folder and select **Execute**. The **Execution Now** dialog opens.
9. Select **Execute** to execute the **Execution List**.

## Executing Test Cases through Agent/Grid

To execute the execution through agent, perform the following actions:

1. On the **Home** page, select required project and select **Design Studio**.
2. Select the **Execution** tab.
3. Expand Folder and select **Execution List**.
4. Select **Configurations**.
5. Select **Agents**. The agent dialog opens.

<figure><img src="../../../.gitbook/assets/image (4989).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Note**:

* A single instance does not support running multiple agents on the same machine at the same time. This given an error as **Array** **variable has incorrect number of subscripts or subscript dimension range exceeded**_._
* The **Configurations** page displays all configured agents, along with their respective status indicators for easy identification.
  * A **green** indicator indicates that the agent is **Active**.&#x20;
  * A **gray** indicator indicates that the agent is **Inactive**.&#x20;
* To learn how to Install Avo Assure **Agent**, refer to [Agent](../../../administration/authentication-configuration/agent-management/).
* To learn how to create Avo Assure **Grid**, refer to [Grid](../../../administration/authentication-configuration/grid-management/).
{% endhint %}

5. In the **ICE count** column, use the spin box to update the client count.
6. Select **Save**.
7. From **Browsers** dropdown, select **Browser**.
8. Select **Save** to save all the changes.
9. Select parent folder and select **Execute**. The **Execution Now** dialog opens.

<figure><img src="../../../.gitbook/assets/image (102).png" alt="" width="563"><figcaption></figcaption></figure>

5. Select **Execute** to execute the Execution List.

{% hint style="info" %}
**Note**: After configuring the settings while creating the Execution List, you can validate and modify them in the **Execute Now** window.
{% endhint %}
