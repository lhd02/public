# DI customization

<table><thead><tr><th width="60" align="center">No.</th><th width="166">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td align="center"><p></p><p>1</p></td><td>DI Custom Function Enable</td><td>When set to <img src="../../../.gitbook/assets/image (5).png" alt="">, the DI custom function is enabled, and you can set related parameters. The function becomes unavailable when disabled.</td></tr><tr><td align="center">2</td><td>DI Custom Function Input Port</td><td>Set the DI port to which the device connects to according to the wiring.</td></tr><tr><td align="center">3</td><td>DI Custom Function Mode</td><td><ul><li>If set to "External Switch Control mode (switch ON, INV ON)," when the connected device switch is turned on, the inverter is powered on, and when the device switch is turned off, the inverter is shut down.</li><li>If set to "DRM0 mode (switch ON, INV OFF)," when the connected device switch is turned on, the inverter is shut down, and when the device switch is turned off, the inverter is powered on.</li><li>If set to "Micro-grid Control mode: (Switch OFF: Off grid INV standby, On-grid INV ON)," when the connected device switch is turned off and grid power outage occurs, the AC side of the inverter is in standby mode. When the power grid is restored and connected to the grid, the inverter operates normally. When the device switch is turned on and grid power outage occurs, the inverter can operate in off-grid mode.</li><li>If set to "Micro-grid Control mode: (Switch ON: Off grid INV standby, On-grid INV ON)," when the connected device switch is turned on and grid power outage occurs, the AC side of the inverter is in standby mode. When the power grid is restored and connected to the grid, the inverter operates normally. When the device switch is turned off and a grid power outage occurs, the inverter can operate in off-grid mode.</li><li>If set to "Gateway Bypass mode (state of switch)," when the connected device switch is turned off and the bypass switch of Gateway is turned on, the inverter cannot operate in off-grid mode. When the device switch is turned on, and the bypass switch of Gateway is turned off, the inverter can operate in off-grid mode.</li><li>If set to "Transfer Switch Position II Status Detection," when the connected device switch is turned off, the transfer switch is in on-grid mode, and the inverter cannot operate in off-grid mode. When the device switch is turned on, the transfer switch is in off-grid mode, and the inverter can operate in off-grid mode.</li></ul></td></tr><tr><td align="center">4</td><td>Connected AIO Machine SN</td><td>Set the SN of the inverter to which the device connects.</td></tr></tbody></table>



## DRM0 parameter

ccording to AS/NZS 4777.2:2020+A1:2021, connecting the inverter to the power grid must meet the Demand Response Mode (DRM) function, of which DRM0 is mandatory.

<sub>**Connection diagram:**</sub>

{% include "../../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">Before setting the DRM0 parameter, ensure that the DI1 of the device is not in use and that it is properly connected to the DRED device.</mark>

<table><thead><tr><th width="60" align="center">No.</th><th width="253.272705078125">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td align="center">1</td><td>DI Custom Function Enable</td><td><img src="../../../.gitbook/assets/image (6).png" alt=""></td></tr><tr><td align="center">2</td><td>DI Custom Function Input Port</td><td>DI Input 1</td></tr><tr><td align="center">3</td><td>DI Custom Function Mode</td><td><p>DRM0 mode (switch ON, INV OFF)</p><p>Notes:</p><p>Switches S5a, S1a, and S9 of the DRED device are normally closed, and S0 is used to control the power on and off of the inverter. When S0 closes, the inverter is powered off, and when S0 opens, the inverter is powered on.</p></td></tr><tr><td align="center">4</td><td>Connected AIO Machine SN</td><td>SN of the inverter connected to the DRED device.</td></tr></tbody></table>



## NS protection parameter

In areas where VDE4105 standards apply, such as VDE-AR-N-4105, VDE-AR-N 4110, and VDE-AR-N 4120, power generating equipment in a power station must support connection with network and system protection (NS) devices.

&#x20;<sub>**Connection diagram**</sub>

{% include "../../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">DI5 is recommended. If DI1–DI4 is not in use, any one of DI1 to DI5 can be connected to the NS protection device.</mark>
* <mark style="color:blue;">Before setting parameters, ensure that the NS protection device is correctly connected.</mark>

<table><thead><tr><th width="69" align="center">No.</th><th width="284.3636474609375">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td align="center">1</td><td>DI Custom Function Enable</td><td><img src="../../../.gitbook/assets/image (6).png" alt=""></td></tr><tr><td align="center">2</td><td>DI Custom Function Input Port</td><td>DI Input 5 (If the NS protection device is connected to another DI port, make settings based on the port)</td></tr><tr><td align="center">3</td><td>DI Custom Function Mode</td><td><p>DRM0 mode (switch ON, INV OFF)</p><p>Notes:</p><p>When the power grid operates abnormally, the NS protection device is turned on, and the inverter automatically shuts down. When the power grid recovers, the NS protection device is turned off, and the inverter is powered on.</p></td></tr><tr><td align="center">4</td><td>Connected AIO Machine SN</td><td>SN of the inverter connected to the NS protection device.</td></tr></tbody></table>
