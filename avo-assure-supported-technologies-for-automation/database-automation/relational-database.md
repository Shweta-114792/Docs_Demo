# Relational Database

A database that stores data in structured tables (rows and columns) with fixed schema, where relationships between data are managed using keys. (Examples include MySQL, PostgreSQL, and Oracle.)

{% hint style="info" %}
**Note:** DB Numbers or DB tags are required in test steps for Avo Assure to recognize the database type.
{% endhint %}

{% hint style="info" %}
**Note:** The example below uses a relational database with **PostgreSQL.** You can follow the same process for other supported databases.
{% endhint %}

## Example

In this example, the Test Case connects to a PostgreSQL database and filters the film table to find all movies with a rating of 'G' and a rental rate of 2.99. It counts the number of matching records and displays the total movie. After that, the filtered data is exported to an Excel file. Finally, the test validates that the exported data matches what's in the database.

### The following actions are used in this example.

* Run Query (DB)
* Get Data (DB)
* Export Data (DB)
* Verify Data (DB)

<figure><img src="../../.gitbook/assets/image (129).png" alt=""><figcaption></figcaption></figure>

### Test Step Group 1: Filter Data by Rating and Rental Rate

**Step 1:** A database query is executed using the Run Query (DB) action. This query retrieves the records from the films table where the film rating and rental rate matches specified values.

<figure><img src="../../.gitbook/assets/image (130).png" alt=""><figcaption></figcaption></figure>

### Test Step Group 2: Count Filtered entries

**Step 1:** The **Get Data (DB)** action fetches the query result using the same input value (ep-lively-glitter-a83wuaj6) and stores the resulting table data into a variable called **{DB\_Data}**.

**Step 2:** The **Display Variable Value** action displays the value located at the first row and first column of the **{DB\_Data}** matrix using **{DB\_Data\[1]\[1]}**.<br>

{% hint style="info" %}
**Note:**

* If the user is using the {DB-Data} variable, it only stores the status as True or False.
* If the user is using the {DB\_Data\[1]\[1]} variable, it retrieves the value at the specified array index.
{% endhint %}

**Step 3:** **Create** **Dynamic Variable action** creates **{Row Count}** to store the number of rows in the fetched data from **{DB\_Data\[1]\[1]}**.

**Step 4:** **Display Variable Value** action shows the value of **{Row Count}** to confirm how many records were retrieved from database.

<figure><img src="../../.gitbook/assets/image (131).png" alt=""><figcaption></figcaption></figure>

### Test Step Group 3: Validate Filtered Entries

**Step 1:** When using the **Create File** action, specify the file path where the system must create the Excel file.

**Step 2:** The **Export Data (DB)** action exports the filtered database result into an Excel file, and the output is exported to the Excel file path defined in the previous step.

**Step 3:** The **Verify Data (DB)** action verifies the data exported to Excel with the results retrieved from the database. This ensures that the contents of the exported file accurately reflect the filtered data from the database.

**Step 4:** The **Display Variable Value** action shows the value of the **{Status}** variable, which indicates whether the validation passed (true or false).

<figure><img src="../../.gitbook/assets/image (132).png" alt=""><figcaption></figcaption></figure>
