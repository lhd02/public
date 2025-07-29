# 削峰模式

{% include "../.gitbook/includes/tips.md" %}

* 某些地区的电费计算方式为：总电费 = 峰值功率费用 + 用电电量费用 + 其它费用。其中，峰值功率指的是从电网取电的最大功率值。该模式适用于有峰谷电价且价差较大的区域。
* <mark style="color:blue;">削峰功能</mark>功能可以配合所有工作模式使用，通过配置从电网取电最大峰值功率，降低高峰期电网取电最大峰值功率，降低用电费用。

### **案例一：在最大自发自用模式下设置削峰** <a href="#an-li-yi-selfconsumption-she-zhi-peak-shaving" id="an-li-yi-selfconsumption-she-zhi-peak-shaving"></a>

假设设置的削峰SOC为50%，最大峰值功率为2kW。

因为总电费 = 峰值功率费用 + 用电电量费用 + 其它费用。其中，峰值功率指的是从电网取电的最大功率值。最大自发自用模式设置削峰后，电网购电功率从5kW下降到2kW，所以总电费降低了。

<figure><img src="../.gitbook/assets/MSA1OV00007-zh.png" alt=""><figcaption></figcaption></figure>

### **案例二：在基于时间的控制模式下设置削峰** <a href="#an-li-er-timebased-control-she-zhi-peak-shaving" id="an-li-er-timebased-control-she-zhi-peak-shaving"></a>

假设设置的削峰SOC为50%，最大峰值功率为2kW。

因为总电费 = 峰值功率费用 + 用电电量费用 + 其它费用。其中，峰值功率指的是从电网取电的最大功率值。基于时间的控制模式设置削峰后，电网购电功率从5kW下降到2kW，所以总电费降低了。

<figure><img src="../.gitbook/assets/MSA1OV00008-zh.png" alt=""><figcaption></figcaption></figure>
