# Test Artifacts in Avo Assure

In Avo Assure, test artifacts refer to the various entities used while creating, managing, and executing automation assets. The test artifacts include **Element Repositories**, **Test Cases**, **Execution Lists, Data Tables**, **Reusable Libraries**, and **End-to-End Flows**. Each of these artifacts serves a different purpose in the automation process and supports specific functionalities within the application.

## Understanding Different Statuses of Test Artifacts

The test artifacts move through different states that represent their lifecycle during creation, review, and version control. These states help users easily understand the current stage of an artifact while working with the application.

The available states are:

* New
* In Progress
* Under Review
* Approved
* Rejected
* Checked In/Approved
* Checked In/In Progress
* Checked In/Under Review
* Checked In/Rejected

For example, when a test artifact is created, it starts in the **New** state. After editing begins, the state changes to **In Progress**. When the test artifact is submitted for review, it moves to the **Under Review** state. Based on the reviewer’s decision, the state changes to either **Approved** or **Rejected**. After the test artifact is pushed to Bitbucket, the state updates to **Checked In/Approved**.

## Understanding Status Icons

<table><thead><tr><th width="203.07403564453125">Icon</th><th>Status</th><th>Description</th></tr></thead><tbody><tr><td><img src="../.gitbook/assets/unknown (2).png" alt=""></td><td>New</td><td>This indicates that the test artifact is created and is not edited.</td></tr><tr><td><img src="../.gitbook/assets/In progress 1.png" alt="" data-size="original"></td><td>In Progress</td><td>This indicates the test artifact is in progress.</td></tr><tr><td><img src="../.gitbook/assets/Under review 1.png" alt=""></td><td>Under Review</td><td>This indicates that the test artifact is under review.</td></tr><tr><td><img src="../.gitbook/assets/Thumbs up 1.png" alt=""></td><td>Approved</td><td>This indicates that the test artifact is approved by the reviewer.</td></tr><tr><td><img src="../.gitbook/assets/Thumbs down 1.png" alt=""></td><td>Rejected</td><td>This indicates that the test artifact is rejected by the reviewer.</td></tr><tr><td><img src="../.gitbook/assets/Thumbs up copy 1.png" alt=""></td><td>Checked In/ Approved</td><td>This indicates that the test artifact is approved and pushed to Bitbucket.</td></tr><tr><td><img src="../.gitbook/assets/In progress copy 1.png" alt=""></td><td>Checked In/ In Progress</td><td>This indicates that the test artifact is in progress and pushed to Bitbucket.</td></tr><tr><td><img src="../.gitbook/assets/Under review-1 1.png" alt=""></td><td>Checked In/ Under Review</td><td>This indicates that the test artifact is under review and pushed to Bitbucket.</td></tr><tr><td><img src="../.gitbook/assets/Thumbs down copy 1.png" alt=""></td><td>Checked In/ Rejected</td><td>This indicates that the test artifact is rejected and pushed to Bitbucket.</td></tr></tbody></table>

## Viewing Status Icons in Avo Assure

You can find the test artifacts status icons in the following areas of Avo Assure:

* **Avo Assure Modules**: Element Repository, Test Case, Execution, and Test Data Management

<figure><img src="../.gitbook/assets/unknown (18).png" alt="" width="563"><figcaption></figcaption></figure>

* **Folder Structure**: Element Repository, Test Case, Execution, and Test Data Management

<figure><img src="../.gitbook/assets/unknown (19).png" alt=""><figcaption></figcaption></figure>

* **Element Repository Details**

<figure><img src="../.gitbook/assets/unknown (20).png" alt=""><figcaption></figcaption></figure>

* **Notifications**

<figure><img src="../.gitbook/assets/image (5023).png" alt=""><figcaption></figcaption></figure>

* **Bitbucket Push Page**

<figure><img src="../.gitbook/assets/unknown (22).png" alt=""><figcaption></figcaption></figure>

## Enabling Show Status

The Show status option is available as a toggle. Enabling this toggle displays the status of test artifacts in folder structure, allowing you to quickly understand the current state of a test artifact.

To enable the show status of the Test Artifacts, perform the following actions:

1. On the **Home** page, select **Design Studio**.
2. On the **Element Repository** page, enable **Show Status** toggle. The icons are displayed.

{% hint style="info" %}
**Note**:

* Use this step for all test artifacts, including **Test Case**, **Execution**, and **Test Data Management** modules.
* Icons are not shown for **New** and **In Progress** artifacts.
{% endhint %}

<figure><img src="../.gitbook/assets/unknown (23).png" alt=""><figcaption></figcaption></figure>
