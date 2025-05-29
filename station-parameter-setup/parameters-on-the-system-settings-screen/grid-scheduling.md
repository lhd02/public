# Grid scheduling

## Power regulation

{% include "../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">In Germany and some European areas, the Ripple Control Receiver is used to convert power grid scheduling signals to dry contact signals, which are then transmitted to power stations. The dry contact communication mode is required to receive the power grid scheduling signal to achieve active and reactive power scheduling for the power station.</mark>
* <mark style="color:blue;">Before this operation, ensure that the inverter you want to configure is connected with the Ripple Control Receiver and ports DI1–DI4 (ports 5–8 for an aviation connector) are not in use. For details, please refer to the Installation Guide.</mark>



## Setting active power control

{% include "../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">When a power station has power limiting requirements, the grid scheduling personnel must temporarily limit the active power fed into the power station or directly disconnect all the active power fed into the power station, that is, active power derating.</mark>

<figure><img src="../../.gitbook/assets/3 (1).jpeg" alt="" width="228"><figcaption></figcaption></figure>

<table><thead><tr><th width="67">No.</th><th width="144">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td><strong>1</strong></td><td>Dry Contact Active Scheduling</td><td>When it is set to <img src="../../.gitbook/assets/2 (9).png" alt="" data-size="line">, you do not need to set the SN for a single device. For multiple devices, drop down and select the SN of the device connected to the Ripple Control Receiver. You can view the SN on the side of the device.</td></tr><tr><td><strong>2</strong></td><td>DI1, DI2, DI3, DI4</td><td><p><img src="../../.gitbook/assets/settingactive.png" alt="" data-size="line">indicates that the switch set on the DI cable is turned on and it is low level.<br><img src="../../.gitbook/assets/seetingdeactive.png" alt="" data-size="line">indicates that the switch set on the DI cable is turned off and it is high level.<br>The parameters shown in the figure are for reference only. Configure these parameters as needed.</p><ul><li>The status combination of DI1 to DI4 must not be duplicated. Otherwise, a command parsing error occurs.</li><li>If the actual DI signal does not match the setting in the App, the device will operate at the maximum active power command (100%).</li></ul></td></tr><tr><td><strong>3</strong></td><td>Percent (%)</td><td><ul><li>Percentage values refer to the final power percentage executed by the device, and the value should be set to the corresponding value according to local grid requirements.</li><li>Positive percentage values indicate inversion (inverter outputs active power), whereas negative values indicate rectification (inverter absorbs active power).</li><li>Supports adding up to 16 percentage value configurations.</li></ul></td></tr></tbody></table>



## Setting reactive power control

{% include "../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">The grid operator requires a large-scale power station to have a certain ability to regulate the voltage at the grid connection point. The grid scheduling personnel schedules the power station to absorb or inject reactive power to the grid connection point according to the real-time reactive power transmission condition in the power grid, that is, reactive power compensation.</mark>

![](<../../.gitbook/assets/3 (1).jpeg>)

<table><thead><tr><th width="72">No.</th><th width="139">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td><strong>1</strong></td><td>Reactive Power Control Mode</td><td><ul><li>No Output: If the grid operator does not require the power station to regulate the voltage at the grid connection point and does not need to implement reactive power compensation, devices can maintain the output with pure active power. In this case, set to "No Output."</li><li>DI mode: Set to "DI mode" when setting dry contact reactive scheduling parameters.</li><li>Grid connection point power factor control: When a distributed power station needs to implement distributed reactive power compensation to reduce or avoid power-factor-adjusted electricity cost and increase power station revenue, you must set "Grid connection point power factor control."</li><li>When the DI mode is selected, you do not need to set the SN for a single device. For multiple devices, drop down and select the SN of the device connected to the Ripple Control Receiver. You can view the SN on the side of the device.</li></ul></td></tr><tr><td><strong>2</strong></td><td>DI1, DI2, DI3, DI4</td><td><p><img src="../../.gitbook/assets/settingactive.png" alt="" data-size="line">indicates that the switch set on the DI cable is turned on and it is low level.<br><img src="../../.gitbook/assets/seetingdeactive.png" alt="" data-size="line">indicates that the switch set on the DI cable is turned off and it is high level.</p><ul><li>The parameters shown in the figure are for reference only. Configure these parameters as needed.</li><li>The status combination of DI1 to DI4 must not be duplicated. Otherwise, a command parsing error occurs.</li><li>If the actual DI signal does not match the setting in the App, the device will operate at the minimum reactive power command (0%).</li></ul></td></tr><tr><td><strong>3</strong></td><td>Percent (%)</td><td><ul><li>Percentage values refer to the final power percentage executed by the device, and the value should be set to the corresponding value according to local grid requirements.</li><li>Positive percentage values indicate the output of capacitive reactive power (raising voltage), whereas negative values indicate the output of inductive reactive power (lowering voltage).</li><li>/Supports adding up to 16 percentage value configurations.</li></ul></td></tr></tbody></table>

