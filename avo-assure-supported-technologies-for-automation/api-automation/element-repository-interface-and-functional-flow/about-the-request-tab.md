# About the Request Tab

The Request tab in the Element Repository enables you to configure and execute API requests. It allows you to specify the HTTP method, endpoint URL, request parameters, and authentication details. This tab serves as the main workspace for building and validating API requests before sending them to the server.

On the **Element Repository** page (Home > Select Project > Design Studio > Element Repository > Request tab), you can do the following:

1. HTTP Method
   * Select the specific HTTP operation for the API endpoint.
   * Supported methods include GET, POST, HEAD, PUT, DELETE, and PATCH.
   * When the HTTP method is selected, Avo Assure automatically formats the request structure.
2. URL
   * This is used to enter the endpoint URL, including host, base path, and resource path.
   * Avo Assure validates whether the URL is reachable when the request is sent.
3. Operation\
   This is used to specify or select the particular operation that should be executed for the configured API request. The behavior of this field varies based on the type of service. Avo Assure supports the following API types:
   * **For SOAP AP**I:
     * Web Services Description Language (WSDL) is an XML based definition that describes the operations, input/output parameters, and endpoints of a SOAP web service. It defines how the service can be called and what data structures are expected and returned.
     * The Operation text box specifies the exact action that the SOAP service should execute. It corresponds to the operation defined in the WSDL and is used to identify which request needs to be triggered on the server.
   * **For REST API**:
     * The Operation text box is not used for REST services. In REST APIs, the request behavior is determined by the HTTP method and endpoint (URL), along with headers and request body, rather than an operation name.
4. Header
   * Use Content-Type headers to inform the server what format your request body uses. Avo Assure supports the following:
     * **Content-Type: application/json**: Use this when you send raw JSON data. Example: When you post user data like `{"name": "John", "id": 123}`.
     * **Content-Type: application/xml** or **Content-Type: text/xml**: Use this when you send raw XML data. Example: When you send SOAP requests or XML payloads like `<user><name>John</name></user>`.
     * **Content-Type: multipart/form-data**: Use this when you upload files or submit forms with mixed content (both text and file attachments). For example: When you upload a document along with user details.
     * **Content-Type: application/x-www-form-urlencoded**: Use this when you send simple form data as encoded key-value pairs. For example: When you send `name=John&id=123` in the body (similar to how data appears in a URL).

{% hint style="info" %}
**Note**: When you select a specific body format (such as JSON, XML, or www-form-urlencoded), Avo Assure automatically adds the corresponding Content-Type in the **Header** tab. You do not need to enter this header manually.
{% endhint %}

5. Body
   * Defines the request payload when the HTTP method supports a body (e.g., POST, PUT and PATCH).
   * Avo Assure supports the following body formats:
     * form-data, x-www-form-urlencoded, and raw (JSON/XML).
   * The defined payload is passed directly to the server, enabling validation of complex request models, authentication payloads, and nested structures.

{% hint style="info" %}
**Note**: For **form-data** body format:

*   When you upload a file and if that file is stored in local client other users cannot use that file during the execution. To allow all users to access the file, configure **Segregated Avo Storage** (**shared storage**).

    Based on the Segregated Avo Storage configuration, the system works as follows:

    * **If Segregated Avo Storage is configured on the Avo server**:\
      The **Upload** option appears. You can upload single or multiple files, and the system saves them in the Segregated Avo Storage location so that all users can access them during debug and execution.
    * **If Segregated Avo Storage is not configured**:\
      You need to provide the local file path directly in the input field and the system saves them in the local Avo client location. To specify single or multiple file paths, separate each path with a semicolon (;). For Example: `c:/user/api`**`;`**`c:/user/downloads/api`
{% endhint %}

6. Params
   * Used for adding Query Parameters or Path Parameters required by the endpoint.
   * **Query Parameters**:
     * These are key-value pairs appended to the endpoint after a question mark (?). They are primarily used to filter or refine the response data.
     * Let us consider an example of `https://api.example.com/users?id=10&status=active` URL. In this case, id=10 and status=active are query parameters that filter the user list based on the specified criteria.
   * **Path Parameters**:
     * This is part of the endpoint URL and are used to identify specific resources. These parameters are placed directly in the path, replacing placeholders defined in the API structure.
     * Let us consider an example of `https://api.example.com/users/10` URL. Here, 10 is a path parameter representing the user ID that uniquely identifies the requested resource.
     * Avo Assure automatically appends these to the URL in the correct format.\
       For example: ?id=10\&status=available.
     * Useful when testing filtered endpoints, search endpoints, or path variable-based REST APIs.
7. Authorization
   * Used to configure authentication for secured APIs directly within Avo Assure.
   * The platform supports the following authentication types:
     * **No Auth**: Used for public or unsecured endpoints.
     * **Basic Auth**: Basic Auth is used to authenticate the user by sending the username and password in an encoded format within the Authorization header. This allows the server to verify the user's identity before processing the API request.
     * **OAuth 2.0**: Allows configuring token based secured endpoints. Tokens generated externally can be used in this authorization for execution.
     * **Bearer Token**: The token is passed in the Authorization header using the format bearer \<token> and does not require manual header creation.
     * **API Key**: Avo Assure allows you to pass authentication details such as an API key or JSON Web Tokens (JWT) through the request header or as a query parameter, depending on the authentication requirements of the target API.
   * Avo Assure automatically manages the authentication headers for each method.
8. Certificate
   * Use this tab because some highly secure APIs (like banking or internal enterprise APIs) require a digital certificate to verify your identity. For these systems, a standard username and password are not enough. They need a digital ID card to trust your connection.
   * Avo Assure needs the following details to locate and use the digital certificate:
     * **Path**: Provide the file path so Avo Assure knows exactly where to find your digital certificate on your computer. Avo Assure attaches this file to your API request to prove your identity to the server.
     * **Password**: Provide the password to unlock the digital certificate securely so that Avo Assure can read the certificate file and include it with your API request.
9. Save
   * Saves the API request configuration in the Element Repository. This option stores the request details so you can reuse the APIs while creating or automating test cases.

{% hint style="info" %}
**Note**: You need to save the request before selecting **Send**. Without saving, you cannot send the API request.
{% endhint %}

10. Send
    * Sends the configured API request to the server and displays the response. Use this option to verify whether the request works correctly before using it in test automation.
11. Append
    * Adds the new configuration details to the existing request configuration during a resend or update. This option helps you to update the request without removing the previously saved settings.

<figure><img src="../../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>
