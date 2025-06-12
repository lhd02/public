# DRM0 parameter

ccording to AS/NZS 4777.2:2020+A1:2021, connecting the inverter to the power grid must meet the Demand Response Mode (DRM) function, of which DRM0 is mandatory.

<sub>**Connection diagram:**</sub>

{% include "../../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">Before setting the DRM0 parameter, ensure that the DI1 of the device is not in use and that it is properly connected to the DRED device.</mark>

<table><thead><tr><th width="60" align="center">No.</th><th width="166">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td align="center">1</td><td>DI Custom Function Enable</td><td><img src="../../../.gitbook/assets/image (3).png" alt=""></td></tr><tr><td align="center">2</td><td>DI Custom Function Input Port</td><td>DI Input 1</td></tr><tr><td align="center">3</td><td>DI Custom Function Mode</td><td><p>DRM0 mode (switch ON, INV OFF)</p><p>Notes:</p><p>Switches S5a, S1a, and S9 of the DRED device are normally closed, and S0 is used to control the power on and off of the inverter. When S0 closes, the inverter is powered off, and when S0 opens, the inverter is powered on.</p></td></tr><tr><td align="center">4</td><td>Connected AIO Machine SN</td><td>SN of the inverter connected to the DRED device.</td></tr></tbody></table>
