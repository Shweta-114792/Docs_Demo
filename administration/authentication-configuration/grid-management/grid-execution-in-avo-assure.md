# Grid Execution in Avo Assure

Grid execution allows you to run multiple test cases parallelly across different agents and clients. This parallel execution reduces the total time required to complete an execution list.

To start a Grid execution, follow these steps:

1. On the **Execution** page, select the created **Execution List**.
2. From the right pane, select the **Configuration** tab.
3. Select the **Agent** option and select the created grid from the dropdown. The grid popup opens.

{% hint style="info" %}
**Note**:

* In the created grid popup, you can also update the client count and select **Save** after making the changes.
* The updated client count is reflected on the **Grids** page (Location: **Admin** > **Grids**).
* You can add up to 10 clients under one agent.
{% endhint %}

4. Select browser from **Browsers** dropdown.
5. Select **Save** to save the configuration.

<figure><img src="../../../.gitbook/assets/image (4988).png" alt=""><figcaption></figcaption></figure>

6. Go to the folder and select the **Execute** button. The **Execute Now** window opens.

{% hint style="info" %}
**Note**: You can also override the configuration details from the **Execute Now** popup.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (2) (1).png" alt=""><figcaption></figcaption></figure>

7. Select the **Execute** button to start the execution.

<figure><img src="../../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

### How Grid Execution Works

Each agent supports a specific number of clients. A client is a functional unit that executes one test case at a time.

#### Flow Diagram

<figure><img src="../../../.gitbook/assets/image (3370).png" alt="" width="563"><figcaption></figcaption></figure>

### Example

In this example, let’s understand how Grid Execution works in Avo Assure:

Let’s say you have **9 test cases** that need to be executed. These are part of your **Execution List** in Avo Assure.

To run these test cases, you have created a Grid setup with the following configuration:

* **Agent 1** has **2 clients**
* **Agent 2** has **3 clients**
* **Agent 3** has **1 client**
* **Agent 4** has **2 clients**

{% hint style="info" %}
**Note:** Only one agent can be installed on a system at a time.
{% endhint %}

That means you have a total of **8 clients** available across all agents. Each client can execute **one test case at a time**.

#### Execution Process

When you start the execution, Avo Assure distributes the test cases across all available clients.

1. **Initial Distribution**: The system assigns the first eight test cases to the available clients:
   * **Test Case 1** - Agent 1, Client 1
   * **Test Case 2** - Agent 1, Client 2
   * **Test Case 3** - Agent 2, Client 1
   * **Test Case 4** - Agent 2, Client 2
   * **Test Case 5** - Agent 2, Client 3
   * **Test Case 6** - Agent 3, Client 1
   * **Test Case 7** - Agent 4, Client 1
   * **Test Case 8** - Agent 4, Client 2
2. **Queuing**: Because all eight clients are busy, **Test Case 9** enters a queue.
3. **As soon as you start the execution**:
   * **Test Case 1** goes to Agent 1 – Client 1
   * **Test Case 2** goes to Agent 1 – Client 2
   * **Test Case 3** goes to Agent 2 – Client 1
   * **Test Case 4** goes to Agent 2 – Client 2
   * **Test Case 5** goes to Agent 2 – Client 3
   * **Test Case 6** goes to Agent 3 – Client 1
   * **Test Case 7** goes to Agent 4 – Client 1
   * **Test Case 8** goes to Agent 4 – Client 2
4. Now all 8 clients are busy, so **Test Case 9** goes into a **queue**.
5. **Dynamic Assignment**: As soon as any client finishes its test case and becomes free, it automatically picks up **Test Case 9** from the queue to complete the execution.
