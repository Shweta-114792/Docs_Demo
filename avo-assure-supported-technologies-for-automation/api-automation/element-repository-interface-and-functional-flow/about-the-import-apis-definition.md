# About the Import APIs Definition

The Import APIs Definition feature allows you to automatically generate multiple APIs in the Element Repository from a provided API specification. Instead of manually configuring each request, Avo Assure analyzes the imported definition and creates the corresponding endpoints, significantly reducing setup time and ensuring consistency across large API collections.&#x20;

This capability is particularly useful when working with services that expose multiple endpoints such as REST or SOAP based systems where rapid, bulk creation of APIs helps to accelerate API automation and testing.

You can import an APIs definition using the following options:&#x20;

* **File**: Import APIs definition file directly from the local system. Only JSON file format is supported.
* **URL**: Import the APIs definition from a hosted location by specifying the definition URL.&#x20;

## About the File Option

On the **Element Repository** page (Home > Select Project > Design Studio > Element Repository > Select Create Folder icon/Parent Folder (Ellipsis icon) > Import APIs Definition > File), you can do the following:&#x20;

1. Import API Definition using File Option
   * Allows you to upload a local Swagger or OpenAPI - Version 2.x / 3.x JSON definition file from their system.&#x20;
   * After the API definition file is uploaded, Avo Assure parses the file and automatically creates API elements in the repository based on the endpoints defined in the specification.&#x20;
   * This eliminates the need to configure each request manually and ensures the imported structure matches the original API contract.

<figure><img src="../../../.gitbook/assets/image (32).png" alt="" width="305"><figcaption></figcaption></figure>

## About the URL Option

You can use the URL option to import an API definition directly from a hosted link.&#x20;

On the **Element Repository** page (Home > Select Project > Design Studio > Element Repository > Select Create Folder icon/Parent Folder (Ellipsis icon) > Import APIs Definition > URL), you can do the following:&#x20;

1. Import API Definition using URL Option
   * Allows you to upload a local Swagger or OpenAPI - Version 2.x / 3.x JSON definition file from their system.&#x20;
   * This method enables you to fetch the API specification using the definition URL provided in the **Source Label** text box.&#x20;
   * The Protocol dropdown identifies the service type, which can be automatically defined or manually selected as **WSDL** for SOAP APIs or **Swagger** for REST APIs.&#x20;
   * After the definition URL and protocol are configured, Avo Assure retrieves the API specification from the specified source and automatically generates the API elements in the Element Repository.

<figure><img src="../../../.gitbook/assets/image (33).png" alt="" width="293"><figcaption></figcaption></figure>
