# Custom Property

### Overview&#x20;

Avo Assure supports automation for web applications by using built-in properties to identify on-screen elements. In addition to the eight default properties (e.g., Id, Attribute Name, Class Attribute), two extra fields- Custom 1 and Custom 2 are available for added flexibility. &#x20;

These fields are useful when the application uses unique attributes (e.g., data-testid, maxlength) that are not part of the standard set, enabling more reliable element identification even when default properties vary.&#x20;

{% hint style="warning" %}
_**Note:** Custom 1 and Custom 2 only work for **web applications.**_&#x20;
{% endhint %}

### Custom 1 – Standard Unique Identifier Property&#x20;

**Custom 1** allows users to define a **unique element property** that is consistently used across the application. This is particularly useful when developers implement a unique attribute (e.g., data-testid, custom-id, etc.) throughout the application to help with element identification.&#x20;

* This custom property acts as a replacement or extension of the default properties.&#x20;
* It ensures that the automation scripts remain robust and maintainable by relying on a developer-defined, consistent element identifier.&#x20;

### Custom 2 – Manual Unique Identifier&#x20;

**Custom 2** gives users the **flexibility to manually assign** a unique or alternate identifier for an element.

* This can be helpful in scenarios where the standard properties and _Custom 1_ do not provide sufficient identification.
* Users can input any attribute or identifier that reliably distinguishes the element in the current context.

**Manual Attribute Update Syntax**

When updating a custom attribute manually in the **Custom Property** settings page, please use the following syntax format:

`tagname[attributename="attributevalue"]`
