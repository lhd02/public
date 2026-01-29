# Sigen EV AC Charger Settings

{% include "../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">In pure charging scenarios, only one Sigen EV AC Charger can be connected. In PV charging or PV storage scenarios, one SigenStor can connect up to two Sigen EV AC Chargers.</mark>

## **Pure charging application**

<figure><img src="../../.gitbook/assets/MSA1CM00079-纯充EVAC (2).png" alt="" width="563"><figcaption></figcaption></figure>

## **PV charging or PV storage & charging application**

{% include "../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">To connect a Sigen EV AC Charger, you need to connect the FE network cable to SigenStor.</mark>
* <mark style="color:blue;">To connect two Sigen EV AC Chargers, you need to connect them to the same WLAN network as SigenStor. For the steps to add them, refer to</mark> [Post-Sales service.](../../station-parameter-setup/installer-tool/after-sales-service.md)

<figure><img src="../../.gitbook/assets/MSA1CM00078-EVAC参数设置.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="154.8887939453125">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td>Schedule</td><td>If the connected car supports the scheduled Charging function, you can set the scheduled charging and discharging periods.</td></tr></tbody></table>

## **Charging Preference** <a href="#charging-preference" id="charging-preference"></a>

<table><thead><tr><th width="72" align="center">No.</th><th width="154.8887939453125">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td align="center">1</td><td>Charging Record</td><td>You can view the charging records.</td></tr><tr><td align="center">2</td><td>Charging Mode</td><td><ol><li><strong>Fast Charging</strong></li><li><strong>PV Surplus Charging</strong></li><li><strong>Sigen AI Mode</strong>（To use this mode, please refer to the activation steps for <a href="optional-sigen-ev-ac-charger-activates-sigen-ai-mode.md">Sigen EV AC Charger activates Sigen AI Mode</a>.）</li></ol><ul><li>Battery Boost: When set to<img src="../../.gitbook/assets/image (2).png" alt=""> , it allows charging from the home battery.</li><li>Cut-OFF SOC: When Battery Boost is enabled, the battery will stop charging the Sigen EV AC charger if the actual SOC is less than the set parameter.</li><li>Grid Charging: When set to<img src="../../.gitbook/assets/image (2).png" alt=""> , it allows setting the rated power of the connected device.</li><li>The maximum power from the grid: In PV surplus charging mode, this value indicates the maximum power that can be drawn from the grid when PV power is insufficient.</li><li>Surplus PV priority: If this parameter is set, it will redirect to the priority page for PV power generation.</li></ul><p></p><ul><li>By integrating local peak/off-peak electricity prices, weather data, and user consumption habits, it provides customized smart charging solutions and enables intelligent scheduling throughout the entire charging process, maximizing cost savings and delivering a convenient experience for users.</li></ul></td></tr><tr><td align="center">3</td><td>OCPP Setting</td><td><ul><li>OCPP Status: Display explicit OCPP connection status.</li><li>When it is set to <img src="../../.gitbook/assets/image (2).png" alt="">, Sigen EV AC Charger can be connected to the OCPP server, and users can select the OCPP platform from the URL drop-down list.</li></ul></td></tr><tr><td align="center">4</td><td>Authorization</td><td>Set the charging authentication. When it is set to <img src="../../.gitbook/assets/image (1) (1) (2).png" alt="">, unauthenticated charging is allowed.</td></tr><tr><td align="center">5</td><td>Card Management</td><td>Bind a Sigen RFID card.</td></tr><tr><td align="center">6</td><td>Advanced Mode</td><td><ul><li>Output Mode: Select single-phase or three-phase output as needed.</li><li>P1 Connected to: When the Output Mode is set to single-phase, you can set which phase P1 is connected to.</li><li>Dynamic load management: When Power Sensor is installed in the networking and is not in off-grid state, and if it is set to <img src="../../.gitbook/assets/image (2).png" alt="">, Sigen EV AC Charger will support dynamic load management (DLM). Sigen EV AC Charger quickly and intelligently regulates the charging current (power) by comparing the power at the grid-connection point reported by the Power Sensor with the "Rated Household Circuit Breaker Current" set by the installer when creating new systems to prevent the Household Circuit Breaker in the distribution panel from being disconnected.</li><li>Home air circuit breaker rated current: The current specification of the household circuit breaker controls the charging power of the AC pile so that the household current is less than the set value.</li><li>Allow charging when off-grid: When it is set to <img src="../../.gitbook/assets/image (2).png" alt="">, charging is allowed during off-grid operation.</li></ul></td></tr><tr><td align="center">7</td><td>Indicator Settings</td><td>Click to set the LED light on/off for the Sigen EV AC Charger.</td></tr><tr><td align="center">8</td><td>Connectivity</td><td><p><strong>Ethernet</strong></p><ul><li>Displays the connection status of Fast Ethernet.</li><li>For Fast Ethernet, network parameters are automatically obtained using a DHCP server. To edit parameters, do the following:</li></ul><ol><li>Configure a WLAN that can access the internet or insert a 4G SIM card.</li><li>Wait until "WLAN" or "Cellular" is displayed as "Connected,” and disconnect the network cable.</li><li>Set "Obtain IP address automatically" to <img src="../../.gitbook/assets/image (1) (1) (2).png" alt="">and edit parameters.</li><li>Re-connect the network cable to the device.</li></ol><p><strong>WLAN</strong></p><p>Displays the connection status of WLAN. If the connection status is displayed as "Not connected" and you want to use the WLAN to access internet, select a WLAN hotspot supporting 2.4 GHz band.</p><p>Notes:</p><ul><li>Non-encrypted WLAN is not recommended as it may lead to Internet access failure.</li><li>When WLAN is the only connection path for the devices to access the internet, switching WLAN to any other wireless router will be prohibited.</li></ul><p><strong>Cellular</strong></p><ul><li>Displays the connection status of 4G network. If the connection status is displayed as "Not connected," and you want to use the 4G network to access the internet, ensure that you insert the 4G SIM card.</li><li>When 4G is used for communication, users can view the monthly traffic usage and set a traffic usage threshold for each month.</li></ul></td></tr></tbody></table>

## **Charger Settings** <a href="#charger-settings" id="charger-settings"></a>

<table><thead><tr><th width="76" align="center">No.</th><th width="183.2222900390625">Parameter name</th><th>Description</th></tr></thead><tbody><tr><td align="center">1</td><td>Grid Code</td><td>Specifies a grid code based on the country/region when devices are used.</td></tr><tr><td align="center">2</td><td>Ground mode</td><td>Specifies the grounding type according to local grid type.</td></tr><tr><td align="center">3</td><td>Home air circuit breaker</td><td>Specifies the rated current according to the home main incoming circuit breaker within the distribution panel.</td></tr><tr><td align="center">4</td><td>Input circuit breaker rated current</td><td>Specifies the rated current according to circuit breakers connected to devices in the distribution panel.</td></tr><tr><td align="center">5</td><td>Charging pile type</td><td>You can choose the charging pile type.</td></tr><tr><td align="center">6</td><td>Phase Type</td><td>Specifies the phase type according to actual wiring.</td></tr><tr><td align="center">7</td><td>Maintenance</td><td><ul><li>Reset: The device restarts.</li><li>This will clear 5-minute performance data, alarms, hourly/daily/monthly/annual power generation records, operation logs, device information, etc. Proceed with caution.</li></ul></td></tr><tr><td align="center">8</td><td>Modbus Settings</td><td>Modbus Native (Slave) Address: Click to set the Modbus slave address.</td></tr></tbody></table>

{% include "../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">For use and precautions of the Sigen EV AC Charger, refer to the Sigen EV AC Charger User Manual.</mark>

## Charging Current Adjustment

{% include "https://app.gitbook.com/s/YEsgDWDFgclMJZqvpmZf/~/reusable/dnF8ucRZR0FwUqCpci9l/" %}

<mark style="color:blue;">A higher output current value results in greater charging power.</mark>

### Manual Adjustment

<figure><img src="../../.gitbook/assets/SSA1CM00069-充电电流调整.jpg" alt="" width="563"><figcaption></figcaption></figure>

### **DLM Automatic Adjustment**

{% include "https://app.gitbook.com/s/YEsgDWDFgclMJZqvpmZf/~/reusable/dnF8ucRZR0FwUqCpci9l/" %}

<mark style="color:blue;">Power Sensor must be installed in the system station.</mark>

<figure><img src="../../.gitbook/assets/SSA1CM00069-DLM.jpg" alt="" width="563"><figcaption></figcaption></figure>

## Charging/Stop Charging Settings

### **Pure Charging Scenario**

Click "START" or "STOP" on the "Home" interface.

### **PV Charging or PV+Storage+Charging Scenario**

Click "AC Charger" on the "Device" interface, then click "START" or "STOP".
