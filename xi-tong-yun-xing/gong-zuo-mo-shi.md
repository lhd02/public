# 工作模式

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">**能系统共有五种工作模式，分别为：Sigen AI Mode、Fully Fed to Grid Mode、Self-Consumption Mode、Time-based Control Mode、Remote EMS Mode。**</mark>
* <mark style="color:blue;">**部分国家可使用Sigen AI Mode，以App界面显式为准。**</mark>

### **Sigen AI Mode**

通过一段时间，记录用户用电习惯和当地电价的波峰波谷等数据，Sigen AI Mode可定制智能用电解决方案，最大程度为客户节约用电价格。

![](../.gitbook/assets/1.jpeg)

### **Fully Fed to Grid Mode**

可使光伏发电最大化卖给电网。白天光伏发电功率＞逆变器的最大输出能力时，逆变器保持最大输出，同时将多余电量存储在电池中；当光伏发电功率＜逆变器最大输出能力或夜间无光伏发电时，电池放电，确保逆变器能够最大化输出。

### **Self-Consumption Mode**

当太阳能充足时，光伏系统产生的电能将优先供给负载，剩余电能存储在电池中，再余电能卖给电网。当太阳能不足时，电池会释放电能供给负载。提高光伏系统的自发自用率和家庭能源自给自足率，可节省电费支出。

![](../.gitbook/assets/2.jpeg)

### **Time-based Control Mode**

Time-based Control模式需要在mySigen App中手动设置充电时段和放电时段，其余时段为非充非放时段。白天光伏发电的剩余电力可以卖给电网或者给电池充电，夜间在电网低电价时段给电池充电，可节省电费支出。

![](<../.gitbook/assets/3 (3).png>)

### **Remote EMS Mode**

设置为本模式后，将允许第三方EMS调度公司设置电站及产品的相关参数。未经安装商确认，请勿进入或退出此模式。

Backup Reserve：

组网中含有Gateway时，可在mySigen App中手动设置“Backup Reserve”值。在电网并网时，电池放电至设置的备电SOC时停止放电；在电网离网时，可以使用备电的电池电量。

示例： Self-Consumption Mode下设置了备电SOC。

![](<../.gitbook/assets/4 (2).png>)
