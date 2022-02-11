# HCL Accelerate
## Overview
<img align="right" src="https://www.hcltechsw.com/wps/wcm/connect/306fda5a-0485-4593-876b-d8f4a221b9cf/unprecendented%2Bvisibility%2Binto%2Byour%2Bvalue%2Bstream.jpg?MOD=AJPERES&CACHEID=ROOTWORKSPACE-306fda5a-0485-4593-876b-d8f4a221b9cf-nWaUQ84" style="width:50%;"/>**HCL Accelerate** is a data-driven value stream management platform that automates the delivery and interpretation of data so businesses can make faster, more strategic decisions and streamline processes.

By integrating with the tools you’re already using, HCL Accelerate aggregates data from across your DevOps pipeline to give you actionable insights to get the most out of your DevOps investments. HCL Accelerate is part of HCL Software DevOps, a comprehensive DevOps product suite comprised of powerful, industry-proven software solutions.

**Capabilities include**:

> - **DevOps Analytics**: Transformation leaders can realize the value of hidden continuous delivery data by making it visible and actionable.
- **Pipeline Aggregation**: Development teams with complex, multi-service applications can orchestrate their continuous delivery pipelines in a single view.
- **Release Management**: Release teams can move to more frequent releases with lightweight, self-service tools including templates and automated controls.
- **Value Stream Visualization**: Delivery teams can go beyond traditional Agile views to provide real-time transparency from concept to production.
- **Strategic Decision Making**: Executives get a complete picture of the DevOps organization, and can identify the top-performing teams to harvest best practices.
<br />
  
