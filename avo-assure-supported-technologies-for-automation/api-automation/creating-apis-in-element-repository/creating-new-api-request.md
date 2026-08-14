# Creating New API Request

You can create and send API request using the following options:

* [**Direct API Request**](creating-new-api-request.md#sending-a-direct-api-request)
* [**Advanced API Request**](creating-new-api-request.md#sending-an-advanced-api-request)

## Sending Direct API Request

This article covers about sending direct API request when the API does not require complex configurations. It allows you to quickly send a request using only the basic details such as the endpoint URL and HTTP method. This option is useful for simple API calls where no additional authentication, parameters, or certificates are required.

To send a direct API request, perform the following actions:&#x20;

1. On the **Home** page, under **Projects**, select the required **Project**.
2. Select **Design Studio**. In the **Element Repository** page, locate the **Create Folder (+)** icon.&#x20;
3. Select **Create Folder** (**+**) icon and select **Create new folder** to create a new folder for element repository. A new folder is created. &#x20;
4. In the **New Folder** text box, enter the element repository folder name. &#x20;
5. In the newly created folder, select Ellipsis (**...**) icon > **Create Repository** > **APIs** to create the repository.&#x20;

<figure><img src="../../../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

6. From the **Select** dropdown, choose the required HTTP method:&#x20;
   * **GET**: Used to retrieve information or data from the specified resource.&#x20;
   * **POST**: Used to submit data to the server to create a new resource.&#x20;
   * **HEAD**: Used to request response headers only without the response body.&#x20;
   * **PUT**: Used to update or replace an existing resource with new data.&#x20;
   * **DELETE**: Used to remove the specified resource from the server.&#x20;
   * **PATCH**: Used to apply partial updates or modifications to an existing resource.
7. In the **Enter URL** text box, enter the API endpoint URL.&#x20;
8. In the **Operation** text box, enter the mathematical operation.&#x20;

{% hint style="info" %}
**Note**:&#x20;

* The **Operation** text box is used only when performing API testing for SOAP based APIs.&#x20;
* As per the requirements, you can specify the value as **Add**, **Subtract**, **Multiply**, or **Divide** in the **Operation** text box.&#x20;
* When you are performing API testing for REST based services, then the **Operation** text box is not applicable.&#x20;
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4965).png" alt=""><figcaption></figcaption></figure>

9. Select the **Header** tab and then enter the API Header details.

{% hint style="info" %}
**Note**: When you select a specific body format (such as JSON, XML, or form-data), Avo Assure automatically adds the corresponding **Content-Type** in the **Header** tab. You do not need to enter this header manually.
{% endhint %}

10. Select the **Body** tab and then enter the API Body details.\
    Here are the different types of body format:

<details>

<summary><strong>none</strong></summary>

The **none** is used when the API request does not require any data in the request body.

To use the **none** body format, perform the following actions:

1. In the **Body** tab, select the **none** option.

{% hint style="info" %}
**Note**: Use this body format when the request does not require a payload.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4) (1).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>form-data</strong></summary>

The **form-data** is used to send data to the server as key–value pairs. It works like a digital form where each field has a name (Key) and the corresponding information (Value). This method allows you to send both text data and files (such as images or documents) in the same request, making it useful for APIs that require file uploads along with other data.

You can send the data in two ways:

* **Key-Value Edit**
* **Bulk Edit**

{% hint style="info" %}
**Note**:&#x20;

* You can customize your table using the following table options:
  * **Manage Columns**: Select the vertical ellipsis (**⋮**) icon to show or hide specific columns, such as **Value**, and **Description**.
  * **Delete Rows**:
    * To delete a row, hover over it and select the **Delete row** icon that appears.
    * Select the checkbox, and the **Delete** button appears. Select **Delete** to remove the row.&#x20;
    * You can also select multiple checkboxes to delete multiple rows at the same time.
{% endhint %}

### **Sending Key-Values**&#x20;

**Key-Value Edit** allows you to define individual parameters for text and files. Following are the two ways to send the key values:

* **Text**&#x20;
* **File**

#### **Sending Key-Values Using Text**

