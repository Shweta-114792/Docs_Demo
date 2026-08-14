# Executing Test Case with Avo Agent

To execute test cases on the grid, perform the following steps:

1. Navigate to the **Execution** tab.
2. Add the required test cases to the **Execution List**.
3. Select **Execute**.
4. In the **Execute** dialog, select the **Grid** option under **Execute On**.
5. Select the required agent from the **Agent** dropdown.

{% hint style="info" %}
**Note**: The status indicator next to the agent's name identifies the current status.&#x20;

* A **green** indicator indicates that the agent is **Active.**
* A **gray** indicator indicates that the agent is **Inactive**.
{% endhint %}

6. Select the required browser from the **Browsers** dropdown.
7. Select **Execute** to start the execution.

<figure><img src="../../../.gitbook/assets/image (3330).png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="info" %}
**Note**:

Execution through an Agent does not support keyboard-related actions such as, **Send Function Keys** and **Send Keystroke Values**.

The number of agents and clients that can be configured depends on the system capacity. Systems with higher capacity support more agents and clients efficiently.
{% endhint %}

### Flow Diagram

<figure><img src="../../../.gitbook/assets/image (3369).png" alt=""><figcaption></figcaption></figure>

### In this example, let’s understand how Agent Execution works in Avo Assure:

Let’s say you have **9 test cases** that need to be executed. These are part of your **Execution List** in Avo Assure.

To run these test cases, you’re using a **single system** where **one agent** is installed and configured with **3 clients**.

{% hint style="info" %}
**Note:** Only one agent can be installed on a system at a time.
{% endhint %}

Test cases are **distributed across 3 available clients**, which execute them in parallel. The remaining test cases will be placed in a queue and executed as clients become available.

#### **Execution Process:**

As soon as you start the execution:

* **Test Case 1** is picked by **Client 1**
* **Test Case 2** is picked by **Client 2**
* **Test Case 3** is picked by **Client 3**

Now, all 3 clients are busy executing their assigned test cases.

The remaining test cases (from **Test Case 4** to **Test Case 9**) remain in the queue.

As soon as any client finishes its current execution, it becomes available and **automatically picks up the next test case** from the queue. For example:

* When Client 1 completes Test Case 1, it picks up **Test Case 4**
* When Client 2 completes Test Case 2, it picks up **Test Case 5**, and so on

This cycle continues until all 9 test cases are executed.
