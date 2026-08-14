# Working with Avo Assure

## Automating VA01 (Sales Order Creation) in SAP using Avo Assure&#x20;

The VA01 transaction in SAP is used to create a new Sales Order. This is one of the most common and critical processes in the SAP Sales & Distribution (SD) module. \
In Avo Assure, we can automate this flow using pre-built SAP actions, reusable repositories, and structured process flows.&#x20;

### SAP Steps in VA01 flow&#x20;

The business process involves:&#x20;

1. **Login:** Authenticate into the SAP system.
2. **Create Sales Order (VA01):** Start the VA01 transaction, enter the order type and organizational details, and provide customer and order information such as Sold-to Party, Ship-to Party, Material, Quantity, and Plant.
3. **Validate Sales Document:** Verify pricing, mandatory fields, and product availability. Once validated, save the order and capture the generated Sales Order Number.
4. **Logout:** Exit the SAP session.

### Implementing VA01 flow in Avo Assure&#x20;

In Avo Assure, the process flow is broken into Test Step Groups inside a Test Case:&#x20;

#### Test Step Group 1 – Login&#x20;

* **Action**: Launch Application.
* **Inputs**: SAP Server, Client, User ID, Password.
* **Validation**: Verify login screen navigation.

<figure><img src="../../.gitbook/assets/image (4372).png" alt=""><figcaption></figcaption></figure>

#### Test Step Group 2 – Create Sales Order (VA01)&#x20;

* **Action**: Start Transaction&#x20;
* **Input**: VA01&#x20;
* **Next**: Select Order Type (OR – Standard Order)&#x20;
* **Actions Used**: Dropdown → Select Value by Text, Set Text (for Org/Division fields)&#x20;
* **Action**: Set Text → Enter Sold-to Party&#x20;
* **Action**: Set Text → Enter Ship-to Party&#x20;
* **Action**: Set Text → Enter Material Code&#x20;
* **Action**: Set Text → Enter Quantity&#x20;
* **Action**: Set Text → Enter Plant&#x20;
* **Validation**: Verify mandatory fields are not empty&#x20;

<figure><img src="../../.gitbook/assets/image (4373).png" alt=""><figcaption></figcaption></figure>

#### Test Step Group 3 – Validate Sales Document&#x20;

* **Action**: Verify Text (for pricing condition fields)&#x20;
* **Action**: Get Status Bar Message → Validate system messages&#x20;
* **Validation**: Ensure no errors are displayed&#x20;
* **Action**: Press Tool Bar Button → Save&#x20;
* **Action**: Get Status Bar Message → Capture Sales Order number&#x20;
* **Output**: Store Sales Order ID in a Dynamic Variable {SO\_Number} for reporting/reuse&#x20;

<figure><img src="../../.gitbook/assets/image (4374).png" alt=""><figcaption></figcaption></figure>

#### Test Step Group 4 – Logout&#x20;

* **Action**: @Sap → End Transaction / Logoff&#x20;
* **Validation**: Verify SAP GUI closes successfully

<figure><img src="../../.gitbook/assets/image (4375).png" alt=""><figcaption></figcaption></figure>

### Avo Assure Features Used in VA01 Automation&#x20;

* **Element Repository**: Create a repository with SAP option selected, store VA01 screen elements (buttons, text fields, dropdowns).&#x20;
* **Reusable Step Groups**: Login and Logout flows can be reused across other SAP test cases.&#x20;
* **Dynamic Variables**: Sales Order Number captured during Save step can be used for downstream test cases (e.g., Invoice creation).&#x20;
* **SAP Actions Library**: Utilized SAP-specific prebuilt actions (Start Transaction, Set Text, Dropdown Select, Get Status Bar, Tool Bar Action).&#x20;
* **Reporting**: Execution results, including captured Sales Order Number, are logged in Unified Reports and Web Reports.&#x20;

#### Example Process Flow in Avo Assure&#x20;

| Test Step Group    | Step                           | Action                      | Input / Expected Result                     |
| ------------------ | ------------------------------ | --------------------------- | ------------------------------------------- |
| Login              | Launch Application             | @Sap → Launch               | User credentials, SAP server                |
| Start Transaction  | Start VA01                     | @Sap → Start Transaction    | VA01, Order Type = OR, Sales Org = 1000     |
| Enter Details      | Fill Customer & Order Info     | Set Text, Dropdown Select   | Sold-to = 1000, Material = MAT01, Qty = 10  |
| Validate Document  | Check Pricing & Messages       | Verify Text, Get StatusBar  | Pricing complete, No error messages         |
| Save Order         | Save and Capture Order Number  | Tool Bar Action → Save      | Output {SO\_Number} captured                |
| Logout             | End SAP Session                | @Sap → Logoff               | Application closed                          |

### Benefits of Automating VA01 Flow&#x20;

* Ensures consistent validation of Sales Order creation.&#x20;
* Reduces manual effort in repetitive order entry tests.&#x20;
* Captures dynamic data (Order Number) for end-to-end testing.&#x20;
* Enhances reusability (Login/Logout groups reused in other flows like ME21N Purchase Order, VF01 Billing).&#x20;

### Conclusion&#x20;

The VA01 Sales Order Creation flow is a fundamental process in SAP SD. Automating it with Avo Assure provides:&#x20;

* Reliability&#x20;
* Faster test execution&#x20;
* End-to-end coverage (integration with downstream processes)&#x20;

By leveraging process flows, element repository, and SAP actions, Avo Assure makes SAP automation structured, reusable, and business aligned.&#x20;

{% hint style="info" %}
**Note**: Verification and Validation can be scripted according to your requirements.
{% endhint %}