To send **text** data using the **form-data** body format, perform the following actions:

1. On the **Request** tab, select **Body**.&#x20;
2. Select **form-data**.
3. In the **Key** column, enter the key name.
4. Select the parameter type as **Text** from dropdown.

{% hint style="info" %}
**Note**: You can only select the parameter type (Text or File) after you add the Key name.
{% endhint %}

5. In the **Value** column, enter the required key value.
6. Enter the description in **Description** column. (Optional)

{% hint style="info" %}
**Note**: You can add multiple rows to include more than one text parameter in the same request.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

#### Sending Key-Values Using File

To upload a **file** using the **form-data** body format, perform the following actions:

1. In the **Request** page, select the **Body** tab.&#x20;
2. Select **form-data**.

<figure><img src="../../../.gitbook/assets/image (4960).png" alt=""><figcaption></figcaption></figure>

3. In the **Key** column, enter the key name.
4. Select the parameter type as **File** from dropdown.
5. Enter the file path or upload the file in the **Value** column.

{% hint style="info" %}
**Note**: To know more about uploading files in Segregated Avo Storage location, [click here](../element-repository-interface-and-functional-flow/about-the-request-tab.md).
{% endhint %}

6. Enter the description in **Description** column. (Optional)

<figure><img src="../../../.gitbook/assets/image (4973).png" alt=""><figcaption></figcaption></figure>

### **Sending in Bulk**

To enter values in **Bulk Edit** mode, perform the following actions:

1. In the **Request** tab, select **Body**.&#x20;
2. Select **form-data.**
3. Select **Bulk Edit** next to the **Description** column.&#x20;

<figure><img src="../../../.gitbook/assets/image (4971).png" alt=""><figcaption></figcaption></figure>

4. Enter the **key name** and its **value** in the request body. &#x20;

{% hint style="info" %}
**Note**: If you enter the request data in **Bulk Edit** mode and then switch to **Key-Value Edit** mode, the system automatically displays the same data in the selected format. You do not need to enter the data again. The same applies when switching from **Key-Value Edit** mode to **Bulk Edit** mode.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4972).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>x-www-form-urlencoded</strong></summary>

The **x-www-form-urlencoded** is used to send data to the server as key–value pairs. It works like submitting a simple web form where each field has a name (Key) and the corresponding data (Value). This format is typically used when the API needs to receive structured text data but does not require file uploads.

To use the **x-www-form-urlencoded** body format, perform the following actions:

1. On the **Request** tab, select **Body**.&#x20;
2. Select **x-www-form-urlencoded**.
3. In the **Key** column, enter the key name.
4. In the **Value** column, enter the key value.

{% hint style="info" %}
**Note**:&#x20;

* You can use this format to send simple text data only. Avo Assure automatically encodes the key-value pairs into a single string before sending the request.
* You can customize your workspace using the following table options:
  * **Manage Columns**: Select the vertical ellipsis (**⋮**) icon to show or hide specific columns, such as **Value**, and **Description**.
  * **Delete Rows**:
    * To delete a row, hover over it and select the **Delete row** icon that appears.
    * Select the checkbox, and the **Delete** button appears. Select **Delete** to remove the row.&#x20;
    * You can also select multiple checkboxes to delete multiple rows at the same time
