# NS protection parameter

In areas where VDE4105 standards apply, such as VDE-AR-N-4105, VDE-AR-N 4110, and VDE-AR-N 4120, power generating equipment in a power station must support connection with network and system protection (NS) devices.

&#x20;<sub>**Connection diagram**</sub>

{% include "../../../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">DI5 is recommended. If DI1–DI4 is not in use, any one of DI1 to DI5 can be connected to the NS protection device.</mark>
* <mark style="color:blue;">Before setting parameters, ensure that the NS protection device is correctly connected.</mark>

<table><thead><tr><th width="69" align="center">No.</th><th width="198">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td align="center">1</td><td>DI Custom Function Enable</td><td><img src="../../../../.gitbook/assets/image (6).png" alt=""></td></tr><tr><td align="center">2</td><td>DI Custom Function Input Port</td><td>DI Input 5 (If the NS protection device is connected to another DI port, make settings based on the port)</td></tr><tr><td align="center">3</td><td>DI Custom Function Mode</td><td><p>DRM0 mode (switch ON, INV OFF)</p><p>Notes:</p><p>When the power grid operates abnormally, the NS protection device is turned on, and the inverter automatically shuts down. When the power grid recovers, the NS protection device is turned off, and the inverter is powered on.</p></td></tr><tr><td align="center">4</td><td>Connected AIO Machine SN</td><td>SN of the inverter connected to the NS protection device.</td></tr></tbody></table>
