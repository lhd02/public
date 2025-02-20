# 典型组网介绍

## **（光）储充组网**

<figure><img src="../.gitbook/assets/zuwang_a.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th>序号</th><th>说明</th><th>序号</th><th width="152">说明</th><th>序号</th><th>说明</th></tr></thead><tbody><tr><td><strong>A</strong></td><td>光伏板</td><td><strong>B</strong></td><td>SigenStor EC /<br>SigenStor AC /<br>Sigen Hybrid</td><td><strong>C</strong></td><td>SigenStor EVDC</td></tr><tr><td><strong>D</strong></td><td>SigenStor BAT</td><td><strong>E</strong></td><td>柴油发电机</td><td><strong>F</strong></td><td>思格能源备电柜（Gateway）</td></tr><tr><td><strong>G</strong></td><td>车辆</td><td><strong>H1</strong></td><td>备电配电单元</td><td><strong>H2</strong></td><td>非备电配电单元</td></tr><tr><td><strong>I1</strong></td><td>备电用电设备</td><td><strong>I2</strong></td><td>非备电用电设备</td><td><strong>J</strong></td><td>思格功率传感器</td></tr><tr><td><strong>K</strong></td><td>电网</td><td><strong>L</strong></td><td>思格云</td><td><strong>M</strong></td><td>路由器</td></tr><tr><td><strong>N</strong></td><td>天线</td><td><strong>O</strong></td><td>思格通信棒（CommMod）</td><td></td><td></td></tr></tbody></table>

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">B为SigenStor AC时，A不配置。</mark>
* <mark style="color:blue;">J具备并网点数据采集实现零功率并网功能。仅部分备电时，J可不配置；部分备电+零功率并网控制时，J配置。</mark>
* <mark style="color:blue;">柴油发电机可作为长期离网场景的备份能源，与Gateway配合可实现光储柴无缝切换的用电体验。</mark>
* <mark style="color:blue;">若H2（非备电配电单元）具有漏电保护功能，推荐额定剩余动作电流为≥逆变器数量×100mA。</mark>
* <mark style="color:blue;">I1（备电家用负载）发生漏电可能导致电击危险，为避免电击危险，F（Gateway）与I1（备电家用负载）间必须安装漏电保护开关。</mark>
* <mark style="color:blue;">通信方式推荐采用FE和WLAN。Sigen CommMod赠送4G流量用完后，需用户自行充值或更换SIM卡。</mark>

### **光充组网**

<figure><img src="../.gitbook/assets/zuwang_b.png" alt=""><figcaption></figcaption></figure>

| 序号    | 说明      | 序号    | 说明           | 序号    | 说明             |
| ----- | ------- | ----- | ------------ | ----- | -------------- |
| **A** | 光伏板     | **B** | Sigen Hybrid | **C** | SigenStor EVDC |
| **D** | 交流开关    | **E** | 用电设备         | **F** | 配电单元           |
| **G** | 车辆      | **H** | 功率传感器        | **I** | 电网             |
| **J** | 思格云     | **K** | 路由器          | **L** | 天线             |
| **M** | CommMod |       |              |       |                |

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">若F（配电单元）具有漏电保护功能，推荐额定剩余动作电流为≥逆变器数量×100mA。</mark>
* <mark style="color:blue;">通信方式推荐采用FE和WLAN。Sigen CommMod赠送4G流量用完后，需用户自行充值或更换SIM卡。</mark>
