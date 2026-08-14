# Integration Configuration

In the **Execution Configuration** window, two options are available — **Test Management Tool** and **Bug Tracking Tool**. These options help you integrate your automation setup with external tools. By using these integrations, you can manage test cases, track bugs, and sync execution results directly from the platform for better visibility and control.

## Test Management Tool

Steps to Configure Test Management Tool:

1. On the **Execution** tab, navigate to the **Configuration** window.
2. Expand the **Test Management Tool** and select **Zephyr/Xray/Zephyr Scale** to connect with the desired test management tool. The **Configuration** pop-up appears.
3. Enter the required integration details based on the selected tool:
   * **Zephyr:** Enter the tool URL, access credentials, and API key token.
   * **Xray:** Select Avo Assure Project and Xray Test Plan.
   * **Zephyr Scale:** Select Zephyr Scale Project.
4. Select **Save** to apply the integration settings.

<figure><img src="../../../.gitbook/assets/image (4340).png" alt=""><figcaption></figcaption></figure>

## Bug Tracking Tool

Steps to configure Bug Tracking Tool:

1. On the **Execution** tab, navigate to the **Configuration** window.
2. Expand the **Bug Tracking Tool** and select **Jira** to connect your automation environment with the bug tracking tool.
3. Turn on the **Auto Defect Creation** toggle. It automatically logs defects in **Jira** whenever a test step fails during execution. (optional)

{% hint style="info" %}
**Note:** You can also log a defect manually in Jira instead of using Auto Defect Creation.
{% endhint %}

4. Select **Save** to apply the integration settings.

<figure><img src="../../../.gitbook/assets/image (4341).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
To learn more about Integrations, refer to [Integration in Avo Assure](../../../integrations-in-avo-assure/).
{% endhint %}
