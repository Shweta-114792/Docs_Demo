# Non-Relational Database

A database that stores data in flexible formats e.g., documents, key-value pairs, or graphs, making it ideal for unstructured or large-scale data. (Examples include MongoDB, Cassandra, and Redis.)

{% hint style="info" %}
**Note:** The example below uses a Non-Relational Database with **MongoDB**. You can follow the same process for other supported databases.
{% endhint %}

## Example

The database contains 21,349 movie entries. From this dataset, movies belonging to the genres Animation, Comedy and Family will be filtered. The cast details of the first two filtered entries will then be validated using dynamic variables storing the values Walt Disney and Clarence Nash. After successful validation, the complete filtered dataset is exported to an Excel sheet.

### The following actions are used in this example.

* Get Data (DB)
* Export Data (DB)

### Test Step Group1: Filter Movies by Genre

**Step1**: The **Get Data (DB)** action fetches the query result using the input value of Get Data action and stores the resulting data into a variable called **{DB\_Data}**.

<figure><img src="../../.gitbook/assets/image (134).png" alt=""><figcaption></figcaption></figure>

### Test Step Group2: Verify Cast Names in First Two Entries

**Step1**: **Create Dynamic Variable** action creates Dynamic variable named **{movie1}** which will contain cast data as **Walt Density** for verification with filter first two entries.

**Step2**: **Create Dynamic Variable** action creates dynamic variable named **{movie2}** which will contain cast data as **Clarence Nash** for verification with filter first two entries.

**Step3**: The **Display Variable Value** action displays the value located at the first row and third column of the **{DB\_Data}** (from 1<sup>st</sup> Test Step Group) matrix using **{DB\_Data\[1]\[3]}**. &#x20;

**Step4**: The **Display Variable Value** action displays the value located at the second row and third column of the **{DB\_Data}** (from 1<sup>st</sup> Test Step Group) matrix using **{DB\_Data\[2]\[3]}**. &#x20;

**Step 5**: The **Compare Value** action will compare the data retrieved from **{DB\_Data\[1]\[3]}** with the dynamically created data that will be stored in **{movie1}**, and result will store it in output variable **{Status1}**.

**Step 6**: The **Compare Value** action will compare the data retrieved from **{DB\_Data\[2]\[3]}** with the dynamically created data that will be stored in **{movie2}**, and result will store it in output variable **{Status2}**.

**Step 7:** The **Display Variable Value** action will display the status of the comparison result, stored in the output variable **{Status1}**, which will contain either **true** (if both value match) or **false** (if both values do not match).

**Step 8**: The **Display Variable Value** action will display the status of the comparison result, stored in the output variable **{Status2}**, which will contain either **true** (if both value match) or **false** (if both values do not match).

<figure><img src="../../.gitbook/assets/image (135).png" alt=""><figcaption></figcaption></figure>

### Test Step Group3: Export Filtered Data

**Step 1**: **Create File** action helps to create file in system, the user needs to provide the file path where the Excel file should be created on the system.   \
**Step 2**: The **Export Data (DB)** action exports the filtered database result into an Excel file, and the output is written to the Excel file path defined in the previous step.&#x20;
