# DRM0 parameter

According to AS/NZS 4777.2:2020+A1:2021, connecting the inverter to the power grid must meet the Demand Response Mode (DRM) function, of which DRM0 is mandatory.

Figure Connection diagram

<figure><img src="../../../../.gitbook/assets/drm0.png" alt=""><figcaption></figcaption></figure>

{% include "../../../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">Before setting the DRM0 parameter, ensure that the DI1 of the device is not in use and that it is properly connected to the DRED device.</mark>

<table><thead><tr><th width="78">No.</th><th width="149">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td><strong>1</strong></td><td>DI Custom Function Enable</td><td><img src="../../../../.gitbook/assets/3 (8).png" alt="" data-size="line"></td></tr><tr><td><strong>2</strong></td><td>DI Custom Function Input Port</td><td>DI Input 1</td></tr><tr><td><strong>3</strong></td><td>DI Custom Function Mode</td><td>DRM0 mode (switch ON, INV OFF)<br>Notes:<br>Switches S5a, S1a, and S9 of the DRED device are normally closed, and S0 is used to control the power on and off of the inverter. When S0 closes, the inverter is powered off, and when S0 opens, the inverter is powered on.</td></tr><tr><td><strong>4</strong></td><td>Connected AIO Machine SN</td><td>SN of the inverter connected to the DRED device.</td></tr></tbody></table>
