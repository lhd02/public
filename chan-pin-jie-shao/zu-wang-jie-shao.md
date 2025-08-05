# Introduction to system wiring

* This product is applicable to household backup power system networking scenarios. It must be used in conjunction with PV panels, inverters, battery packs, main control switches, loads, generators, and power grid.
* In the event of a power outage, the household energy storage system switches to off-grid operation mode. After the power grid resumes normal operation, the household energy storage system switches back to on-grid mode. This achieves a seamless switchover between PV storage and Generator.

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">Under backup power networking, the duration of off-grid operation of the backup power load is related to the power supply capacity of the PV storage system. If there is an abnormality in the power supply of the PV storage system during off-grid operation (including but not limited to abnormal PV power generation, insufficient battery power, and abnormal power supplies to the Generator), the backup power load will still be unable to operate.</mark>
* <mark style="color:blue;">The networking diagram takes two inverters as an example. The number of inverters that can be connected depends on the Gateway specification. For more information, see Table 2-1.</mark>

**Table 2-1**

<table><thead><tr><th width="50" align="center">S/N</th><th width="204">Model</th><th>Number of Inverters that can be connected</th></tr></thead><tbody><tr><td align="center">1</td><td>Sigen Gateway TPLV C30-2</td><td>2 units</td></tr><tr><td align="center">2</td><td>Sigen Gateway C60-2</td><td>2 units</td></tr><tr><td align="center">3</td><td>Sigen Gateway C60 AU</td><td>2 units</td></tr><tr><td align="center">4</td><td>Sigen Gateway TPLV C70-6</td><td>6 units</td></tr><tr><td align="center">5</td><td>Sigen Gateway C120-6</td><td>6 units</td></tr><tr><td align="center">6</td><td>Sigen Gateway C180-9</td><td>9 units</td></tr><tr><td align="center">7</td><td>Sigen Gateway C300-12</td><td>12 units</td></tr><tr><td align="center">8</td><td>Sigen Gateway C600</td><td>30 units</td></tr><tr><td align="center">9</td><td>Sigen Gateway C1200</td><td>50 units</td></tr><tr><td align="center">10</td><td>Sigen Gateway C600-B</td><td>10 units</td></tr><tr><td align="center">11</td><td>Sigen Gateway C1200-B</td><td>20 units</td></tr></tbody></table>

### **Whole home backup system wiring diagram**

**Single inverter (Gateway has the circuit breaker for connecting smart load/diesel generator)**

<figure><img src="../.gitbook/assets/SSA1OV00029-单逆-en (2).jpg" alt=""><figcaption></figcaption></figure>

**Single inverter (Gateway does not have the circuit breaker connected to the smart load/diesel generator)**

<figure><img src="../.gitbook/assets/SSA1OV00029-单逆无智-en.jpg" alt=""><figcaption></figcaption></figure>

### **Multiple inverters (Gateway has the circuit breaker for connecting smart load/diesel generator)**

<figure><img src="../.gitbook/assets/SSA1OV00029-多逆有智en.png" alt=""><figcaption></figcaption></figure>

### **Multiple inverters (Gateway does not have the circuit breaker connected to the smart load/diesel generator)**

<figure><img src="../.gitbook/assets/SSA1OV00029-多逆无智en.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="64" align="center">No.</th><th width="114">Description</th><th width="65" align="center">No.</th><th width="295">Description</th><th width="63">No.</th><th>Description</th></tr></thead><tbody><tr><td align="center"><strong>A</strong></td><td>PV panel</td><td align="center"><strong>B</strong></td><td>SigenStor EC/Sigen Hybrid</td><td><strong>C</strong></td><td>SigenStor BAT</td></tr><tr><td align="center"><strong>D</strong></td><td>Gateway</td><td align="center"><strong>E</strong></td><td>Backup Distribution panel</td><td><strong>F</strong></td><td>Backup Household loads</td></tr><tr><td align="center"><strong>G</strong></td><td>Diesel generator</td><td align="center"><strong>H</strong></td><td>Smart loads</td><td><strong>I</strong></td><td>Power grid</td></tr><tr><td align="center"><strong>J</strong></td><td>mySigen</td><td align="center"><strong>K</strong></td><td>Router</td><td><strong>L</strong></td><td>Antenna</td></tr><tr><td align="center"><strong>M</strong></td><td>CommMod</td><td align="center"></td><td></td><td></td><td></td></tr></tbody></table>

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">If F (backup household load) experiences leakage, it may pose a risk of electric shock. In order to avoid this hazard, a residual current device (RCD) must be installed between the D (Gateway) and the F (backup household load).</mark>
* <mark style="color:blue;">As a backup energy source for long-term off-grid applications, the diesel generator can work in tandem with the Gateway to provide a smooth transition between PV, storage and diesel generation.</mark>
* <mark style="color:blue;">All the power equipment in the owner's home can be connected as smart loads. To ensure that this product maximizes the benefits to users, it is recommended that the high-power equipment be connected as smart loads (heat pumps, pool heaters, clothes dryers, etc.), which can be cut off when the energy storage system has low power. Other low-power equipment are connected as household loads (lights, routers, etc.)</mark>
* <mark style="color:blue;">It is recommended to use Fast Ethernet and WLAN for communication with inverters. When free 4G traffic of CommMod runs out, users must replace an SIM card.</mark>

