# Fast Charging

Sigen EV AC Charger can achieve the fastest charging speed when it charges the vehicle with the maximum available power. In other words, when the generated PV power meets the power demand of loads, the surplus PV power, discharging power of battery pack and grid input power are supplied together to the Sigen EV AC Charger to charge the vehicle. You can use "Battery Boost" to set whether the battery pack is to be discharged. When set to <img src="../../.gitbook/assets/image.png" alt="" data-size="line">, the battery is allowed to discharge power to the Sigen EV AC Charger to charge the vehicle, and the discharge cutoff SOC can be set. When set to <img src="../../.gitbook/assets/image (1).png" alt="" data-size="line"> or the battery is discharged to the set cut-off SOC , the Sigen EV AC Charger draws charging power from the surplus PV power and the grid.

{% include "https://app.gitbook.com/s/TloersTHotEHfhAYIXek/~/reusable/XFcVPnhaLr201f139kSa/" %}

<mark style="color:blue;">**"Battery Boost" is only used to set whether the battery pack discharges power to the Sigen EV AC Charger.**</mark>

* **Charger System Wiring**

The charging power is obtained from the grid. This mode is used by default and no setting is required.

* **PV charging system wiring**

**Daytime**: When the generated PV power meets the power demand of loads, the surplus PV power is supplied to the Sigen EV AC Charger for charging vehicles. When the surplus PV power is insufficient, the charger obtains power from the grid. “Battery Boost” cannot be set in this mode.

**Nighttime**: The charging power is sourced from the grid.

* **PV storage and charging system wiring**

**Daytime**: When "Battery Boost" is set to <img src="../../.gitbook/assets/image.png" alt="" data-size="line">, once the generated PV power meets the power demand of loads, the surplus PV power and the discharge power of battery pack are both supplied to the Sigen EV AC Charger for charging vehicles. When the surplus PV power is insufficient, the charger obtains power from the grid.

**Nighttime**: When "Battery Boost" is set to <img src="../../.gitbook/assets/image.png" alt="" data-size="line">, once the discharge power of battery pack meets the power demand of loads, the surplus power is supplied to the Sigen EV AC Charger for charging vehicles. When the discharge power of battery pack is insufficient, the charger obtains power from the grid.

**Examples of daytime usage scenarios for the Sigen EV AC Charger in PV charging or PV storage and charging system wiring.**

Model: Sigen EVAC 11 4G T2 WH; Output mode: three-phase; **Household Circuit Breaker** in the connected distribution panel: 44 kW (63A); "Grid import Power Limit": 44 kW.

| A                                                                                                     | B                           | C                                                        | D                          |
| ----------------------------------------------------------------------------------------------------- | --------------------------- | -------------------------------------------------------- | -------------------------- |
| Generated power of PV system or generated power of PV system + discharging power of battery pack (kW) | Consumed power of load (kW) | <p>Compensating power of grid (kW)</p><p>C=(D-(A-B))</p> | Actual charging power (kW) |
| 20                                                                                                    | 15                          | 6                                                        | 11                         |
| 10                                                                                                    | 40                          | 41                                                       | 11                         |
| 5                                                                                                     | 40                          | 44                                                       | 9\[1]                      |
| 0                                                                                                     | 40                          | 40                                                       | 0 (Do not start \[2])      |

**Note \[1]**: When C is no greater than the maximum available power, and when the DLM function is enabled, the maximum available power of the Sigen EV AC Charger is D = (A + maximum available power) - B.

**Note \[2]:**

* When C is no greater than the maximum available power, and when the DLM function is enabled, if D is less than the minimum starting power of Sigen EV AC Charger, Sigen EV AC Charger will not start.
* When the DLM function is enabled, the minimum starting charging power of Sigen EV AC Charger is 5.52 kW (three-phase output) or 1.84 kW (single-phase output). In other cases (PV Surplus Charging), the minimum starting charging power of Sigen EV AC Charger is 4.14 kW (three-phase output) or 1.38 kW (single-phase output).
