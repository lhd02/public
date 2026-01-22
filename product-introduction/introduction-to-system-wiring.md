# Introduction to system wiring

* This product is applicable to household backup power system networking scenarios. It must be used in conjunction with PV panels, inverters, battery packs, main control switches, loads, generators, and power grid.
* In the event of a power outage, the household energy storage system switches to off-grid operation mode. After the power grid resumes normal operation, the household energy storage system switches back to on-grid mode. This achieves a seamless switchover between PV storage and Generator.

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">Under backup power networking, the duration of off-grid operation of the backup power load is related to the power supply capacity of the PV storage system. If there is an abnormality in the power supply of the PV storage system during off-grid operation (including but not limited to abnormal PV power generation, insufficient battery power, and abnormal power supplies to the Generator), the backup power load will still be unable to operate.</mark>
* <mark style="color:blue;">The networking diagram takes two inverters as an example. The number of inverters that can be connected depends on the Gateway specification. For more information, see Table 2-1.</mark>

**Table 2-1**

<table><thead><tr><th width="107" align="center">S/N</th><th>Model</th><th>Number of Inverters that can be connected</th></tr></thead><tbody><tr><td align="center">1</td><td>Sigen Gateway SP AU</td><td>2 units</td></tr><tr><td align="center">2</td><td>Sigen Gateway Home SP</td><td>1 units</td></tr><tr><td align="center">3</td><td>Sigen Gateway Home SP AU</td><td>2 units</td></tr><tr><td align="center">4</td><td>Sigen Gateway Home SP 12K</td><td>1 units</td></tr><tr><td align="center">5</td><td>Sigen Gateway Home SP 12K CN</td><td>1 units</td></tr><tr><td align="center">6</td><td>Sigen Gateway Home Single Phase 12K</td><td>1 units</td></tr><tr><td align="center">7</td><td>Sigen Gateway HomePro SP</td><td>1 units</td></tr><tr><td align="center">8</td><td>Sigen Gateway HomePro SP-F</td><td>1 units</td></tr><tr><td align="center">9</td><td>Sigen Gateway HomePro SP-F AU</td><td>2 units</td></tr><tr><td align="center">10</td><td>Sigen Gateway HomeMax SP</td><td>3 units</td></tr><tr><td align="center">11</td><td>Sigen Gateway HomeMax SP 12K</td><td>2 units</td></tr><tr><td align="center">12</td><td>Sigen Gateway HomeMax SP LA</td><td>2 units</td></tr><tr><td align="center">13</td><td>Sigen Gateway Loadhub</td><td>2 units</td></tr><tr><td align="center">14</td><td>Sigen Gateway TP AU</td><td>2 units</td></tr><tr><td align="center">15</td><td>Sigen Gateway Home TP</td><td>1 units</td></tr><tr><td align="center">16</td><td>Sigen Gateway Home TP AU</td><td>2 units</td></tr><tr><td align="center">17</td><td>Sigen Gateway Home TP 30K</td><td>1 units</td></tr><tr><td align="center">18</td><td>Sigen Gateway Home TP 30K CN</td><td>1 units</td></tr><tr><td align="center">19</td><td>Sigen Gateway Home Three Phase 30K</td><td>1 units</td></tr><tr><td align="center">20</td><td>Sigen Gateway Home Three Phase 30K CN</td><td>1 units</td></tr><tr><td align="center">21</td><td>Sigen Gateway HomePro TP</td><td>2 units</td></tr><tr><td align="center">22</td><td>Sigen Gateway HomePro TP-L</td><td>2 units</td></tr><tr><td align="center">23</td><td>Sigen Gateway HomeMax TP</td><td>2 units</td></tr><tr><td align="center">24</td><td>Sigen Gateway HomeMax TP CN</td><td>2 units</td></tr></tbody></table>

### **Whole home backup system wiring diagram**

**Single inverter (Gateway has the circuit breaker for connecting smart load/generator)**

![](../.gitbook/assets/SSA1OV00029-单逆-en.jpg)

**Single inverter (Gateway does not have the circuit breaker connected to the smart load/generator)**

![](../.gitbook/assets/SSA1OV00029-单逆无智-en.jpg)

**Multiple inverters (Gateway has the circuit breaker for connecting smart load/generator)**

![](../.gitbook/assets/SSA1OV00029-多逆有智en.png)

**Multiple inverters (Gateway does not have the circuit breaker connected to the smart load/generator)**

![](../.gitbook/assets/SSA1OV00029-多逆无智en.png)

