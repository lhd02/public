# Setting active power control

{% include "../../../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">When a power station has power limiting requirements, the grid scheduling personnel must temporarily limit the active power fed into the power station or directly disconnect all the active power fed into the power station, that is, active power derating.</mark>

<table><thead><tr><th width="60">No.</th><th width="166">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td>1</td><td>Dry Contact Active Scheduling</td><td></td></tr><tr><td>2</td><td>DI1, DI2, DI3, DI4</td><td></td></tr><tr><td>3</td><td>Percent (%)</td><td><ul><li>Percentage values refer to the final power percentage executed by the device, and the value should be set to the corresponding value according to local grid requirements.</li></ul><ul><li>Positive percentage values indicate inversion (inverter outputs active power), whereas negative values indicate rectification (inverter absorbs active power).</li></ul><ul><li>Supports adding up to 16 percentage value configurations.</li></ul></td></tr></tbody></table>

*
