# 典型组网介绍

* 本公司产品可用于家庭储能系统。家庭储能系统由光伏板、逆变器、电池包、总控制开关、思格能源备电柜、负载、电网等组成。
* 家庭储能系统主要功能是将光伏板产生的直流电存储到电池包中，也可以将光伏与电池包中的电转化成交流电提供给负载使用或并入电网。

{% include ".gitbook/includes/tips.md" %}

<mark style="color:blue;">备电组网下，备电负载离网运行时长与光储系统供电能力相关，若离网运行时，光储系统供电出现异常（包含但不限于光伏发电异常、电池电量不足、油机等供电源异常），备电负载依然存在无法运行情况。</mark>

### **组网图（全屋备电）**

<figure><img src=".gitbook/assets/SSA1OV00029-zh.jpg" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="74">序号</th><th width="151.9090576171875">说明</th><th width="72.5455322265625">序号</th><th width="154.1817626953125">说明</th><th width="56.1817626953125">序号</th><th>说明</th></tr></thead><tbody><tr><td><strong>A</strong></td><td>光伏板</td><td><strong>B</strong></td><td>思格能源控制器</td><td><strong>C</strong></td><td>思格储能电池</td></tr><tr><td><strong>D</strong></td><td>思格能源备电柜</td><td><strong>E</strong></td><td>备电配电单元</td><td><strong>F</strong></td><td>备电家用负载</td></tr><tr><td><strong>G</strong></td><td>柴油发电机</td><td><strong>H</strong></td><td>智能负载</td><td><strong>I</strong></td><td>电网</td></tr><tr><td><strong>J</strong></td><td>思格云</td><td><strong>K</strong></td><td>路由器</td><td><strong>L</strong></td><td>天线棒</td></tr><tr><td><strong>M</strong></td><td>思格通信棒</td><td></td><td></td><td></td><td></td></tr></tbody></table>

{% include ".gitbook/includes/tips.md" %}

* <mark style="color:blue;">柴油发电机可作为长期离网场景的备份能源，与思格能源备电柜配合可实现光储柴无缝切换的用电体验。</mark>
* <mark style="color:blue;">业主家中的用电设备均可作为智能负载接入。为保证本产品对用户利益最大化，建议大功率设备作为智能负载接入（如热泵、泳池加热器、干衣机等），当储能电量不足时可切出。其他小功率设备作为家用负载接入（如灯、路由器等）。</mark>
* <mark style="color:blue;">通信方式推荐采用FE和WLAN。思格通信棒赠送4G流量用完后，需用户自行充值或更换SIM卡。</mark>

### **组网图（部分备电）**

<figure><img src=".gitbook/assets/SSA1OV00030-zh.jpg" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="68.6363525390625">序号</th><th>说明</th><th width="70.727294921875">序号</th><th>说明</th><th width="93.8182373046875">序号</th><th>说明</th></tr></thead><tbody><tr><td><strong>A</strong></td><td>光伏板</td><td><strong>B</strong></td><td>思格能源控制器</td><td><strong>C</strong></td><td>思格储能电池</td></tr><tr><td><strong>D</strong></td><td>思格能源备电柜</td><td><strong>E1</strong></td><td>备电配电单元</td><td><strong>E2</strong></td><td>非备电配电单元</td></tr><tr><td><strong>F1</strong></td><td>备电家用负载</td><td><strong>F2</strong></td><td>非备电家用负载</td><td><strong>G</strong></td><td>柴油发电机</td></tr><tr><td><strong>H</strong></td><td>智能负载</td><td><strong>I</strong></td><td>功率传感器</td><td><strong>J</strong></td><td>电网</td></tr><tr><td><strong>K</strong></td><td>思格云</td><td><strong>L</strong></td><td>路由器</td><td><strong>M</strong></td><td>天线棒</td></tr><tr><td><strong>N</strong></td><td>思格通信棒</td><td></td><td></td><td></td><td></td></tr></tbody></table>

{% include ".gitbook/includes/tips.md" %}

* <mark style="color:blue;">柴油发电机可作为长期离网场景的备份能源，与思格能源备电柜配合可实现光储柴无缝切换的用电体验。</mark>
* <mark style="color:blue;">业主家中的用电设备均可作为智能负载接入。为保证本产品对用户利益最大化，建议大功率设备作为智能负载接入（如热泵、泳池加热器、干衣机等），当储能电量不足时可切出。其他小功率设备作为家用负载接入（如灯、路由器等）。</mark>
* <mark style="color:blue;">功率传感器具备并网点数据采集实现零功率并网功能。仅部分备电时，功率传感器可不配置；部分备电+零功率并网控制时，功率传感器需配置。</mark>
* <mark style="color:blue;">通信方式推荐采用FE和WLAN。思格通信棒赠送4G流量用完后，需用户自行充值或更换SIM卡。</mark>

### **组网图（非备电组网）**

<figure><img src=".gitbook/assets/SSA1OV00031-ZH.jpg" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="73.45458984375">序号</th><th width="150.181884765625">说明</th><th width="62.181884765625">序号</th><th>说明</th><th width="86.45458984375">序号</th><th>说明</th></tr></thead><tbody><tr><td><strong>A</strong></td><td>光伏板</td><td><strong>B</strong></td><td>思格能源控制器</td><td><strong>C</strong></td><td>思格储能电池</td></tr><tr><td><strong>D</strong></td><td>交流开关</td><td><strong>E</strong></td><td>配电单元</td><td><strong>F</strong></td><td>家用负载</td></tr><tr><td><strong>G</strong></td><td>功率传感器</td><td><strong>H</strong></td><td>电网</td><td><strong>I</strong></td><td>思格云</td></tr><tr><td><strong>J</strong></td><td>路由器</td><td><strong>K</strong></td><td>天线棒</td><td><strong>L</strong></td><td>思格通信棒</td></tr></tbody></table>

{% include ".gitbook/includes/tips.md" %}

* <mark style="color:blue;">与每一台逆变器连接的交流开关额定电压均需 ≥380 Va.c., 额定电流推荐规格：</mark>
  * <mark style="color:blue;">SigenStor EC (5.0-8.0) TP：额定电流为25A</mark>
  * <mark style="color:blue;">SigenStor EC (10.0-15.0) TP：额定电流为32A</mark>
  * <mark style="color:blue;">SigenStor EC (17.0-20.0) TP：额定电流为40A</mark>
  * <mark style="color:blue;">SigenStor EC 25.0 TP：额定电流为50A</mark>
* <mark style="color:blue;">通信方式推荐采用FE和WLAN。思格通信棒赠送4G流量用完后，需用户自行充值或更换SIM卡。</mark>
* <mark style="color:blue;">配电单元的交流开关额定电压需 ≥380 Va.c., 额定电流需：≥ 逆变器最大输出电流 x 并机数量 x 1.25【1】</mark>

注【1】：逆变器最大输出电流可在产品《思格产品参数》上获取。