<table><thead><tr><th width="71" align="center">No.</th><th>Description</th><th width="69.8182373046875" align="center">No.</th><th>Description</th><th width="70.0908203125" align="center">No.</th><th>Description</th></tr></thead><tbody><tr><td align="center"><strong>A</strong></td><td>PV panel</td><td align="center"><strong>B</strong></td><td>SigenStor EC/Sigen Hybrid</td><td align="center"><strong>C</strong></td><td>SigenStor BAT</td></tr><tr><td align="center"><strong>D</strong></td><td>Gateway</td><td align="center"><strong>E</strong></td><td>Backup Distribution panel</td><td align="center"><strong>F</strong></td><td>Backup Household loads</td></tr><tr><td align="center"><strong>G</strong></td><td>Generator</td><td align="center"><strong>H</strong></td><td>Smart loads</td><td align="center"><strong>I</strong></td><td>Power grid</td></tr><tr><td align="center"><strong>J</strong></td><td>mySigen</td><td align="center"><strong>K</strong></td><td>Router</td><td align="center"><strong>L</strong></td><td>Antenna</td></tr><tr><td align="center"><strong>M</strong></td><td>CommMod</td><td align="center"></td><td></td><td align="center"></td><td></td></tr></tbody></table>

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">If F (backup household load) experiences leakage, it may pose a risk of electric shock. In order to avoid this hazard, a residual current device (RCD) must be installed between the D (Gateway) and the F (backup household load).</mark>
* <mark style="color:blue;">As a backup energy source for long-term off-grid applications, thediesel generator can work in tandem with the Gateway to provide a smooth transition between PV, storage and diesel generation.</mark>
* <mark style="color:blue;">All the power equipment in the owner's home can be connected as smart loads. To ensure that this product maximizes the benefits to users, it is recommended that the high-power equipment be connected as smart loads (heat pumps, pool heaters, clothes dryers, etc.), which can be cut off when the energy storage system has low power. Other low-power equipment are connected as household loads (lights, routers, etc.)</mark>
* <mark style="color:blue;">It is recommended to use Fast Ethernet and WLAN for communication with inverters. When free 4G traffic of CommMod runs out, users must replace an SIM card.</mark>

### **Partial home backup system wiring diagram**

**Single inverter (Gateway has the circuit breaker for connecting smart load/generator)**

![](../.gitbook/assets/SSA1OV00030-单逆有智en.png)

**Single inverter (Gateway does not have the circuit breaker connected to the smart load/generator)**

![](../.gitbook/assets/SSA1OV00030-单逆无智-en.jpg)

**Multiple inverters (Gateway has the circuit breaker for connecting smart load/generator)**

![](../.gitbook/assets/SSA1OV00030-多逆有智en.png)

**Multiple inverters (Gateway does not have the circuit breaker connected to the smart load/generator)**

![](../.gitbook/assets/SSA1OV00030-多逆无智en.png)

<table><thead><tr><th width="71.6363525390625" align="center">No.</th><th>Description</th><th width="71.3636474609375" align="center">No.</th><th>Description</th><th width="71" align="center">No.</th><th>Description</th></tr></thead><tbody><tr><td align="center"><strong>A</strong></td><td>PV panel</td><td align="center"><strong>B</strong></td><td>SigenStor EC/Sigen Hybrid</td><td align="center"><strong>C</strong></td><td>SigenStor BAT</td></tr><tr><td align="center"><strong>D</strong></td><td>Gateway</td><td align="center"><strong>E1</strong></td><td>Backup Distribution panel</td><td align="center"><strong>E2</strong></td><td>Non-Backup Distribution panel</td></tr><tr><td align="center"><strong>F1</strong></td><td>Backup Household loads</td><td align="center"><strong>F2</strong></td><td>Non-Backup Household loads</td><td align="center"><strong>G</strong></td><td>Generator</td></tr><tr><td align="center"><strong>H</strong></td><td>Smart loads</td><td align="center"><strong>I</strong></td><td>Power sensor</td><td align="center"><strong>J</strong></td><td>Power grid</td></tr><tr><td align="center"><strong>K</strong></td><td>mySigen</td><td align="center"><strong>L</strong></td><td>Router</td><td align="center"><strong>M</strong></td><td>Antenna</td></tr><tr><td align="center"><strong>N</strong></td><td>CommMod</td><td align="center"></td><td></td><td align="center"></td><td></td></tr></tbody></table>

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">If E2 (non-backup distribution panel) features leakage protection, it is recommended that the rated residual operating current be greater than or equal to the number of inverters × 100 mA.</mark>
* <mark style="color:blue;">If F1 (backup household load) experiences leakage, it may pose a risk of electric shock. In order to avoid this hazard, a residual current device (RCD) must be installed between the D (Gateway) and the F1 (backup household load).</mark>
* <mark style="color:blue;">As a backup energy source for long-term off-grid applications, the diesel generator can work in tandem with the Gateway to provide a smooth transition between PV, storage and diesel power generation.</mark>
* <mark style="color:blue;">All the power equipment in the owner's home can be connected as smart loads. To ensure that this product maximizes the benefits to users, it is recommended that the high-power equipment be connected as smart loads (heat pumps, pool heaters, clothes dryers, etc.), which can be cut off when the energy storage system has low power. Other low-power equipment are connected as household loads (lights, routers, etc.)</mark>
* <mark style="color:blue;">Power sensor has the function of data acquisition for grid connection points enables zero-power grid connection. For partial home backup</mark> <mark style="color:blue;">system wiring, Power sensor does not need to be configured. For partial backup power and zero-power grid connection control system wiring, Power sensor is configured.</mark>
* <mark style="color:blue;">It is recommended to use Fast Ethernet and WLAN for communication with inverters. When free 4G traffic of CommMod runs out, users must replace an SIM card.</mark>
