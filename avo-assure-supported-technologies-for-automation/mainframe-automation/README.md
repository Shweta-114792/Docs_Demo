# Mainframe Automation

Mainframe Automation in Avo Assure enables you to automate interactions with mainframe applications and terminal-based systems through an action-driven approach. Avo Assure supports Bluezone, Mocha, etc emulators.

{% hint style="info" %}
To learn more about supported Mainframes emulators, refer [Supported Technologies](../../avo-assure-installation-requirements/supported-technologies.md#mainframes)
{% endhint %}

This document includes:

* [Prerequisites](./#prerequisites)
* [Configuring Connection in Mainframe](./#configuring-connection-in-mainframe)
* [Creating Element Repository for Mainframe](creating-element-repository-for-mainframe.md)
* [Creating Test Case for Mainframe](creating-test-case-for-mainframe.md)

## Prerequisites

Following are the requirements for performing mainframe automation:

1. Mainframe emulator must be configured.
2. Connection must be established.
3. Username and password must be handy.

## Configuring Connection in Mainframe

To establish connection in mainframe, perform the following actions:

1. Open the Mainframe application.
2. Select **Session** and select **New Mainframe Display** to create a new connection. The **Define New Connection** dialog opens.

![](<../../.gitbook/assets/unknown (301).png>)

3. In **Connection Name** text box, enter connection name for the mainframe.
4. In **Host Address** text box, enter host address.
5. In **TCP Port** text box, enter TCP port number.
6. Select **Ok**.

![](<../../.gitbook/assets/unknown (302).png>)

7. On the **TN3270E Properties** dialog, select Ok.
8. Note the x and y axis to create elements in Avo Assure.

![](<../../.gitbook/assets/unknown (303).png>)
