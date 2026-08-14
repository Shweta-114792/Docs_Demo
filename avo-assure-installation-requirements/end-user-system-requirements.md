# End-User System Requirements

Avo Assure requires a system environment that supports stable performance, secure network communication, and compatibility with its automation capabilities. It includes supported operating systems, hardware requirements, storage recommendations, network and firewall configurations, browser driver requirements, and execution security prerequisites. Use this information to prepare your environment and verify compatibility before installation and execution of Avo Assure.

## Supported Operating Systems

<table data-header-hidden><thead><tr><th valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top"><strong>Platform</strong></td><td valign="top"><strong>Supported Versions</strong></td></tr><tr><td valign="top">Windows Desktop</td><td valign="top">Windows 10 or later</td></tr><tr><td valign="top">Windows Server</td><td valign="top">Windows Server 2016 or later</td></tr><tr><td valign="top">macOS</td><td valign="top">macOS 13 Ventura or later</td></tr></tbody></table>

### Key Notes

* Avo Assure supports Apple Silicon devices.
* Windows 7, Windows 8, and Windows 8.1 are not supported.
* On macOS:
  * Only Web application automation is supported.
  * Desktop application automation and Agent execution is not supported.

## Minimum Hardware Requirements

The following table lists the minimum and recommended hardware requirements for each Avo Client or Virtual Machine (VM):

<table data-header-hidden><thead><tr><th valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top"><strong>Component</strong></td><td valign="top"><strong>Requirement</strong></td></tr><tr><td valign="top">Operating System</td><td valign="top">Windows 10, Windows Server 2016, or later versions. macOS 13 or later</td></tr><tr><td valign="top">Minimum RAM</td><td valign="top">8 GB</td></tr><tr><td valign="top">Recommended RAM</td><td valign="top">16 GB</td></tr><tr><td valign="top">Avo Client Runtime Allocation</td><td valign="top">Minimum 2 GB available memory for Avo Client processes</td></tr><tr><td valign="top">Free Disk Space</td><td valign="top">Minimum 2 GB excluding screenshots</td></tr><tr><td valign="top">Minimum CPU Cores (Single/Parallel Execution)</td><td valign="top">2 vCPU</td></tr><tr><td valign="top">Recommended CPU (Parallel Execution)</td><td valign="top">4 vCPU</td></tr><tr><td valign="top">Minimum Download Speed</td><td valign="top">10 Mbps</td></tr><tr><td valign="top">Minimum Upload Speed</td><td valign="top">10 Mbps</td></tr><tr><td valign="top">Recommended Latency</td><td valign="top">Less than 100 ms</td></tr></tbody></table>

## Virtual Machines and Virtual Desktop Infrastructure Requirements

In shared Virtual Machines (VMs), Virtual Desktop Infrastructure (VDI), Citrix, or Remote Desktop Services (RDS) environments, multiple users can run execution sessions simultaneously. Allocate sufficient RAM and CPU resources to support the combined workload of all active user sessions.

* Minimum system requirements apply to each active Avo execution session and are not shared across concurrent sessions.
* Allocate 8 GB RAM minimum for each active execution session.
* Allocate 16 GB RAM for optimal execution performance.
* Reserve the dedicated 2 GB Avo Client allocation for each concurrent execution session.
* Use dedicated execution VMs for better execution stability and performance.
* Additional resource requirements depend on the following factors:
  * Number of Concurrent Users
  * Parallel Executions
  * Browser Instances/Tabs
  * Application Complexity
  * Screenshot/Video capture usage
  * Background Processes

## Storage Requirements

### Local Machine Storage

Each client machine must have a minimum of 2 GB free disk space excluding screenshots.

The storage requirement includes the following components:

* Execution Logs
* Browser Drivers
* Runtime Artifacts
* Temporary Files
* Application Cache
* Execution Dependencies

### Shared or Centralized Storage

You can store screenshots and execution artifacts in either of the following locations:

* Avo-managed Storage (recommended)
* Customer-managed Shared Storage

#### Key Notes

