# Agent Management

The Avo Agent is a collection of multiple Avo Clients that acts as a bridge between the system and clients which helps in parallel and distributed execution.&#x20;

Agent execution refers to running multiple test cases across different browsers, devices, or environments. This allows test cases to execute reducing overall execution time and improving test efficiency.&#x20;

In Avo Assure, execution is achieved by distributing test cases across multiple clients with the help of an Avo Agent, enabling flexible and efficient parallel/distributed test execution.&#x20;

## **Prerequisites**

Before proceeding with parallel and distributed execution, ensure the following are in place:

1. **Avo Agent Installation**: Avo Agent should be installed either from the Landing Page or the Admin tab.
2. **Client Configuration**: The required number of clients should be initialized within the Avo Agent.
3. **Agent Status**: The Agent should be in an Active state for execution to begin.
4. **Independent Test Cases**: Ensure that all test cases are designed to run independently. Test cases should not depend on the outcome or data of other test cases.

{% hint style="info" %}
**Note:** If the test cases are dependent on different application type, use **End-to-End** (**E2E**) and then use **Agent** for execution.
{% endhint %}

### This Document Includes

[**Install And Configure Avo Agent**](install-and-configure-agent.md)\
The steps to install and configure Avo Agent

[**Manage Agent**](manage-agent.md)\
The steps to edit agent count and delete Avo Agent

[**Work with Avo Agent**](executing-test-case-with-avo-agent.md)\
The steps to work with Avo Agent.
