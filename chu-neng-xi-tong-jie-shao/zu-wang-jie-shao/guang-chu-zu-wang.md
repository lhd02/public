# 光储组网

* 本公司产品可用于家庭储能系统。家庭储能系统由光伏板、逆变器、电池包、总控制开关、思格能源备电柜、负载、电网等组成。
* 家庭储能系统主要功能是将光伏板产生的直流电存储到电池包中，也可以将光伏与电池包中的电转化成交流电提供给负载使用或并入电网。

{% include "../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">备电组网下，备电负载离网运行时长与光储系统供电能力相关，若离网运行时，光储系统供电出现异常（包含但不限于光伏发电异常、电池电量不足、油机等供电源异常），备电负载依然存在无法运行情况。</mark>

## **全屋备电组网图**

<figure><img src="../../.gitbook/assets/SHA1OV00009-zh.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="59.5555419921875" align="center">序号</th><th width="128">说明</th><th width="61.111083984375" align="center">序号</th><th>说明</th><th width="60.333251953125" align="center">序号</th><th>说明</th></tr></thead><tbody><tr><td align="center"><strong>A</strong></td><td>光伏板</td><td align="center"><strong>B</strong></td><td>Sigen Hybrid</td><td align="center"><strong>C</strong></td><td>SigenStor储能系统（SigenStor BC+SigenStor BAT）</td></tr><tr><td align="center"><strong>D</strong></td><td>思格能源备电柜</td><td align="center"><strong>E</strong></td><td>备电配电单元</td><td align="center"><strong>F</strong></td><td>备电家用负载</td></tr><tr><td align="center"><strong>G</strong></td><td>柴油发电机</td><td align="center"><strong>H</strong></td><td>智能负载</td><td align="center"><strong>I</strong></td><td>电网</td></tr><tr><td align="center"><strong>J</strong></td><td>思格云</td><td align="center"><strong>K</strong></td><td>路由器</td><td align="center"><strong>L</strong></td><td>天线棒</td></tr><tr><td align="center"><strong>M</strong></td><td>CommMod</td><td align="center"></td><td></td><td align="center"></td><td></td></tr></tbody></table>

{% include "../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">Sigen Hybrid支持级联台数≤20。</mark>
* <mark style="color:blue;">Sigen Hybrid+SigenStor储能系统支持连接Sigen Hybrid+ SigenStor储能系统，也支持连接Sigen Hybrid。</mark>
* <mark style="color:blue;">F（备电家用负载）发生漏电可能导致电击危险，为避免电击危险，D（</mark>思格能源备电柜<mark style="color:blue;">）和F（备电家用负载）之间必须安装漏电保护开关。</mark>
* <mark style="color:blue;">柴油发电机可作为长期离网场景的备份能源，与Gateway配合可实现光储柴无缝切换的用电体验。</mark>
* <mark style="color:blue;">业主家中的用电设备均可作为智能负载接入。为保证本产品对用户利益最大化，建议大功率设备作为智能负载接入（如热泵、泳池加热器、干衣机等），当储能电量不足时可切出。其他小功率设备作为家用负载接入（如灯、路由器等）。</mark>
* <mark style="color:blue;">通信方式推荐采用FE和WLAN。CommMod赠送4G流量用完后，需用户自行充值或更换SIM卡。</mark>

## **部分备电组网图**

<figure><img src="../../.gitbook/assets/SHA1OV00010-zh.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="61.33331298828125" align="center">序号</th><th>说明</th><th width="60.3333740234375" align="center">序号</th><th>说明</th><th width="60.3333740234375" align="center">序号</th><th>说明</th></tr></thead><tbody><tr><td align="center"><strong>A</strong></td><td>光伏板</td><td align="center"><strong>B</strong></td><td>Sigen Hybrid</td><td align="center"><strong>C</strong></td><td>SigenStor储能系统（SigenStor BC+SigenStor BAT）</td></tr><tr><td align="center"><strong>D</strong></td><td>思格能源备电柜</td><td align="center"><strong>E1</strong></td><td>备电配电单元</td><td align="center"><strong>E2</strong></td><td>非备电配电单元</td></tr><tr><td align="center"><strong>F1</strong></td><td>备电家用负载</td><td align="center"><strong>F2</strong></td><td>非备电家用负载</td><td align="center"><strong>G</strong></td><td>柴油发电机</td></tr><tr><td align="center"><strong>H</strong></td><td>智能负载</td><td align="center"><strong>I</strong></td><td>功率传感器</td><td align="center"><strong>J</strong></td><td>电网</td></tr><tr><td align="center"><strong>K</strong></td><td>思格云</td><td align="center"><strong>L</strong></td><td>路由器</td><td align="center"><strong>M</strong></td><td>天线棒</td></tr><tr><td align="center"><strong>N</strong></td><td>CommMod</td><td align="center"></td><td></td><td align="center"></td><td></td></tr></tbody></table>

{% include "../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">Sigen Hybrid支持级联台数≤20台。</mark>
* <mark style="color:blue;">Sigen Hybrid+SigenStor储能系统支持连接Sigen Hybrid+ SigenStor储能系统，也支持连接Sigen Hybrid。</mark>
* <mark style="color:blue;">若E2 (非备电配电单元) 具有漏电保护功能，推荐额定剩余动作电流为≥逆变器数量×100mA。</mark>
* <mark style="color:blue;">F1（备电家用负载）发生漏电可能导致电击危险，为避免电击危险，D（</mark>思格能源备电柜<mark style="color:blue;">）和F1（备电家用负载）之间必须安装漏电保护开关。</mark>
* <mark style="color:blue;">柴油发电机可作为长期离网场景的备份能源，与</mark>思格能源备电柜<mark style="color:blue;">配合可实现光储柴无缝切换的用电体验。</mark>
* <mark style="color:blue;">业主家中的用电设备均可作为智能负载接入。为保证本产品对用户利益最大化，建议大功率设备作为智能负载接入（如热泵、泳池加热器、干衣机、热得快等），当储能电量不足时可切出。其他小功率设备作为家用负载接入（如灯、路由器等）。</mark>
* <mark style="color:blue;">功率传感器具备并网点数据采集实现零功率并网功能。仅部分备电时，功率传感器可不配置；部分备电+零功率并网控制时，功率传感器需配置。</mark>
* <mark style="color:blue;">通信方式推荐采用FE和WLAN。CommMod赠送4G流量用完后，需用户自行更换SIM卡。</mark>

## **非备电组网图**

<figure><img src="../../.gitbook/assets/SHA1OV00011-zh.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="60.66668701171875" align="center">序号</th><th width="128">说明</th><th width="60" align="center">序号</th><th>说明</th><th width="59.22216796875" align="center">序号</th><th>说明</th></tr></thead><tbody><tr><td align="center"><strong>A</strong></td><td>光伏板</td><td align="center"><strong>B</strong></td><td>Sigen Hybrid</td><td align="center"><strong>C</strong></td><td>SigenStor储能系统（SigenStor BC+SigenStor BAT）</td></tr><tr><td align="center"><strong>D</strong></td><td>交流开关</td><td align="center"><strong>E</strong></td><td>配电单元</td><td align="center"><strong>F</strong></td><td>家用负载</td></tr><tr><td align="center"><strong>G</strong></td><td>功率传感器</td><td align="center"><strong>H</strong></td><td>电网</td><td align="center"><strong>I</strong></td><td>mySigen</td></tr><tr><td align="center"><strong>J</strong></td><td>路由器</td><td align="center"><strong>K</strong></td><td>天线棒</td><td align="center"><strong>L</strong></td><td>CommMod</td></tr></tbody></table>

{% include "../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">Sigen Hybrid支持级联台数≤20台。</mark>
* <mark style="color:blue;">Sigen Hybrid+SigenStor储能系统支持连接Sigen Hybrid+ SigenStor储能系统，也支持连接Sigen Hybrid。</mark>
* <mark style="color:blue;">Sigen Hybrid (2.0-6.0) SP2系列：与每一台逆变器连接的交流开关额定电压均需≥240Va.c.，额定电流推荐规格：</mark>
  * <mark style="color:blue;">Sigen Hybrid (2.0-4.0) SP2系列：额定电流为25A。</mark>
  * <mark style="color:blue;">Sigen Hybrid (4.6-6.0) SP2系列：额定电流为40A。</mark>
* <mark style="color:blue;">Sigen Hybrid (3.0-12.0) TP2系列：与每一台逆变器连接的交流开关额定电压均需≥415 Va.c.，额定电流推荐规格：</mark>
  * <mark style="color:blue;">Sigen Hybrid (3.0, 4.0) TP2系列：额定电流为10A。</mark>
  * <mark style="color:blue;">Sigen Hybrid (5.0, 6.0) TP2系列：额定电流为16A。</mark>
  * <mark style="color:blue;">Sigen Hybrid (7.5, 8.0) TP2系列：额定电流为25A。</mark>
  * <mark style="color:blue;">Sigen Hybrid (10.0, 12.0) TP2系列：额定电流为32A。</mark>
* <mark style="color:blue;">若E（配电单元）具有漏电保护功能，推荐额定剩余动作电流为≥逆变器数量×100mA。</mark>
* <mark style="color:blue;">配电单元的交流开关额定电压需 ≥240Va.c., 额定电流需：≥ 逆变器最大输出电流 x 并机数量 x 1.25</mark><sup><mark style="color:blue;">【1】<mark style="color:blue;"></sup>
* <mark style="color:blue;">通信方式推荐采用FE和WLAN。Sigen CommMod赠送4G流量用完后，需用户自行充值或更换SIM卡。</mark>

<mark style="color:blue;">注【1】：逆变器最大输出电流可在产品</mark>《思格产品参数》<mark style="color:blue;">上获取。</mark>