* If you use customer-managed shared storage, allocate a minimum of 50 GB shared storage initially.
* Storage usage increases proportionally with execution volume, screenshot retention, and data retention policies.
* Shared storage locations must be accessible from all execution machines when centralized storage is configured.

## Execution Permissions & Security Requirements

Security tools such as antivirus software, Endpoint Detection and Response (EDR), application control tools, or execution policy frameworks must allow execution of the following:

<table data-header-hidden><thead><tr><th valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top"><strong>File</strong></td><td valign="top"><strong>Purpose</strong></td></tr><tr><td valign="top">Avoagent.exe</td><td valign="top">Agent Execution</td></tr><tr><td valign="top">Run.bat</td><td valign="top">Execution Launcher</td></tr><tr><td valign="top">Python.exe</td><td valign="top">Runtime Dependency</td></tr><tr><td valign="top">Powershell.exe</td><td valign="top">Script Execution</td></tr><tr><td valign="top">Avoassure.ps1</td><td valign="top">PowerShell Automation</td></tr></tbody></table>

## Certificate-Based Distribution

Configure certificate-based whitelisting for AminHoldings to prevent execution blocks during installation, client updates, agent updates, and runtime operations.

Ensure that the certificate trust chain is available across the following environments:

* VDI environments
* Shared VMs
* Endpoint Protection Platforms
* Application Control Policies
* Enterprise Software Deployment Tools

## Network & Firewall Requirements

Avo Assure modules require secure network connectivity to communicate with cloud and system components. Ensure that your IT team configures the necessary allowlist rules for the following URLs:

<table><thead><tr><th valign="top">URL</th><th valign="top">Purpose</th></tr></thead><tbody><tr><td valign="top">https://&#x3C;instancename>.avoassure.ai/</td><td valign="top">Application Access</td></tr><tr><td valign="top">https://avoirisprodapi.avoassure.ai</td><td valign="top">API Communication</td></tr><tr><td valign="top">https://downloads.avoassure.ai/driver</td><td valign="top">Browser Driver Downloads</td></tr><tr><td valign="top">https://&#x3C;instancename>.avoassure.ai/getAgentTask</td><td valign="top">Agent Task Retrieval</td></tr></tbody></table>

## Browser Driver Requirements

All execution systems must have permission to download, store, and execute browser drivers from the following location: https://downloads.avoassure.ai/driver

### Key Notes

Avo Assure updates browser drivers periodically to maintain browser compatibility.

## Supported Browser Drivers

<table data-header-hidden><thead><tr><th valign="top"></th><th valign="top"></th></tr></thead><tbody><tr><td valign="top"><strong>Driver</strong></td><td valign="top"><strong>Browser</strong></td></tr><tr><td valign="top">Chromedriver.exe</td><td valign="top">Google Chrome</td></tr><tr><td valign="top">msedgedriver.exe</td><td valign="top">Microsoft Edge</td></tr></tbody></table>

### Key Notes

Ensure drivers are not blocked by security policies.

## Preparing for Installation

You must complete the preparatory steps to ensure the Avo Assure Client is installed correctly and is ready for use. Here are the preparatory steps:

1. **Whitelist Instance URL**: Request your IT administrator to add the Avo Assure instance URL to the network allowlist.
2. **Enable .exe downloads**: Ensure your IT team allows or enables downloading of .exe files so the Client installer can be downloaded and installed.
3. **Validate Installation Setup**\
   Perform the following actions to validate the installation setup:
   1. Log in to the application.
   2. Create a new project.
   3. [Capture elements](../create-and-execute-tests-with-design-studio/working-with-element-repository-section/create-element-repository/capturing-elements-in-avo-assure/).
   4. Run Test cases through the [Execution List](../create-and-execute-tests-with-design-studio/working-with-execution-section/creating-execution-list/).

**Note**: If you are finding WebDriver version mismatch issues for Google Chrome, here is the Troubleshooting Guide:

{% file src="../.gitbook/assets/Troubleshooting Steps for Chrome Driver Update Issue.pdf" %}
