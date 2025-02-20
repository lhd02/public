# Typical System Wiring

### (PV) Storage and Charging System Wiring

<figure><img src="../.gitbook/assets/zuwang_a.png" alt=""><figcaption></figcaption></figure>

| No.    | Description            | No.    | Description                             | No.    | Description                         |
| ------ | ---------------------- | ------ | --------------------------------------- | ------ | ----------------------------------- |
| **A**  | Solar Panel            | **B**  | SigenStor EC/ SigenStor AC/Sigen Hybrid | **C**  | SigenStor EVDC                      |
| **D**  | SigenStor BAT          | **E**  | Diesel Generator                        | **F**  | Gateway                             |
| **G**  | Vehicle                | **H1** | Backup Power Distribution Panel         | **H2** | Non-backup Power Distribution Panel |
| **I1** | Backup Power Equipment | **I2** | Non-backup Power Equipment              | **J**  | Power Sensor                        |
| **K**  | Power Grid             | **L**  | mySigen                                 | **M**  | Router                              |
| **N**  | Antenna                | **O**  | CommMod                                 |        |                                     |

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">When B is SigenStor AC, A is not configured.</mark>
* <mark style="color:blue;">J features data collection from grid-connected points to realize zero power grid connection. For partial backup, J can be left un-configured. In the case of partial backup + zero-power grid connection control, J is configured.</mark>
* <mark style="color:blue;">As a backup energy source for long-term off-grid applications, the diesel generator can work in tandem with the Gateway to provide a smooth transition between PV, energy storage, and diesel power generation.</mark>
* <mark style="color:blue;">If H2 (Non-backup Power Distribution Panel) features leakage protection, it is recommended that the rated residual operating current be greater than or equal to the number of inverters × 100 mA.</mark>
* <mark style="color:blue;">If I1 (Backup Power Equipment) experiences leakage, it may pose a risk of electric shock. In order to avoid this hazard, a residual current device (RCD) must be installed between the F (Gateway) and the I1 (Backup Power Equipment).</mark>
* <mark style="color:blue;">It is recommended to use Fast Ethernet and WLAN for communication with inverters. When free 4G traffic of Sigen CommMod runs out, users must top up their accounts or replace an SIM card.</mark>

### PV and Charging System Wiring

<figure><img src="../.gitbook/assets/zuwang_b.png" alt=""><figcaption></figcaption></figure>

| No.   | Description | No.   | Description     | No.   | Description        |
| ----- | ----------- | ----- | --------------- | ----- | ------------------ |
| **A** | Solar Panel | **B** | Sigen Hybrid    | **C** | SigenStor EVDC     |
| **D** | AC switch   | **E** | Power Equipment | **F** | Distribution Panel |
| **G** | Vehicle     | **H** | Power Sensor    | **I** | Power Grid         |
| **J** | mySigen     | **K** | Router          | **L** | Antenna            |
| **M** | CommMod     |       |                 |       |                    |

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">If F (Distribution Panel) features leakage protection, it is recommended that the rated residual operating current be greater than or equal to the number of inverters × 100 mA.</mark>
* <mark style="color:blue;">It is recommended to use Fast Ethernet and WLAN for communication with inverters. When free 4G traffic of Sigen CommMod runs out, users must top up their accounts or replace an SIM card.</mark>
