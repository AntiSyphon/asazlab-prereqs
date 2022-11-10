# Pre-Requisite : Deploy course Lab Environment (ASAZLab.com)


Students are required to deploy the ASAZLab in their Azure subscription.

## Important Information
* An "upgraded" or "Pay-as-you-go" Azure account is required to deploy the lab environment.  See other pre-requisite instruction if you do not yet have an Azure account.
* The cost of the lab environment is approximately $20/day for A2 sized VMs.
* Remember after the end of class delete your lab environment to ensure you have no unexpected fees from Azure.
* The VM size selection will default to B2s, A2,or A2_V2 depending on region selection and availability.  Generally B2s is least expensive if available. Any of these options are acceptable for the lab environment.

## Deploy Antisyhon Training Azure Lab (ASAZLab)

<Details><summary> <b> Step 1: Kickoff Deployment</b></summary>
<blockquote>

Deploy the Antisyhon Training AZLab from ASAZLab.com:
* https://www.ASAZLab.com

[ASAZLab][ASAZLab]

| ![](../images/prls2-1.jpg) |
|----------------------------|

Or, you can view the operations in more detail on GitHub:
[ASAZLab-Github][ASAZLab-Github]

| ![](../images/prls2-2a.jpg)|
|----------------------------|


And, deploy via the README with one click!! 

**Be sure you are in a browser session you are either comfortable authenticating to Azure or you already have an authenticated session.**

| ![](../images/prls2-2b.jpg) |
|----------------------------|

Next up you will choose your subscription, resource group, and region.  


| ![](../images/prls2-3.jpg) |
|----------------------------|

The VM size selection will default to B2s, A2,or A2_V2 depending on region selection and availability.  Generally B2s is least expensive if available. Any of these options are acceptable for the lab environment.

Feel free to modify the size of your VMs should you so choose. The default selections made for this course have been tested thoroughly and represent a balance of performance and cost.


|![](../images/prls2-4.jpg)|
|----------------------------|

The next step in your custom deployment is to confirm the public IP space. Feel free to limit this range more specifically to your known and trusted addresses. 

**Please be aware that a demonstration will be provided and a discussion around this exposure and that leaving this address wide open (0.0.0.0/0) presents an interesting perspective of the Internet and the risks of exposing services there.**

| ![](../images/prls2-5.jpg) |
|----------------------------|

That is pretty much it for the configuration of your ARM template based deployment of the DO AZ lab environment. The next screenshot includes a warning about agreeing to the terms on Microsoft.

| ![](../images/prls2-6.jpg) |
|----------------------------|

Whether you agree or not, should you choose to click Create, you implicitly do.

| ![](../images/prls2-7.jpg) |
|----------------------------|

The full deployment will take approximately 45 minutes.  You do not need to keep the window open, the process will continue even if you close it.  In the following section, you will configure the new lab environment to report logs to Azure Sentinel.  You must wait for deployment to complete before continuing.
</blockquote>
</details>

<Details><summary> <b>Step 2: Gather Public IP Addresses for Access</b></summary>
<blockquote>

Gather your public IP addresses. 

**https://portal.azure.com/#home --> Resource groups --> <ASAZ_Lab_Resource_Group> --> Resources --> Filter --> "public"**

| ![](../images/prls4-1.jpg) |
|----------------------------|

Click through each resource to gather the assigned public IP addresses.

| ![](../images/prls4-2.jpg) |
|----------------------------|

As you gather them up, document them!   Be sure you have the following IP addresses documented to be ready for class.
```
DC01 (pip-DC01) Public IP:
SRV01 (pip-SRV01) Public IP:
WS05 (pip-WS05) Public IP: 
Nux (pip-Nux01) Public IP: 
```


</blockquote>
</details>


---

Copyright - All Rights Reserved, Antisyhon Training LLC


  [ASAZLab]: https://www.ASAZLab.com
  [ASAZLab-Github]: https://github.com/AntiSyphon/asazlab
  [WWHF]: https://wildwesthackinfest.com/
  [2]: https://wildwesthackinfest.com/training/