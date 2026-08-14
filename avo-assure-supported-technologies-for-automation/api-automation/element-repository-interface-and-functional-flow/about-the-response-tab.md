# About the Response Tab

The Response tab in the Element Repository displays the server’s response to the executed API request. It is used for validating responses, troubleshooting failures, and analyzing returned data during API testing.&#x20;

On the **Element Repository** page (Home > Select Project > Design Studio > Element Repository > Response tab), you can do the following:&#x20;

1. Body:  This tab shows the response message returned by the server. The content is displayed in JSON/XML, form-data and x-www-form-urlencoded format depending on the server returns.
2. Header:
   * This tab lists all response headers received from the API, such as server details, content type, and cache information.
   * The tab also provides additional execution details such as:
     * The HTTP status code received from the server. This helps to determine whether the request was successful (e.g., 200, 201) or resulted in errors such as client errors (400, 401, 404) or server errors (500, 503).
     * The response time.
     * The result of the request indicating whether it passed or failed.

<figure><img src="../../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>
