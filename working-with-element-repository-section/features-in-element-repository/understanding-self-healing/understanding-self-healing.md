# Understanding Self Healing

Avo Assure's next-generation Self Heal uses AI-based heuristic matching to capture contextual fingerprints and understand the UI during test execution and intelligently identify elements on the screen. Unlike traditional approaches that depend on locator-based identification captured during script creation, it can seamlessly adapt to many UI changes without requiring updates to the test script.

This advanced self healing capability goes beyond simply switching to alternative element properties or locator strategies. By leveraging the contextual fingerprints of UI elements, it helps recover from UI changes more effectively, reducing test maintenance effort, improving automation stability, and enabling faster release cycles.

### Prerequisites (For scripts built before Avo Assure v26.4.2)

Following are the prerequisites to perform self healing:

* For existing elements, test cases must consistently pass.
* For each element, at least one locator (preferably P1) should accurately identify the correct element.

### Scope

* Currently, it works only via Execution lists (not in debug) and runs in the background with no UI changes in Avo Assure.
* Only Web applications are supported.

### Self Healing Recovery Scenarios Inclusions

Following UI changes are handled when self heal is enabled:

* Element ID
* Name attribute
* Class name
* CSS selector
* in XPath
* Relative XPath
* Layout
* Element relocation within a page
* Iframe and nested Iframe elements

{% hint style="info" %}
**Note:** Any scenario outside this scope is not supported currently.
{% endhint %}