* To change the display format, refer the steps given in [form-data](creating-new-api-request.md#form-data).
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (18) (1).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>raw - JSON or XML</strong></summary>

The **raw** (**JSON** or **XML**) is used to send structured data in a specific format such as JSON or XML. In this method, you provide the entire request body in the selected format. It is commonly used when an API expects well-structured data to create, update, or process information on the server.

### Sending JSON Body Request

To use the **raw - JSON** body format, perform the following actions:

1. On the **Request** tab, select **Body**.&#x20;
2. Select the **raw** option.
3. Select **JSON** from the dropdown next to **raw**.
4. In the text editor area, enter or paste your JSON payload.

<figure><img src="../../../.gitbook/assets/image (9) (2).png" alt=""><figcaption></figcaption></figure>

### Sending XML Body Request

To use the **raw - XML** body format, perform the following actions:

1. On the **Request** tab, select **Body**.&#x20;
2. Select the **raw** option.
3. Select **XML** from the dropdown next to **raw**.
4. In the text editor area, enter or paste your XML payload.

</details>

11. Select the **Save** button to store the configuration.&#x20;

{% hint style="info" %}
The saved element can be used while creating API Test cases.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (4968).png" alt=""><figcaption></figcaption></figure>

12. Select the **Send** button to execute the API request.

{% hint style="info" %}
**Note**:&#x20;

* After you save the request, the **Send** button becomes enabled.
* After executing the API request, you can go to the **Response** tab to view the result. To learn more, [click here](../element-repository-interface-and-functional-flow/about-the-response-tab.md).&#x20;
{% endhint %}

13. Select the **Append** checkbox to overwrite the existing configuration with the new configuration details during a resend or update.

{% hint style="info" %}
**Note**: If existing request details are not overwritten during a resend or update, the previous configuration remains unchanged.&#x20;
{% endhint %}

## Sending Advanced API Request

This article covers about advanced API request, when an API requires additional configurations before sending the request. These configurations may include parameters, authentication details, headers, or security certificates. This option allows you to define and manage these settings to ensure the request meets the APIs security and validation requirements.

To send an advanced API request, perform the following actions:&#x20;

1. Follow Steps 1 through 10 from the **Sending a Direct API Request** section to set up the basic request.
2. Select the **Params** tab and enter the parameter and its value as required.
3. Select the **Authorization** tab and select the required authorization from the **TYPE** dropdown. Here are the different types of Authorization:

<details>

<summary><strong>No Auth</strong></summary>

To configure **No Auth** authorization, perform the following action:

1. In the **TYPE** dropdown, select the **No Auth** option. 

{% hint style="info" %}
**Note**: When the API does not require authentication, then you can use the **No Auth** option.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>Basic Auth</strong></summary>

To configure **Basic Auth** authorization, perform the following actions: &#x20;

1. In the **TYPE** dropdown, select the **Basic Auth** option. &#x20;
2. In the **Username** text box, enter the **Username**. &#x20;
3. In the **Password** text box, enter the **Password**. 

<figure><img src="../../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>OAuth2.0</strong></summary>

To configure **OAuth2.0** authorization, perform the following actions:

1. In the **TYPE** dropdown, select the **OAuth2.0** option. &#x20;
2. In the **URL** text box, enter the URL. &#x20;
3. In the **Client ID** text box, enter the client id. &#x20;
4. In the **Client Secret** text box, enter the client secret. &#x20;
5. In the **Scope** text box, enter the scope. &#x20;
6. In the **Grant** **Type** text box, enter the grant type. &#x20;
7. Select the **Generate** **Token** button to generate the token. 

<figure><img src="../../../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>Bearer Auth</strong></summary>

To configure **Bearer Auth** authorization, perform the following actions: &#x20;

1. In the **TYPE** dropdown, select the **Bearer Auth** option. &#x20;
2. In the **Bearer** text box, enter the bearer token.

<figure><img src="../../../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>Api Key</strong></summary>

To configure **Api Key** authorization, perform the following actions: &#x20;

1. In the **TYPE** dropdown, select the Api Key option. &#x20;
2. In the **Key** text box, enter the key. 
3. In the **Value** text box, enter the value.

{% hint style="info" %}
**Note:** When you provide the token, add the prefix **JWT** before the token and include a space between **JWT** and the token.
{% endhint %}

4. From the **Add To** option, select **Header** or **Params** from the dropdown.

<figure><img src="../../../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>

</details>

4. Select the **Certificate** tab and do the following: &#x20;
   * In the **Path** text box, enter the certificate path and certificate key (optional). &#x20;
   * In the **Password** text box, enter the certificate password. &#x20;
   * Select **Submit** button to finalize the API request setup.

{% hint style="info" %}
**Note**: If you want to change or update the configured data, you can select the **Reset** button. 
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

5. Select the **Save** button to store the configuration.&#x20;
6. Select the **Send** button to execute the API request.
7. Select the **Append** checkbox to overwrite the existing configuration with the new configuration details during a resend or update.
