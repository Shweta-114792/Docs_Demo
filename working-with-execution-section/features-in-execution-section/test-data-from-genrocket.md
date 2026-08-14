# Test data from GenRocket

The **Refresh Test Data from GenRocket** feature in the Execution Configuration window allows you to use fresh test data for every execution. You can specify the number of records to be fetched from Data table, ensuring that each run uses new data from your Test Data.

This helps keep your automated tests up-to-date and avoids reusing old test data.

{% hint style="info" %}
To learn more about GenRocket, [click here](../../../../integrations-in-avo-assure/test-data-management/genrocket.md).
{% endhint %}

Steps to use Test Data from Execution Configuration:

1. On the **Execution** page, navigate to the **Configuration** window.
2. Expand the **Test data from GenRocket** section, enable the **Refresh test data generation from GenRocket** toggle to refresh the test data for every execution. &#x20;
3. Enter the count in **Number of Records** to specify how many rows of test data to use during the execution.

{% hint style="info" %}
**Note**:&#x20;

* By default, the **Number of records** is set to 1.
* Always use the Testcase in the **Execution List** that contains GenRocket test data.
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (4350).png" alt=""><figcaption></figcaption></figure>
