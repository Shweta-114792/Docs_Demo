# Through Data Table

Avo Assure have the in-house data table by which user can perform data parametrization by creating table in Test Data Management.

{% hint style="info" %}
**Note:** There was no option to write in data tables. With new enhancement, users can write back to a data table by providing syntax in the input field available in a Test Step under the Test Step Group
{% endhint %}

**Step-by-step process to copy Data Table path for using it in Data parametrization:**

1. Create Data Table

{% hint style="info" %}
**Note**:

* You can add up to 100 columns, and there is no limit on rows in the Data Table.
* For creating Data Table in Avo Assure refer this [Data Table | Avo Assure](../../../../integrations-in-avo-assure/versioning/bitbucket/reviewing-test-artifacts/data-table.md)
{% endhint %}

2. Click **(…)** icon and **Copy datatable path** for using it in test step for data parametrization.

<figure><img src="../../../../.gitbook/assets/image (4872).png" alt=""><figcaption></figcaption></figure>

User need to add three mandatory additional steps to the Test Step Group for performing Data Parameterization of Data Table

1. Navigate to **Test Case** window, select Test Case where data needs to be parametrized
2. Click **+** icon and add new step

<figure><img src="../../../../.gitbook/assets/image (2613).png" alt=""><figcaption></figcaption></figure>

3. Select **@Generic** as element and **Get Param** as action and enter copied **Datatable path** in Input Value

<figure><img src="../../../../.gitbook/assets/image (2621).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Note:** Data Table must be created in same project
{% endhint %}

4. Add new step, select **@Generic** as element and **Start Loop** as action

<figure><img src="../../../../.gitbook/assets/image (2615).png" alt=""><figcaption></figcaption></figure>

5. Add variables in pipe operator in Input Value column to fetch the value from excel sheet

{% hint style="info" %}
**Note:** Variable name should match with Data table Variables
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (2616).png" alt=""><figcaption></figcaption></figure>

6. Add new step where the iteration process should be halted, select **@Generic** as element and **End Loop** as action

{% hint style="info" %}
**Note:** If End Loop is not added then user will get Dangling error while execution
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (2618).png" alt=""><figcaption></figcaption></figure>
