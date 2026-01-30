# SigenStor EVDC设置

<figure><img src="../../.gitbook/assets/MSA1CM00078-EVDC (1).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="76" align="center">序号</th><th width="159.818115234375">参数名称</th><th>说明</th></tr></thead><tbody><tr><td align="center">1</td><td>Charging Record</td><td>点击可查看充电记录。</td></tr><tr><td align="center">2</td><td>Schedule</td><td>若接入的车支持预约充电功能，可设置预约充放电时段。</td></tr></tbody></table>

### **Charging Preference**

<table><thead><tr><th width="76" align="center">序号</th><th width="172.818115234375">参数名称</th><th>说明</th></tr></thead><tbody><tr><td align="center"><strong>1</strong></td><td>Charging Mode</td><td><ol><li><strong>Fast Charging：大幅提升充电速率，短时间为设备补充大量电量的快速充电模式。</strong></li><li><strong>PV Surplus Charging：利用光伏发电系统中多余电能给电池充电的光伏余电充电模式。</strong></li><li><strong>（可选）Bi-directional Charging：将SigenStor EVDC作为额外的“储能”，参与整个电站的调度，为家用设备或电网放电。</strong>(开启V2X功能后，可设置此模式。具体操作步骤参见（<a href="ke-xuan-v2x-gong-neng-she-zhi.md">可选）V2X功能设置</a>。)</li></ol><ul><li>Battery Boost：设置为<img src="../../.gitbook/assets/image (19).png" alt="">时，可通过家用电池充电。</li><li>Cut-OFF SOC：Battery Boost使能时，当实际SOC＜设置参数时，电池停止给SigenStor EVDC充电。</li><li>Car Discharging Power：设置电动车的最大放电功率，SigenStor EVDC放电功率＜设置参数。</li><li>Stop Discharging：放电截止SOC，当电动车的SOC小于该值时，电动车停止放电。</li><li>Grid Charging：设置为<img src="../../.gitbook/assets/image (19).png" alt="">时，在PV余电模式下，允许从电网给电动车充电。</li><li>Surplus PV priority：选中设备，上下拖动可修改设备优先级。</li></ul></td></tr><tr><td align="center"><strong>2</strong></td><td>Charging Setting</td><td><ul><li>Charging power allowed for EVDC：设置SigenStor EVDC允许最大充电功率。</li><li>Vehicle Charging Cut-off SOC：设置充电截止SOC参数。当电动车的SOC值＞设置参数时，停止给车充电。</li></ul></td></tr><tr><td align="center"><strong>3</strong></td><td>OCPP Management</td><td><ul><li>OCPP Status：显式OCPP连接状态。</li><li>OCPP Settings：设置为<img src="../../.gitbook/assets/image (17).png" alt=""> 时，SigenStor EVDC可以连接到OCPP的服务器，使用者可以从URL下拉菜单选择OCPP的平台。</li></ul></td></tr><tr><td align="center"><strong>4</strong></td><td>Authorization</td><td>充电鉴权设置。设置为 <img src="../../.gitbook/assets/image (16).png" alt="">时，可无鉴权充电。</td></tr><tr><td align="center"><strong>5</strong></td><td>Card Management</td><td>绑定Sigen RFID card。</td></tr><tr><td align="center"><strong>6</strong></td><td>My Vehichle</td><td>点击可添加和修改电动车信息。</td></tr></tbody></table>

### **Charger Settings**

<table><thead><tr><th width="151.54547119140625">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>Maintenance</td><td><ul><li>Reset：设备重启。</li><li>Erase All Content：可清除5min性能数据、告警、小时&#x26;日&#x26;月&#x26;年发电量、运行日志、设备信息等，请谨慎操作。</li></ul></td></tr></tbody></table>

{% include "../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">SigenStor EVDC用户日常使用方式及注意事项请参见《Sigen EV DC Charging Module 用户手册》。</mark>
