# Importing APIs Definition

This article explains how to import APIs definitions can be imported from local files or URLs into the Element Repository to automatically create APIs and streamline API configuration.

You can import APIs into the Element Repository using following options:

* [**Plus (+) icon**](importing-apis-definition.md#importing-api-definition-using-create-folder--icon)
* [**Ellipsis (...) icon**](importing-apis-definition.md#importing-api-definition-using-ellipsis-...-icon)

## Importing APIs Definition using Plus icon

To Import APIs Definition in Element Repository using **Plus** (**+**) icon, perform the following actions:

1. On the **Home** page, under **Projects**, select the required **Project**.
2. Select **Design Studio.**
3. Select the **Element Repository** page
4. Select the Plus (**+**) icon.
5. Select **Import APIs Definition**. The Import APIs Definition dialog opens.

<figure><img src="../../../.gitbook/assets/image (31).png" alt="" width="335"><figcaption></figcaption></figure>

6. You can import API definition using the following options:

* **File**
* **URL**

<details>

<summary><strong>File</strong></summary>

To import an API definition using **File** option, perform the following actions:

1. In the **Import APIs Definition** dialog box, select the **Upload JSON File** button.

<figure><img src="../../../.gitbook/assets/image (43).png" alt="" width="304"><figcaption></figcaption></figure>

2. Select the appropriate **JSON File** from your local system.
3. Select the **Import API** to import the selected JSON File.
4. After the API definition is imported, it appears in the **Element Repository** page.

</details>

<details>

<summary><strong>URL</strong></summary>

To import an API definition using **URL** option, perform the following actions:

1. In the **Source label** text box, enter the API endpoint URL.
2. From the **Protocol** dropdown, select the required protocol.

{% hint style="info" %}
**Note**:

* When using SOAP APIs, make sure to enter **?WSDL** at the end of URL entered in **Source label** text box which automatically selects prototype as WSDL.\
  For example: https://ecs.syr.edu/faculty/fawcett/code/calcWebService/Calc.asmx?WSDL
* When using REST APIs, **Swagger** protocol must be selected.
{% endhint %}

3. Select **Import API** button to import API Definition.

<figure><img src="../../../.gitbook/assets/image (44).png" alt="" width="290"><figcaption></figcaption></figure>

4. After the API definition is imported, it appears in the **Element Repository** page.

</details>

8. Select the **send** button to execute the imported API definition.

{% hint style="info" %}
After executing the API request, you can go to [**Response**](../viewing-response-details.md) tab to view the result.
{% endhint %}

9. Select the **save** button to store the configuration.

## Importing APIs Definition using Ellipsis (...) Icon

To Import API Definition in Element Repository by selecting **ellipsis (...)** icon, perform the following actions:

1. In **Element Repository** page, select the parent folder in which you want to import the API definition.
2. Select the **ellipsis (...)** icon corresponding to that folder.
3. From the menu options, select **Import Definition**. The **Import API Definition** dialog box appears.

<figure><img src="../../../.gitbook/assets/image (45).png" alt="" width="511"><figcaption></figcaption></figure>

4. You can import API definition using the following options:
   * **File**
   * **URL**

<details>

<summary><strong>File</strong></summary>

To import an API definition using **File** option, perform the following actions:

1. In the **Import API Definition** dialog box, select the **Upload JSON File** button.
2. Select the appropriate **JSON File** from your local system.
3. Select the **Import API** to import the selected JSON File.
4. After the API definition is imported, it appears in the **Element Repository** page.

</details>

<details>

<summary><strong>URL</strong></summary>

To import an API definition using **URL** option, perform the following actions:

1. In the **Source label** text box, enter the API endpoint URL.
2. From the **Protocol** dropdown, select the required protocol.
3. Select **Import API** button to import API Definition.

{% hint style="info" %}
**Note**:

* When using SOAP service, make sure to enter **?WSDL** at the end of URL entered in **Source label** text box which automatically selects prototype as WSDL.\
  For example: https://ecs.syr.edu/faculty/fawcett/code/calcWebService/Calc.asmx?WSDL
* When using Rest service, **Swagger** protocol must be selected.
{% endhint %}

4. After the API definition is imported, it appears in the **Element Repository** page.

</details>

5. Select the **send** button to execute the imported API definition.

{% hint style="info" %}
After executing the API request, you can go to [**Response**](../viewing-response-details.md) tab to view the result.
{% endhint %}

6. Select the **save** button to store the configuration as a APIs element.
