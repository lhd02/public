# PV Surplus Charging

<details>

<summary><mark style="color:blue;"><strong>Background Information</strong></mark></summary>

* <mark style="color:blue;">Sigen EV AC Charger cannot start charging in this mode at nighttime. Please use this mode during the daytime.</mark> <mark style="color:blue;">Set "Grid Charging" to</mark> <img src="../../.gitbook/assets/image (2).png" alt="" data-size="line"> <mark style="color:blue;">to allow the Sigen EV AC Charger to obtain charging power from the grid. You can set the "The maximum power from the grid" to limit the amount of power purchased from the grid, therefore saving your tariff.</mark>
* <mark style="color:blue;">Set "Battery Boost" to</mark> <img src="../../.gitbook/assets/image (2).png" alt="" data-size="line"> <mark style="color:blue;">to allow the battery to discharge power to the Sigen EV AC Charger to charge the vehicle, and the discharge cutoff SOC can be set. When set to</mark> <img src="../../.gitbook/assets/image (3).png" alt="" data-size="line"> <mark style="color:blue;">or the battery is discharged to the set cut-off SOC , the Sigen EV AC Charger draws charging power from the surplus PV power and the grid.</mark>
* <mark style="color:blue;">"Battery Boost" is only used to set whether the battery pack discharges power to the Sigen EV AC Charger.</mark>
* <mark style="color:blue;">Drag the device under the "Surplus PV Priority" menu to set the priority of using the surplus PV power (the priority is from top to bottom).</mark>

</details>

* **PV storage and charging system wiring**

When the generated PV power meets the power demand of loads but the surplus PV power is insufficient, power is obtained from the grid. Set "Grid Charging" to <img src="../../.gitbook/assets/image (2).png" alt="" data-size="line"> and set the value for "The maximum power from the grid". When the surplus PV power is sufficient, power is supplied to the device according to the set priority.

* **PV storage and charging system wiring**

When "Battery Boost" is set to <img src="../../.gitbook/assets/image (4).png" alt="" data-size="line"> and the device that uses the surplus PV power is set to the Sigen EV AC Charger taking priority over the battery pack, once the generated PV power meets the power demand of loads, the surplus PV power and the discharging power of battery pack are both supplied to the Sigen EV AC Charger for charging vehicles. When the surplus PV power is insufficient, power is obtained from the grid. Set "Grid Charging" to <img src="../../.gitbook/assets/image (4).png" alt="" data-size="line"> and set the value for "The maximum power from the grid".

When the device that uses the surplus PV power is set to the battery pack taking priority over the Sigen EV AC Charger, the surplus PV power is supplied to the Sigen EV AC Charger for charging vehicles. When the surplus PV power is insufficient, power is obtained from the grid. Set "Grid Charging" to <img src="../../.gitbook/assets/image (4).png" alt="" data-size="line"> and set the value for "The maximum power from the grid".

**Examples of daytime usage scenarios for the Sigen EV AC Charger in PV charging or PV storage and charging system wiring.**

Model: Sigen EVAC 11 4G T2 WH; Output Mode: three-phase.

| A                                                                                                     | B                           | C                                           | D                          | E                                              |
| ----------------------------------------------------------------------------------------------------- | --------------------------- | ------------------------------------------- | -------------------------- | ---------------------------------------------- |
| Generated power of PV system or generated power of PV system + discharging power of battery pack (kW) | Consumed power of load (kW) | Compensating power of grid (kW) C=(D-(A-B)) | Actual charging power (kW) | The maximum power from the grid set value (kW) |
| 20                                                                                                    | 15                          | 0                                           | 5                          | 4.14                                           |
| 20                                                                                                    | 18                          | 2.14                                        | 4.14                       | 4.14                                           |
| 20                                                                                                    | 25                          | 9.14\[1]                                    | 4.14                       | 4.14                                           |
| 20                                                                                                    | 15                          | 0                                           | 5                          | 1                                              |
| 20                                                                                                    | 16                          | 0.14                                        | 4.14                       | 1                                              |
| 20                                                                                                    | 18                          | 2.14\[2]                                    | 4.14\[2]                   | 1                                              |

* When the DLM function is enabled, the minimum starting charging power of Sigen EV AC Charger is 5.52 kW (three-phase output) or 1.84 kW (single-phase output). In other cases (Fast Charging), the minimum starting charging power of Sigen EV AC Charger is 4.14 kW (three-phase output) or 1.38 kW (single-phase output).
* Note \[1]: In this scenario, if the generated PV power or the generated PV power together with the discharging power of the battery pack is consumed by the loads, there is still a need for 4.14 kW of grid input power. The charging power of the Sigen EV AC Charger must be sourced from the grid, and the actual charging power must be less than or equal to the set value of "The maximum power from the grid."
* Note \[2]: In this scenario, after the generated power of the PV system or generated power of the PV system + discharging power of the battery pack is consumed by the loads, 2 kW remains. The surplus PV power can be used to charge the Sigen EV AC Charger. The minimum starting charging power of the Sigen EV AC Charger is 4.14 kW, which requires 2.14 kW of grid input power. If the grid input power of Sigen EV AC Charger exceeds the set value of "The maximum power from the grid," the charging will continue for 6 minutes. If, after 6 minutes, the actual charging power still exceeds the set value of "The maximum power from the grid," the Sigen EV AC Charger will stop charging.