1. On the console you can adjust the client workload (simulate increasing or decreasing) via the top left panel slider bar.  You will notice the Session Count value for the servers increase or decrease accordingly.
2. On the top right panel, you can view the auto scaling threshold % values which have been set for the demo instance.

    -	Left axis shows the overall cpu usage for the customer.
    -	First column is for the server.  The default threshold value is set to 90% for this demo. In actual OneDB product implementation, the threshold value may be different/is configurable.
    -	Second column shows the Connection Manager. The default threshold is also set to 90%.
    -	Third column shows the count (#) of OneDB servers. This will increase or decrease during the demo.
    -	Fourth column is the count (#) of Connection Managers.

3. Scaling up by the Kubernetes scheduler usually initiates within approximately 3 mins.  The Horizontal Pod Autoscaler (HPA) automatically scales the number of pods in a replication controller, deployment, replica set or stateful set based on observed CPU utilization. (For more info see: [Horizontal Pod Autoscaler | Kubernetes](https://kubernetes.io/docs/tasks/run-application/horizontal-pod-autoscale/)).
4. Scaling down takes slightly longer and initiates within approximately 5 minutes after being under the designated threshold percentage.

---

## HTML Experimentation

### Block Elements

#### Description List (dl, dt, dd)
```
<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>
```

<dl>
  <dt>Coffee</dt>
  <dd>Black hot drink</dd>
  <dt>Milk</dt>
  <dd>White cold drink</dd>
</dl>

#### Preformatted text (pre)

Text in a \<pre\> element is displayed in a fixed-width font, and the text preserves both spaces and line breaks. The text will be displayed exactly as written in the HTML source code.

```
<pre>
Text in a pre element
is displayed in a fixed-width
font, and it preserves
both      spaces and
line breaks, and shows up on a background
</pre>
```

<pre>
Text in a pre element
is displayed in a fixed-width
font, and it preserves
both      spaces and
line breaks, and shows up on a background
</pre>

#### Section (section)

This is two sections:
```
<section>
<h2>WWF History</h2>
<p>The World Wide Fund for Nature (WWF) is an international organization working on issues regarding the conservation, research and restoration of the environment, formerly named the World Wildlife Fund. WWF was founded in 1961.</p>
</section>

<section>
<h2>WWF's Symbol</h2>
<p>The Panda has become the symbol of WWF. The well-known panda logo of WWF originated from a panda named Chi Chi that was transferred from the Beijing Zoo to the London Zoo in the same year of the establishment of WWF.</p>
</section>
```

<section>
<a href="https://www.youtube.com/watch?v=-cCr7AO3J2A"><img align="right" src="YouTubeVideo.png" style="width: 50%;" /></a>
<h2>WWF History</h2>
<p>The World Wide Fund for Nature (WWF) is an international organization working on issues regarding the conservation, research and restoration of the environment, formerly named the World Wildlife Fund. WWF was founded in 1961.</p>
</section>

<section>
<h2>WWF's Symbol</h2>
<p>The Panda has become the symbol of WWF. The well-known panda logo of WWF originated from a panda named Chi Chi that was transferred from the Beijing Zoo to the London Zoo in the same year of the establishment of WWF.</p>
</section>

---

### Inline Elements

#### Keyboard (kbd)

```
<p>Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy text (Windows).</p>
```

<p>Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy text (Windows).</p>

#### Short Quotation (q)

```
<p>WWF's goal is to:
<q>Build a future where people live in harmony with nature.</q>
We hope they succeed.</p>
```

<p>WWF's goal is to:
<q>Build a future where people live in harmony with nature.</q>
We hope they succeed.</p>

#### Sample Output (samp)

```
<p>Message from my computer:</p>
<p><samp>File not found.<br>Press F1 to continue</samp></p>
```

<p>Message from my computer:</p>

<p><samp>File not found.<br>Press F1 to continue</samp></p>

#### Subscript and Superscript (sub and sup)

```
<p>H<sub>2</sub>O</p>
<p>E=MC<sup>2</sup></p>
```

<p>H<sub>2</sub>O</p>
<p>E=MC<sup>2</sup></p>

Variable (var)

```
<p>The area of a triangle is: 1/2 x <var>b</var> x <var>h</var>, where <var>b</var> is the base, and <var>h</var> is the vertical height.</p>
```

<p>The area of a triangle is: 1/2 x <var>b</var> x <var>h</var>, where <var>b</var> is the base, and <var>h</var> is the vertical height.</p>

---

### SECTION 1: Preparing for HCL Accelerate Demo
  <details><summary><strong>Deploying HCL Accelerate to a SoFy sandbox</strong></summary><br />
<i>To experience the demo scenarios documented below, a working instance of HCL Accelerate must be running and seeded with data in a SoFy sandbox.</i><br /><br />

**Steps to deploying and launching HCL Accelerate in SoFy**
  
  <img align="right" style="width:30%" src="https://github.com/scott-good/blog/blob/main/Accelerate_Tile.png" />

1. Locate the HCL Accelerate product card in the SoFy catalog and click "Add to Solution".
2. Enter a solution name and click "Create".

> HINT: Solution names must be comprised of lowercase alphanumeric characters and cannot contain any special characters.
    
> ADDITIONAL INFO: Creating a SoFy solution will result in a custom helm chart being created for the purposes of bootstrapping the HCL Accelerate deployment in a kubernetes environment.

3. Click "Deploy" to create the HCL Accelerate demo environment in a SoFy sandbox. In just a few minutes, SoFy will deploy HCL Accelerate to HCL's Google Cloud sandbox environment.

4. When the deployment has completed, click on "View Solution Console" and authenticate with the credentials provided.
5. At the top of the Solution Console, locate the HCL Accelerate card and click on "General Information".
6. Click on the "Open Link" button to launch HCL Accelerate in a new browser tab.

**CELEBRATE**: Congratulations, you have successfully deployed and launched HCL Accelerate in a SoFy Demo Sandbox!</details><details><summary><strong>Steps to seed HCL Accelerate with demo data</strong></summary>
<br />
  <img align="right" style="width:50%;" src="https://hclcr.io/files/sofy/catalog/hcl-accelerate-demo/generic/accelerate_GettingStarted.png" />
As HCL Accelerate is data driven and the data is date sensitive, for the purposes of this demo it is important to seed the HCL Accelerate environment with meaningful data simulating integrations with the many tools that typically make up a DevOps pipeline. Tools used for the purposes of planning, continuous integration, continuous delivery, continuous testing, and continuous availability.
    

  
> **WARNING: Integrations with external repositories, not managed by HCL Software, are not permitted in a SoFy demo environment. To integrate HCL Accelerate with your tool repositories, please reach out to your HCL Software Sales Rep and ask about a Proof of Concept activity.**
  
1. Having navigated to the HCL Accelerate authentication page, log in using "admin" for both the Username and Password. Click "Login".
2. On the "Getting started with HCL Accelerate" page, click "Install demo data" in the *Try sample demo data* panel.
  
> HINT: The Accelerate <i>Getting started</i> page is displayed once by default after the initial log in. If you are not presented with the "Getting started" page after authenticating with Accelerate, click the "?" on the top navigation bar and select "Getting started" from the list of options presented.

3. When the demo data has finished loading (Install complete), navigate to the Settings page gear icon and click Integrations.
4. Disable the EMRI_Bottleneck integration.
5. Enable the EMRI_Bottleneck integration to trigger the bottleneck algorithm calculations.

> ADDITIONAL INFO: During the "Populating data" stage of the demo data load, a large number of data points will automatically be written to the MongoDB (Accelerate's repository). As this can take some time, please be patient (up to 15 minutes). The "Try sample demo data" progress bar will show when the demo data has been successfully loaded.
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
