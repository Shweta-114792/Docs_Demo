# Grid Management in Vertical

Use the Grid Management feature in Vertical Management to create, edit, and delete grids for a selected vertical. A grid defines a group of agents and the Avo client count, which you can use to execute tests. This section describes how to create a new grid, update agents in an existing grid, and remove a grid that is no longer required.

## Creating a Grid in Vertical Management

To create a grid, perform the following actions:

1. On the **Home** page, select **Admin**. 
2. In the left navigation pane, select **Vertical management** > **Grid Management**. The **Grids** page opens. 
3. From the **Select a Vertical** dropdown, select the required vertical.

{% hint style="info" %}
To know how to create verticle in RBAC, [click here](vertical-management/vertical-creation.md).
{% endhint %}

4. Select **+ Add New**. The **Create New Grid** dialog box opens.

<figure><img src="../../../.gitbook/assets/image (5005).png" alt=""><figcaption></figcaption></figure>

5. In the **Grid Name** text box, enter the grid name.
6. In the **Agents List** table, select the required agents from the Agent column to include them in the grid.
7. In the **Avo Client Count** column, use the spin box to set the client count.

{% hint style="info" %}
**Note**:

* You can directly enter the client count in the spin box.
* You can select the agent based on its status:
  * **Active**: The agent is ready to execute tests.
  * **Inactive**: The agent is unavailable and cannot execute tests.
* You can create multiple grids by selecting the **+** **Create Grid** button.
{% endhint %}

8. Select **Create** to add the grid. You can use the created grid to execute tests.

<figure><img src="../../../.gitbook/assets/image (5006).png" alt=""><figcaption></figcaption></figure>

## Editing a Grid in Vertical Management

To edit a grid, perform the following actions:

1. On the **Home** page, select **Admin**. 
2. In the left navigation pane, select **Vertical management** > **Grid Management**. The **Grids** page opens. 
3. From the **Select a Vertical** dropdown, select the required vertical. The available grids appear.
4. Hover over the required grid row for which you want to edit. The **Edit** icon appears.
5. Select the **Edit** icon. The **Edit Grid** dialog box appears.

<figure><img src="../../../.gitbook/assets/image (5007).png" alt=""><figcaption></figcaption></figure>

6. In the **Agents List** table, select or clear the required agents.
7. Select **Update**. The Grid updated successfully message appears.

<figure><img src="../../../.gitbook/assets/image (5008).png" alt=""><figcaption></figcaption></figure>

## Deleting a Grid in Vertical Management

To delete a grid, perform the following actions:

1. On the **Home** page, select **Admin**. 
2. In the left navigation pane, select **Vertical management** > **Grid Management**. The **Grids** page opens. 
3. From the **Select a Vertical** dropdown, select the required vertical. The available grids appear.
4. Hover over the required grid row for which you want to delete. The **Delete** icon appears.

<figure><img src="../../../.gitbook/assets/image (5009).png" alt=""><figcaption></figcaption></figure>

5. Select the **Delete** icon. A confirmation message appears.
6. Select **Yes** to delete the grid. The Deleted successfully message appears.
