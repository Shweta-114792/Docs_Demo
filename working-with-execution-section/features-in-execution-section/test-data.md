# Test Data

The **Test Data** option in the **Execution Configuration** that allows you to specify or overwrite the ADV (Advance) Excel sheet path that holds the test data for parameterization.\
This option takes priority over the ADV excel file path defined in the test step or Testcase. It allows you to update or change the data source without modifying the test design, making it easier to manage the data used for a specific execution.\
When the test runs, Avo Assure uses the ADV Excel file path defined under the **Test Data** section of the **Execution Configuration** instead of the one provided in the test step.

{% hint style="info" %}
**Note**: To learn more about how to organize the Test Data in Excel file, [click here](../../../../actions/generic/loops-and-condition-operations/get-param/adv-parameter.md).
{% endhint %}

Steps to use an ADV Excel file path in Test Data:

1. On the **Execution** tab, navigate to **Configuration** window.
2. Expand the **Test Data** from the Configuration.
3. Enter the ADV Excel file path along with the sheet name, and specify ADV (e.g., C:\Users\Downloads\Sample Data.xlsx;Sheet1;ADV) for the file that contains multiple data sets.
4. Select **Save** to save the configuration.

<figure><img src="../../../../.gitbook/assets/image (4347).png" alt=""><figcaption></figcaption></figure>

5. Execute the Testcase. Avo Assure automatically picks the correct data set from the ADV Excel file during execution.
