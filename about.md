# HCL Accelerate
## Overview
<img align="right" src="https://www.hcltechsw.com/wps/wcm/connect/306fda5a-0485-4593-876b-d8f4a221b9cf/unprecendented%2Bvisibility%2Binto%2Byour%2Bvalue%2Bstream.jpg?MOD=AJPERES&CACHEID=ROOTWORKSPACE-306fda5a-0485-4593-876b-d8f4a221b9cf-nWaUQ84" style="width:50%;"/>**Bring unity to your DevOps strategy with HCL Accelerate**, a Value Stream Management platform that brings DevOps data together once-and-for-all. Accelerate helps organizations get the most out of their DevOps investments by optimizing delivery pipeline flow, increasing throughput, identifying bottlenecks, and unifying data from across your organization so that teams can make intelligent business decisions based on data.

**Capabilities include**:

- DevOps Analytics: Transformation leaders can realize the value of hidden continuous delivery data by making it visible and actionable.
- Pipeline Aggregation: Development teams with complex, multi-service applications can orchestrate their continuous delivery pipelines in a single view.
- Release Management: Release teams can move to more frequent releases with lightweight, self-service tools including templates and automated controls.
- Value Stream Visualization: Delivery teams can go beyond traditional Agile views to provide real-time transparency from concept to production.
- Strategic Decision Making: Executives get a complete picture of the DevOps organization, and can identify the top-performing teams to harvest best practices.

<details><summary><strong>SECTION 1: Preparing for HCL Accelerate Demo</strong></summary>
  <br />
  <details><summary><strong>Deploying HCL Accelerate to a SoFy sandbox</strong></summary>
In order to experience HCL Accelerate by completing the demo scenarios documented below, a working instance of HCL Software's value stream management solution must be running and seeded with data in a SoFy sandbox.

Steps to deploying and launching HCL Accelerate

Locate the HCL Accelerate product card in the SoFy catalog and click "Add to Solution".
Enter a solution name and click "Create".

HINT: Solution names must be lower case alphanumeric and cannot contain any special characters.

ADDITIONAL INFO: Creating a SoFy solution will result in a custom helm chart being created for the purposes of bootstrapping the HCL Accelerate deployment in a kubernetes environment.

Click "Deploy" to create the HCL Accelerate demo environment in a SoFy sandbox.

Very quickly, SoFy will deploy HCL Accelerate to HCL's Google Cloud sandbox environment.

When the deployment has completed, click on "View Solution Console" and authenticate with the credentials provided.
In the Solution Content section of the Solution Console view, locate the HCL Accelerate card and click on "General Information".
Click on the "Open Link" button to launch HCL Accelerate in a new browser tab.

CELEBRATE: Congratulations, you have successfully deployed and launched HCL Accelerate in a SoFy Demo Sandbox.</details><details><summary><strong>Steps to seed HCL Accelerate with demo data</strong></summary>
<br />
As HCL Accelerate is data driven and the data is date sensitive, for the purposes of this demo it is important to seed the HCL Accelerate environment with meaningful data simulating integrations with the many tools that typically make up a DevOps pipeline. Tools used for the purposes of planning, continuous integration, continuous delivery, continuous testing, and continuous availability.
    <img align="left" style="width:50%;" src="https://hclcr.io/files/sofy/catalog/hcl-accelerate-demo/generic/accelerate_GettingStarted.png" />
  
**WARNING: Integrations with external repositories, not managed by HCL Software, are not permitted in a SoFy demo environment. To integrate HCL Accelerate with your tool repositories, please reach out to your HCL Software Sales Rep and ask about a Proof of Concept activity.**
  
1. Having navigated to the HCL Accelerate authentication page, log in using "admin" for both the Username and Password. Click "Login".
2. On the "Getting started with HCL Accelerate" page, click "Install demo data" in the *Try sample demo data* panel.
  
  <details><summary>HINT</summary>
  <hr />
   *The Accelerate Getting started page is displayed once by default after the initial log in. If you are not presented with the "Getting started" page after authenticating with Accelerate, click the "?" on the top navigation bar and select "Getting started" from the list of options presented.*
  <hr />
  </details>

3. When the demo data has finished loading (Install complete), navigate to the Settings page gear icon and click Integrations.
4. Disable the EMRI_Bottleneck integration.
5. Enable the EMRI_Bottleneck integration to trigger the bottleneck algorithm calculations.

ADDITIONAL INFO: During the "Populating data" stage of the demo data load, a large number of data points will automatically be written to the MongoDB (Accelerate's repository). As this can take some time, please be patient (up to 15 minutes). The "Try sample demo data" progress bar will show when the demo data has been successfully loaded.
  </details>
</details>
---

<details><summary><strong>What’s New in this Helm Chart Version</strong></summary>
  
</details>
<details><summary><strong>Product Documentation</strong></summary>
  
</details>
<details><summary><strong>Incompatibilities</strong></summary>
  
</details>
<details><summary><strong>Limitations</strong></summary>
  
</details>
<details><summary><strong>Using … in SoFy</strong></summary>
  
</details>
<details><summary><strong>Advanced Configuration Settings</strong></summary>
  
</details>
<details><summary><strong>Supported Environments</strong></summary>
  
</details>
<details><summary><strong>Upgrades</strong></summary>
  
</details>



<details><summary><strong>Collapsible Sections</strong></summary>
  <ul>
    <li>Some content needs to be written as HTML, such as unordered lists.</li>
    <li>On the other hand, quite a lot of markdown still works properly, as shown in the following sections.</li>
  </ul>
</details>
<details><summary><strong>Products Involved</strong></summary>

| Item | Details |
| --- | --- |
| HCL Products included in this demo | HCL OneDB 2.0.1.1 or higher (Helm chart v0.4.14 or later) |
| Estimated install time before ready to use | 6 minutes |

</details>

<details><summary><strong>How It Works In SoFy</strong></summary>

### Access URLs

Build a solution with OneDB and the HCL OneDB High Availability (HA) & Scale-Out Demo Pack, and deploy it into the sandbox. Once your SoFy solution is deployed, you can find all access URLs for this service from the SoFy Solution Console.

1. OneDB Scale-Out demo home page will be at:

   `https://onedb-scale-app.{sandbox-id}.play.{sofy-domain}`

   For example, `https://onedb-scale-app.sbx0034.play.sofy.dev/`

2. OneDB Demo Pack home page will be at:

   `https://onedbdemo.{sandbox-id}.play.{sofy-domain}`

   For example, `https://onedbdemo.sbx0034.play.sofy.dev/`

3. SoFy Solution Console will be at:

   `https://sofy-console.{sandbox-id}.play.{sofy-domain}`

   For example, `https://sofy-console.sbx0034.play.sofy.dev/`

</details>

<details><summary><strong>Troubleshooting & Limitations</strong></summary>

### Limitations

- This demo pack will only function properly in SoFy sandbox environments because it does not work with self-signed certs.

</details>

## Other thoughts

Need to leave a blank line after the closing \<details\> tag.
