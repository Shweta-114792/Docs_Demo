# Through Excel Sheet

User need to add three mandatory steps to the Test Step Group for performing Data Parameterization

1. Navigate to **Test Case** window, select Test Case where data needs to be parametrized
2. Click **+** icon and add new step

<figure><img src="../../../../.gitbook/assets/image (2613).png" alt=""><figcaption></figcaption></figure>

3. Select **@Generic** as element and **Get Param** as action and enter **Excel path** in Input Value

Syntax for Excel file: `<Excel file path>;<Sheet Name>`

<figure><img src="../../../../.gitbook/assets/image (2614).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
**Note:** Excel sheet must be in unrestricted folder
{% endhint %}

4. Add new step, select **@Generic** as element and **Start Loop** as action

<figure><img src="../../../../.gitbook/assets/image (2615).png" alt=""><figcaption></figcaption></figure>

5. Add variables in pipe operator in Input Value column to fetch the value from excel sheet

{% hint style="warning" %}
**Note:** Variable name should match with Excel sheet Variables
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (2616).png" alt=""><figcaption></figcaption></figure>

6. Add new step where the iteration process should be halted, select **@Generic** as element and **End Loop** as action

{% hint style="warning" %}
**Note:** If End Loop is not added then user will get Dangling error while execution
{% endhint %}

<figure><img src="../../../../.gitbook/assets/image (2618).png" alt=""><figcaption></figcaption></figure>
