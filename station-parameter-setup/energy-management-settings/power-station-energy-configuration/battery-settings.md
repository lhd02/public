# Battery Settings

Setting battery-related parameters can optimize battery performance, extend battery life, and achieve intelligent charging and discharging strategies.

## Charging Source Prority

{% include "../../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">**By default priority, PV is placed before Grid, PV solar charges the battery first，Grid supplements the remaining charge.**</mark>
* <mark style="color:blue;">**In the negative electricity price scenario, Grid can be adjusted to be before PV.**</mark>
* <mark style="color:blue;">**The battery acquires power according to the set order.**</mark>

<figure><img src="../../../.gitbook/assets/MSA1CM00073-电网设置-电网输出优先级 (1).png" alt="" width="563"><figcaption></figcaption></figure>

## Discharging Source Prority

{% include "../../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">Battery releases power according to the set order. The battery discharge priority can be configured based on the actual situation.</mark>

<figure><img src="../../../.gitbook/assets/MSA1CM00073-电池放电优先级.png" alt="" width="375"><figcaption></figcaption></figure>



## Battery Level Setting

<figure><img src="../../../.gitbook/assets/MSA1CM00073-电池电量设置 (1).png" alt="" width="563"><figcaption></figcaption></figure>

<table><thead><tr><th width="63" align="center">No.</th><th width="191">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td align="center">1</td><td>Charge Cut-off SOC</td><td>Sets the capacity at which the battery pack stops charging.</td></tr><tr><td align="center">2</td><td>Discharge Cut-off SOC</td><td><ul><li>Sets the capacity at which the battery pack stops discharging.</li><li>Value 0 is not recommended for this parameter to avoid irreversible attenuation due to failure to charge the battery pack in time.</li><li>The priority is given to "Backup Capacity" in backup system wiring mode, while the parameter is applied in non-backup system wiring mode.</li></ul></td></tr><tr><td align="center">3</td><td>Peak shaving</td><td>Set the battery peak shaving cutoff point.</td></tr><tr><td align="center">4</td><td>Backup Reserve SOC</td><td><ul><li>You can set this parameter when a gateway exists in the system wiring.</li><li>In the on-grid scenario, the battery pack stops discharging when the backup capacity value is reached. In the off-grid scenario, the battery pack supplies power to power device and stops discharging when the Discharge Cut-off SOC setting is reached.</li><li>Users can manually set this parameter according to the power interruption frequency of their regions and leave time. Value 0 is not recommended for this parameter to avoid irreversible attenuation due to failure to charge the battery pack in time.</li></ul></td></tr></tbody></table>

## Battery Preheating scheduling

{% include "../../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">Pre-adjust the battery temperature to the optimal working range in low temperature environments to prevent performance degradation and safety hazards caused by low temperature.</mark>

<figure><img src="../../../.gitbook/assets/MSA1CM00073-电池设置-预热调度 (1).png" alt="" width="375"><figcaption></figcaption></figure>

<table><thead><tr><th width="67" align="center">No.</th><th width="206">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td align="center">1</td><td>Pack preheating</td><td>Set to <img src="../../../.gitbook/assets/image (1) (1) (1) (1) (1).png" alt=""> to set the battery preheating period.</td></tr></tbody></table>

## Battery Power Limit

{% include "../../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">If you need to set more detailed charging and discharging data, you can set this parameter.</mark>

<figure><img src="../../../.gitbook/assets/MSA1CM00073-电池功率设置.png" alt="" width="375"><figcaption></figcaption></figure>

<table><thead><tr><th width="77" align="center">No.</th><th width="259">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td align="center">1</td><td>Battery Max Charging Power</td><td>Set the maximum charging input power allowed by the battery.</td></tr><tr><td align="center">2</td><td>Battery Max Discharging Power</td><td>Set the maximum discharging output power allowed by the battery.</td></tr></tbody></table>

## Battery Automation

{% include "../../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">If this parameter is set, the battery will prioritize executing the parameters set by Battery Automation.</mark>

<figure><img src="../../../.gitbook/assets/MSA1CM00073-电池自动化.png" alt="" width="563"><figcaption></figcaption></figure>

<table><thead><tr><th width="68" align="center">No.</th><th width="148">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td align="center">1</td><td>Add Time Period</td><td>Click to add Time Period.</td></tr><tr><td align="center">2</td><td>Add your action</td><td><p>Click to add battery operation status.</p><p><strong>Battery Charging</strong></p><ol><li>Maximum Charging Power: Set the maximum total input power allowed for the battery charging, including all charging sources.</li><li>Maximum Charging Power From grid to BAT: Set the maximum charging input power from Grid to BAT. This parameter must be ≤ Maximum Charging Power.</li><li>Battery Charging From Grid Cut-off SOC: When the battery SOC reaches this threshold, the grid is forced to stop charging the battery.</li><li>Battery Charging Source Priority: Adjust the battery energy source priority.</li></ol><p><strong>Battery Discharging</strong></p><ol><li>Maximum Discharging Power: Set the maximum total discharging output power allowed for the battery.</li><li>Maximum Discharging Power from BAT to Grid: Set the maximum discharging output power from BAT to Grid.This parameter must be ≤ Maximum Discharging Power.</li><li>Discharge Cut-off SOC from BAT to Grid: When the battery SOC reaches this threshold, the BAT is forced to stop transmitting power to the grid.</li></ol><p><strong>Battery Preserve: Maintain the current SOC without change.</strong></p><p><strong>Battery Self Consumption</strong></p><ol><li>Maximum Charging Power: Set the maximum charging input power from PV to the battery.</li><li>Maximum Discharging Power: Set the maximum discharging output power of the battery to the household load.</li></ol></td></tr></tbody></table>
