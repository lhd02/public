# Peak Shaving

{% include "https://app.gitbook.com/s/ZGNxOhPbnqkITg7JQHuh/~/reusable/AxOnSdThcis4NCgqEO8Z/" %}

* <mark style="color:blue;">某些地区的电费计算方式为：总电费 = 峰值功率费用 + 用电电量费用 + 其它费用。其中，峰值功率指的是从电网取电的最大功率值。该模式适用于有峰谷电价且价差较大的区域。</mark>
* <mark style="color:blue;">Peak Shaving功能可以配合所有工作模式使用，通过配置从电网取电最大峰值功率，降低高峰期电网取电最大峰值功率，降低用电费用。</mark>

### 案例一：Self-Consumption设置Peak Shaving

假设Peak Shaving设置的削峰SOC为50%，最大峰值功率为2 kW。因为总电费 = 峰值功率费用 + 用电电量费用 + 其它费用。其中，峰值功率指的是从电网取电的最大功率值。Self-Consumption设置Peak Shaving后，电网购电功率从5 kW下降到2 kW，所以总电费降低了。

<figure><img src="../.gitbook/assets/MSA1OV00007-zh.png" alt=""><figcaption></figcaption></figure>

### 案例二：Time-based Control设置Peak Shaving

假设Peak Shaving设置的削峰SOC为50%，最大峰值功率为2 kW。因为总电费 = 峰值功率费用 + 用电电量费用 + 其它费用。其中，峰值功率指的是从电网取电的最大功率值。Time-based Control设置Peak Shaving后，电网购电功率从5 kW下降到2 kW，所以总电费降低了。

<figure><img src="../.gitbook/assets/MSA1OV00008-zh.png" alt=""><figcaption></figcaption></figure>
