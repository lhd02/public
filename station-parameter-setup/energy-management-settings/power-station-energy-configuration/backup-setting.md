# Backup Setting

## Backup Reserve

{% include "../../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">**By default priority, PV is placed before Battery. PV power prioritizes grid feed-in, with battery supplementing grid sales.**</mark>
* <mark style="color:blue;">**Skip this section if no Gateway is configured.**</mark>
* <mark style="color:blue;">**Users can manually set this parameter according to the power interruption frequency of their regions and leave time.**</mark>

If there is a gateway in your networking, you can manually set the "Backup Reserve" value in the mySigen App. In grid connection mode, the battery stops discharging when the backup power SOC setting is reached. In the event of grid power outage, the backup power becomes available.

For example, the backup power SOC is set in Self-Consumption Mode.

<figure><img src="../../../.gitbook/assets/SSA1OV00014-en.jpg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/MSA1CM00078-备电设置.png" alt=""><figcaption></figcaption></figure>

## Backup History

{% include "../../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">**After Gateway is installed in the system, the system records on-grid/off-grid events. You can view the time and reason for the on-/off-grid switchover through the following methods.**</mark>

<figure><img src="../../../.gitbook/assets/MSA1CM00078-备电历史.png" alt=""><figcaption></figcaption></figure>

## Backup Event Center

<figure><img src="../../../.gitbook/assets/MSA1CM00078-备电事件.png" alt=""><figcaption></figcaption></figure>
