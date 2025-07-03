# 充电模式设置

![](<../../.gitbook/assets/MSA1CM00051-充电模式-zh (2).png>)

### **快速充电**

* SigenStor EVDC以最大充电功率（“EVDC允许充电功率”设置值），车辆快速充电至“车辆充电截止SOC”值（参见[充电设置](evdc-yun-xu-chong-dian-gonglshe-zhi.md)章节），充电速度最快。
* 本模式下，SigenStor EVDC默认充电功率来源优先级为：光伏发电功率→电池包放电功率→电网买入功率。其中，电池包是否放电，您可通过“电池增强”设置。设置为<img src="../../.gitbook/assets/image.png" alt="" data-size="line">时，允许电池放电供SigenStor EVDC给车辆充电，且可设置放电的截止SOC值。当设置为<img src="../../.gitbook/assets/image (1).png" alt="" data-size="line">或电池放电至设置的截止SOC值，SigenStor EVDC不允许从电池包获取充电功率。

<sub>**举例：**</sub><sub>SigenStor“工作模式”为“最大自发自用”，SigenStor含有2个电池包，每个电池包额定放电功率为4kW,SigenStor EVDC额定充电功率为25kW，“电池增强”设置为</sub><img src="../../.gitbook/assets/image.png" alt="" data-size="line">，<sub>放电的截止SOC设置为0%。在不同光照情况下，功率分配：</sub>

| 光伏发电功率 | 电池包功率  | 负载消耗功率 | 电网补电功率 | 直流桩充电功率 |
| ------ | ------ | ------ | ------ | ------- |
| 0kW    | 放电：8kW | 6kW    | 23kW   | 25kW    |
| 23kW   | 放电：8kW | 6kW    | 0kW    | 25kW    |
| 31kW   | 0kW    | 6kW    | 0kW    | 25kW    |
| 35kW   | 充电：4kW | 6kW    | 0kW    | 25kW    |

### **光伏盈余充电**

{% include "../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">**SigenStor EVDC无法在夜间使用本模式启动充电，请在白天使用本模式。**</mark>

* 光伏发电满足负载用电后，光伏剩余功率供给设备充电，您可通过拖动“光伏盈余优先级”菜单下的设备，设置使用光伏剩余功率的优先级（优先级为从上往下）。
* 当设置使用光伏剩余功率SigenStor EVDC优先于电池包，且“电池增强”设置为<img src="../../.gitbook/assets/image.png" alt="" data-size="line">时，允许电池包放电，光伏剩余功率+电池包放电一同供给SigenStor EVDC为车辆充电。当电池包放电至设置的截止SOC值时，电池包停止放电。

<sub>**举例：**</sub><sub>SigenStor“工作模式”为“最大自发自用”，SigenStor含有2个电池包，每个电池包额定放电功率为4kW,SigenStor EVDC额定充电功率为25kW，“电池增强”设置为</sub><img src="../../.gitbook/assets/image (1).png" alt="" data-size="line"><sub>。在不同光照情况下，功率分配：</sub>

| 光伏发电功率 | 电池包功率  | 负载消耗功率 | 电网补电功率 | 直流桩充电功率 |
| ------ | ------ | ------ | ------ | ------- |
| 0kW    | 放电：6kW | 6kW    | 0kW    | 0kW     |
| 6kW    | 0kW    | 6kW    | 0kW    | 0kW     |
| 16kW   | 0kW    | 6kW    | 0kW    | 10kW    |
| 31kW   | 0kW    | 6kW    | 0kW    | 25kW    |
| 35kW   | 充电：4kW | 6kW    | 0kW    | 25kW    |

{% include "../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">**“电池增强”仅设置电池包是否放给SigenStor EVDC。**</mark>
