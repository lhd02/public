# Third-party inverter

### Method 1: **Connecting using Gateway**

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">Only third-party inverters that not support off-grid functionality are allowed to connect.</mark>
* <mark style="color:blue;">Before connecting to a third-party inverter, ensure that the third-party inverter is connected to the smart load circuit breaker of the Gateway. For connection details, refer to the Installation Guide of the respective product.</mark>
* <mark style="color:blue;">On the "Device" screen, set related parameters based on the third-party inverter. Then, you can check detailed settings on the "Device" screen.</mark>

<figure><img src="../.gitbook/assets/SSA1CM00072-gateway添加三逆.png" alt=""><figcaption></figcaption></figure>

### Method 2: **Connecting using an electric meter**

{% include "../.gitbook/includes/tips.md" %}

<mark style="color:blue;">Before connecting to a third-party inverter, make sure that:</mark>

* <mark style="color:blue;">The third-party inverter is properly connected to an electric meter which is purchased from our company.</mark>
* <mark style="color:blue;">The electric meter is properly connected to the COM port of our inverter. For connection ports, please refer to the respective Installation Guide.</mark>

<figure><img src="../.gitbook/assets/SSA1CM00072-电表添加三逆.png" alt=""><figcaption></figcaption></figure>

**Diagram of third-party inverter wiring connections**

<figure><img src="../.gitbook/assets/MSA1CM00090-en.png" alt=""><figcaption></figcaption></figure>

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">The diagram displays the connections among different cables of equipment. The specific ports shall be determined by actual equipment.</mark>
* <mark style="color:blue;">On the "Device" screen, set related parameters based on the third-party inverter and the connected meter. Then, you can check detailed settings on the "Device" screen.</mark>
* <mark style="color:blue;">In the off grid state, when the operating power of the third-party inverter is ≤ (load usage power + Sigen inverter charging power), the third-party inverter can operate normally.</mark>
* <mark style="color:blue;">In the off grid state, when the operating power of the third-party inverter is greater than (load usage power + Sigen inverter charging power), the third-party inverter will stop running.</mark>
