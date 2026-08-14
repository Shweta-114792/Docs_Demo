---
hidden: true
---

# Copy of Viewing Response Details

The APIs response helps you view and verify the results of a APIs request. An API response includes the response body, headers, and HTTP status code. You can check details such as the returned data, response time, and status to ensure the request executes correctly.

* **Response Header**: Displays response headers such as status code, content type, and other metadata.
* **Response Body**: Shows the main content of the API response in all body formats (form-data, x-www-form-urlencoded and raw (JSON or XML)).

## Viewing Response in Element Repository

To view and validate the APIs response, perform the following actions:

1. On the **Element Repository** page, after sending an APIs request, select the **Response** tab.
2. On the **Response** tab, you can validate an APIs response using the following tabs:

<details>

<summary><strong>Response Header</strong></summary>

The **Header** tab displays the **HTTP status code**, **Server**, **response time**, **Content-Type**, and **Length**.

<figure><img src="../../.gitbook/assets/unknown (87).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary><strong>Response Body</strong></summary>

The **Body** tab displays the response returned by the server. The content is displayed in JSON, XML, or raw format depending on the server returns.

<figure><img src="../../.gitbook/assets/unknown (86).png" alt=""><figcaption></figcaption></figure>

</details>

## Viewing Response in Test Case

To view and validate the APIs response, perform the following actions:

1. On the **Test Case** page, send the APIs request.
2. Select the **Add Step Manually** (**+**) button. The new step created.
3. Add the required validation steps by using the following actions:
   * **Get Body**: Retrieves the response body from the executed Web Service request.
   * **Get Header**: Retrieves the header value by using the header key.
   * **Get Key Value**: Retrieves a specific key value from the JSON response body.
   * **Get Tag Value**: Retrieves a specific tag value from the XML response body.

{% hint style="info" %}
**Note:** To add APIs test steps, refer to[ Creating APIs Test Case.](creating-apis-test-case.md#adding-elements-manually)
{% endhint %}