### **Partial home backup system wiring diagram**

### **Single inverter (Gateway has the circuit breaker for connecting smart load/diesel generator)**

<figure><img src="../.gitbook/assets/SSA1OV00030-单逆-en.jpg" alt=""><figcaption></figcaption></figure>

### **Single inverter (Gateway does not have the circuit breaker connected to the smart load/diesel generator)**

<figure><img src="../.gitbook/assets/SSA1OV00030-单逆无智-en.jpg" alt=""><figcaption></figcaption></figure>

### **Multiple inverters (Gateway has the circuit breaker for connecting smart load/diesel generator)**

<figure><img src="../.gitbook/assets/SSA1OV00030-EN (1).jpg" alt=""><figcaption></figcaption></figure>

### **Multiple inverters (Gateway does not have the circuit breaker connected to the smart load/diesel generator)**

<figure><img src="../.gitbook/assets/SSA1OV00030-多逆无智en.png" alt=""><figcaption></figcaption></figure>

| No.    | Description            | No.    | Description                             | No.    | Description                   |
| ------ | ---------------------- | ------ | --------------------------------------- | ------ | ----------------------------- |
| **A**  | PV panel               | **B**  | SigenStor EC/SigenStor AC /Sigen Hybrid | **C**  | SigenStor BAT                 |
| **D**  | Gateway                | **E1** | Backup Distribution panel               | **E2** | Non-Backup Distribution panel |
| **F1** | Backup Household loads | **F2** | Non-Backup Household loads              | **G**  | Diesel Generator              |
| **H**  | Smart loads            | **I**  | Power sensor                            | **J**  | Power grid                    |
| **K**  | mySigen                | **L**  | Router                                  | **M**  | Antenna                       |
| **N**  | CommMod                |        |                                         |        |                               |

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">If E2 (non-backup distribution panel) features leakage protection, it is recommended that the rated residual operating current be greater than or equal to the number of inverters × 100 mA.</mark>
* <mark style="color:blue;">If F1 (backup household load) experiences leakage, it may pose a risk of electric shock. In order to avoid this hazard, a residual current device (RCD) must be installed between the D (Gateway) and the F1 (backup household load).</mark>
* <mark style="color:blue;">As a backup energy source for long-term off-grid applications, the diesel generator can work in tandem with the Gateway to provide a smooth transition between PV, storage and diesel power generation.</mark>
* <mark style="color:blue;">All the power equipment in the owner's home can be connected as smart loads. To ensure that this product maximizes the benefits to users, it is recommended that the high-power equipment be connected as smart loads (heat pumps, pool heaters, clothes dryers, etc.), which can be cut off when the energy storage system has low power. Other low-power equipment are connected as smart loads (heat pumps, pool heaters, clothes dryers, etc.), which can be cut off when the energy storage system has low power. Other low-power equipment are connected as household loads (lights, routers, etc.)</mark>
* <mark style="color:blue;">Power sensor has the function of data acquisition for grid connection points enables zero-power grid connection. For partial home backup system wiring, Power sensor does not need to be configured. For partial backup power and zero-power grid connection control system wiring , Power sensor is configured.</mark>
* <mark style="color:blue;">It is recommended to use Fast Ethernet and WLAN for communication with inverters. When free 4G traffic of CommMod runs out, users must replace an SIM card.</mark>
