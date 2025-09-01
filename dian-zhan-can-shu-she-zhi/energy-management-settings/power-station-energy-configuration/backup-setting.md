# Backup Setting

## Backup Reserve

{% include "https://app.gitbook.com/s/UbDQx7leHsTF4wXWth5S/~/reusable/v0ROOBJtnqMcvClWk0gj/" %}

* <mark style="color:blue;">Skip this section if no Gateway is configured.</mark>
* <mark style="color:blue;">Users can manually set this parameter according to the power interruption frequency of their regions and leave time.</mark>

If there is a gateway in your networking, you can manually set the "Backup Reserve" value in the mySigen App. In grid connection mode, the battery stops discharging when the backup power SOC setting is reached. In the event of grid power outage, the backup power becomes available.

For example, the backup power SOC is set in Self-Consumption Mode.

<figure><img src="../../../.gitbook/assets/SSA1OV00014-en.jpg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/MSA1CM00071-备电设置.png" alt=""><figcaption></figcaption></figure>

## Backup History

{% include "https://app.gitbook.com/s/OGIICehJiMvqdVX7wksn/~/reusable/p4FUqXvLmYuzqficHZJF/" %}

<mark style="color:blue;">After installing the Gateway in the system, grid-connection and off-grid events will be automatically recorded. You can view the timing and reasons for grid mode switching through the following methods.</mark>

## Storm Watch

{% include "https://app.gitbook.com/s/OGIICehJiMvqdVX7wksn/~/reusable/p4FUqXvLmYuzqficHZJF/" %}

* This function is only available for power stations that have batteries and have enabled the off-grid function.
* After enabling this function, the system will charge the batteries in advance after obtaining extreme weather information.

<figure><img src="../../../.gitbook/assets/MSA1CM00085-风暴预警.png" alt="" width="297"><figcaption></figcaption></figure>

<table><thead><tr><th width="81.88885498046875" align="center" valign="middle">No.</th><th width="178.3233642578125" valign="middle">Parameter name</th><th width="458.888916015625" valign="top">Description</th></tr></thead><tbody><tr><td align="center" valign="middle">1</td><td valign="middle">Storm Watch</td><td valign="top">When set to<img src="../../../.gitbook/assets/image (38).png" alt="">，the Storm Watch function is enabled.</td></tr><tr><td align="center" valign="middle">2</td><td valign="middle">Backup Settings</td><td valign="top">Enable backup before the storm：Set the duration for pre - charging before extreme weather, which can be set from 1 - 24 hours.</td></tr><tr><td align="center" valign="middle">3</td><td valign="middle">Weather Warnings</td><td valign="top">Select the type of extreme weather.</td></tr></tbody></table>
