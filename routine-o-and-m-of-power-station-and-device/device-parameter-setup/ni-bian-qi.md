# 逆变器

![](<../../.gitbook/assets/0 (4).jpeg>)

### **IPS（仅意大利CEI-021电网标准码存在）**

<table><thead><tr><th width="75">序号</th><th>参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>IPS external command signal</td><td>设置IPS外部指令信号。</td></tr><tr><td>2</td><td>IPS local command signal</td><td>设置IPS内部指令信号。</td></tr></tbody></table>

### **Power**

<table><thead><tr><th width="122">序号</th><th width="219">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Maximum apparent power</td><td>设置本参数可调整设备的最大视在功率。</td></tr><tr><td>2</td><td>Maximum Active Power Output</td><td>设置本参数可调整设备的最大输出有功功率。</td></tr><tr><td>3</td><td>Maximum Active Power Input</td><td>设置本参数可调整设备的最大输入有功功率。</td></tr></tbody></table>

### **System Parameters**

<table><thead><tr><th width="76">序号</th><th width="167">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Insulation impedance threshold</td><td>为保护设备安全，当设备检测到实际光伏阵列输出的对地绝缘阻抗值＜此参数所设置的值时，设备无法运行。</td></tr><tr><td>2</td><td>PV input start voltage</td><td>当接入的PV组串较少时，可设置更低的启动电压。</td></tr><tr><td>3</td><td>Ground fault detection</td><td>当设置为<img src="../../.gitbook/assets/1.png" alt="" data-size="line">时，当设备未接地或接地不良时，将产生接地异常告警。</td></tr></tbody></table>

### **Voltage Protection**

<table><thead><tr><th width="96">序号</th><th width="152">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Level-<em><strong>N</strong></em> Overvoltage Protection Threshold</td><td>设置电网电压<em><strong>N</strong></em>级过压保护值，当实际电压＞所设置的保护值，并满足设置的保护时间时，将触发设备告警，反之告警消失。</td></tr><tr><td>2</td><td>Level-<em><strong>N</strong></em> Overvoltage Protection Duration</td><td>设置电网电压<em><strong>N</strong></em>级过压保护时间。</td></tr><tr><td>3</td><td>Level-<em><strong>N</strong></em> Undervoltage Protection Threshold</td><td>设置电网电压<em><strong>N</strong></em>级欠压保护值，当实际电压＜所设置的保护值，并满足设置的保护时间时，将触发设备告警，反之告警消失。</td></tr><tr><td>5</td><td>Level-<em><strong>N</strong></em> Undervoltage Protection Duration</td><td>设置电网电压<em><strong>N</strong></em>级欠压保护时间。</td></tr><tr><td>6</td><td>Ten-Minute Sliding Window Overvoltage Protection Threshold</td><td>设置十分钟过压保护点。当电压以十分钟为窗口滑动的平均值＞所设置的保护值，并满足设置的保护时间时，将触发设备告警，反之告警消失。</td></tr><tr><td>7</td><td>Ten-Minute Sliding Window Overvoltage Protection Time</td><td>设置十分钟过压保护时间。</td></tr></tbody></table>

注：_**N**_&#x8868;示1到6。“Voltage Protection”可设置参数与“Grid Code”相关联，具体可设置参数以实际界面为准。

### **Frequency Protection**

<table><thead><tr><th width="95">序号</th><th width="135">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Level-<em><strong>N</strong></em> Overfrequency Protection Threshold</td><td>设置电网电压<em><strong>N</strong></em>级过频保护值，当实际电网频率＞所设置的保护值，并满足设置的保护时间时，将触发设备告警，反之告警消失。</td></tr><tr><td>2</td><td>Level-<em><strong>N</strong></em> Overfrequency Protection Duration</td><td>设置电网电压<em><strong>N</strong></em>级过频保护时间。</td></tr><tr><td>3</td><td>Level-<em><strong>N</strong></em> Underfrequency Protection Threshold</td><td>设置电网电压<em><strong>N</strong></em>级欠频保护值，当实际电网频率＜所设置的保护值，并满足设置的保护时间时，将触发设备告警，反之告警消失。</td></tr><tr><td>4</td><td>Level-<em><strong>N</strong></em> Underfrequency Protection Duration</td><td>设置电网电压<em><strong>N</strong></em>级欠频保护时间。</td></tr></tbody></table>

注：_**N**_&#x8868;示1到6。“Frequency Protection”可设置参数与“Grid Code”相关联，具体可设置参数以实际界面为准。

### **Power Response to overfrequency**

<table><thead><tr><th width="83">序号</th><th width="237">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Power Response to Overfrequency Enable</td><td>当设置为<img src="../../.gitbook/assets/2.png" alt="" data-size="line">时，电网频率＞触发值，会限制设备输出有功功率。</td></tr><tr><td>2</td><td>Trigger Frequency</td><td>设置过频降额触发阈值。</td></tr><tr><td>3</td><td>Power Droop Rate</td><td>频率恢复后，有功功率按照本参数设置的梯度值恢复。</td></tr><tr><td>4</td><td>Exit Frequency</td><td>设置过频降额退出阈值。即电网频率＜退出阈值时，设备输出有功功率停止降额。</td></tr><tr><td>5</td><td>Power Reference Mode</td><td><ul><li>Freeze Active Power When Triggered：触发过频降额时的实时有功功率。</li><li>Maximum Active Power：设备最大有功功率。</li><li>When triggered, freeze active power + minimum active power absolutevalue：触发过频降额时的实时功率+储能可充电功率。</li></ul></td></tr><tr><td>6</td><td>Overfrequency derating response delay</td><td>设置过频降额后，设备输出功率开始变化至到达平稳值的95%所需要的时间。</td></tr><tr><td>7</td><td>Overfrequency derating exit delay</td><td>设置为<img src="../../.gitbook/assets/3.png" alt="" data-size="line">时，过频降额退出延时生效，可设置“Overfrequency derating exit delay”值。</td></tr><tr><td>8</td><td>Overfrequency derating exit frequency enable</td><td>设置为<img src="../../.gitbook/assets/4.png" alt="" data-size="line">时，过频降额退出延时生效，可设置“Overfrequency derating exit delay”值。</td></tr></tbody></table>

### **Power Response to underfrequency**

<table><thead><tr><th width="85">序号</th><th width="144">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Power Response to Underfrequency Enable</td><td>当设置为<img src="../../.gitbook/assets/5.png" alt="" data-size="line">时，电网频率＜触发值，设备输出有功功率变大。</td></tr><tr><td>2</td><td>Trigger Frequency</td><td>设置欠频升功率触发阈值。</td></tr><tr><td>3</td><td>Power Droop Rate</td><td>频率恢复后，有功功率按照本参数设置的梯度值恢复。</td></tr><tr><td>4</td><td>Exit Frequency</td><td>设置欠频升功率退出阈值。即电网频率＞退出阈值时，设备输出有功功率停止升功率。</td></tr><tr><td>5</td><td>Underfrequency power boost power reference mode</td><td><ul><li>Freeze Active Power When Triggered：触发欠频升功率时的实时有功功率</li><li>Remaining active power capacity of PCS：设备额定功率</li><li>Maximum Active Power：设备最大有功功率</li><li>Remaining discharge power capacity of the battery：触发欠频升功率时的实时功率+储能可放电功率</li></ul></td></tr><tr><td>9</td><td>Underfrequency power boost response delay</td><td>设置触发欠频升功率后，等待设备输出有功功率产生变化的时间。</td></tr><tr><td>7</td><td>Underfrequency power boost exit delay</td><td>“Underfrequency power boost exit frequency enable”设置为<img src="../../.gitbook/assets/6.png" alt="" data-size="line">时，通过本参数，设置退出欠频升功率后，当电网频率＞“Under-Frequency Power Increase Exit Frequency”值时，等待设备输出有功功率停止升功率的时间。</td></tr><tr><td>8</td><td>Underfrequency power boost exit frequency enable</td><td>设置为<img src="../../.gitbook/assets/7.png" alt="" data-size="line">时，欠频升功率退出延时生效，可设置“Underfrequency power boost exit delay”。</td></tr></tbody></table>

### **P-U Curve**

<table><thead><tr><th width="88">序号</th><th width="120">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>P-U Voltage Enable</td><td>当设置为<img src="../../.gitbook/assets/8.png" alt="" data-size="line">时，电网电压根据PU曲线对应关系，调节设备输出有功功率。</td></tr><tr><td>2</td><td>P-U curve Points included</td><td>设备根据电网电压实际值与额定值的比“U/Un(%)”，实时调整有功功率和额定功率的比值P/Pn。</td></tr><tr><td>3</td><td>P-U curve power regulation time</td><td>设置因电网电压改变而根据PU曲线对应关系调节设备输出有功功率值的95%所需时间。</td></tr></tbody></table>

### **Grid Fault Reconnection**

<table><thead><tr><th width="91">序号</th><th width="114">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Grid Fault Reconnect Enable</td><td>当设置为 <img src="../../.gitbook/assets/20.png" alt="" data-size="line">时，电网故障恢复后，实际电网电压和频率在所设置范围内并持续设定时间后，才允许设备并网。</td></tr><tr><td>2</td><td>Reconnection Upper Frequency</td><td>电网故障恢复后，电网频率高于“Reconnection Upper Frequency”的设定值时不允许设备重新并网</td></tr><tr><td>3</td><td>Reconnection Lower Frequency</td><td>电网故障恢复后，电网频率低于“Reconnection Lower Frequency”的设定值时不允许设备重新并网</td></tr><tr><td>4</td><td>Reconnection Upper Voltage</td><td>电网故障恢复后，电网电压高于“Reconnection Upper Voltage”的设定值时不允许设备重新并网</td></tr><tr><td>5</td><td>Reconnection Lower Voltage</td><td>电网故障恢复后，电网电压低于“Reconnection Lower Voltage”的设定值时不允许设备重新并网</td></tr><tr><td>6</td><td>Observation Time</td><td>设置电网故障恢复以后，设备重新启动的等待时间。</td></tr><tr><td>7</td><td>Maximum <strong>Continuous</strong> Current</td><td>设置本参数可调整设备的最大视在电流。</td></tr><tr><td>8</td><td>AFCI Enables</td><td>设置为<img src="../../.gitbook/assets/10.png" alt="" data-size="line">时，设备将进行直流电弧检测。</td></tr></tbody></table>

### **EMS Control**

<table><thead><tr><th width="76">序号</th><th width="115">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Single-Machine Active Power Dispatch Enable</td><td><p>设置为<img src="../../.gitbook/assets/11.png" alt="" data-size="line">时，针对单台设备进行功率调度，可设置有功功率模式，无功功率模式。</p><p><img src="../../.gitbook/assets/warning.png" alt="" data-size="original"></p><p>设置了本参数的逆变器，将无法参与EMS控制。</p></td></tr></tbody></table>

### **Grid Connection Startup Check**

<table><thead><tr><th width="76">序号</th><th width="118">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Startup Grid Connection Detection</td><td>当设置为<img src="../../.gitbook/assets/13.png" alt="" data-size="line">时，实际电网电压和频率在所设置范围内并持续设定时间后，才允许设备并网。</td></tr><tr><td>2</td><td>Startup Grid Connection Detection Time</td><td>设置设备开机后，实际电网电压和频率在所设置范围内，设备等待并网的时间。</td></tr><tr><td>3</td><td>Startup Grid Connection Detection Frequency Upper Limit</td><td>设置设备开机后，允许设备并网的频率最大值。</td></tr><tr><td>4</td><td>Startup Grid Connection Detection Frequency Lower Limit</td><td>设置设备开机后，允许设备并网的频率最小值。</td></tr><tr><td>5</td><td>Startup Grid Connection Detection Voltage Upper Limit</td><td>设置设备开机后，允许设备并网的电压最大值。</td></tr><tr><td>6</td><td>Startup Grid Connection Detection Voltage Lower Limit</td><td>设置设备开机后，允许设备并网的电压最小值。</td></tr><tr><td>7</td><td>Startup Grid Connection Detection Power Gradient</td><td>设置设备开机后，设备并网后功率逐渐上升的幅度。</td></tr></tbody></table>

### **Reactive power Settings**

<table><thead><tr><th width="100">序号</th><th width="306">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Reactive power regulation mode</td><td>按照所设置的模式调节无功功率。</td></tr><tr><td>2</td><td>Enable QU Curve Automatic Adjustment</td><td>当设置为<img src="../../.gitbook/assets/14.png" alt="" data-size="line">时，无功功率依照“QU Curve Automatic Adjustment Time Constant”设置的时间值完成自动调节。</td></tr><tr><td>3</td><td>Reactive power Q/S regulation</td><td>按照百分比形式调节设备的无功功率输出。</td></tr><tr><td>4</td><td>QU Curve Automatic Adjustment Time Constant</td><td>设置电网电压变化触发QU曲线时，无功功率完成自动调节所需要的时间。</td></tr><tr><td>5</td><td>Fixed value adjustment of reactive power</td><td>按照固定值形式调节设备的无功功率输出。</td></tr><tr><td>6</td><td>Power factor adjustment</td><td>设置设备的功率因数。</td></tr><tr><td>7</td><td>PF-P/Pn curve Points included</td><td>设置设备根据P/Pn(%)实时调整输出的功率因数。</td></tr><tr><td>8</td><td>PF-P/Pn adjustment time</td><td>设置根据对应PF-P/Pn曲线关系调节设备输出无功功率值的95%所需时间。</td></tr><tr><td>9</td><td>PF-U curve Points included</td><td>设置设备根据电网电压实际值与额定值的比“U/Un(%)”，实时调整的功率因数。</td></tr><tr><td>10</td><td>Q-P curve Points included</td><td>设置设备根据有功功率与有功最大值的比值“P/Pmax”，实时调整无功功率与有功最大值的比Q/Pmax。</td></tr><tr><td>11</td><td>Q-P curve adjustment time</td><td>设置根据对应Q-P曲线关系调节设备输出无功功率值的95%所需时间。</td></tr><tr><td>12</td><td>Q-U curve Points included</td><td>设置设备根据电网电压实际值与额定值的比值U/Un(%)，实时调整输出的无功功率和视在功率的比值Q/S。</td></tr><tr><td>13</td><td>Q-U curve trigger power</td><td>设置设备触发Q-U曲线功能的P/Pmax。设备的实际功率＞设置值时，启动Q-U曲线调度功能。</td></tr><tr><td>14</td><td>Q-U curve exit power</td><td>设置设备退出Q-U曲线功能的P/Pmax。设备的实际功率＜设置值时，退出Q-U曲线调度功能。。</td></tr><tr><td>15</td><td>Q-U curve power regulation time</td><td>设置根据对应Q-U曲线关系调节设备输出无功功率值的95%所需时间。</td></tr></tbody></table>

### **Active power Settings**

<table><thead><tr><th width="93">序号</th><th width="363">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Active power regulation mode</td><td>按照所设置的模式调节有功功率。</td></tr><tr><td>2</td><td>Percentage active power adjustmen</td><td>按照百分比形式调节设备的有功功率输出。</td></tr><tr><td>3</td><td>Fixed value adjustment of active power</td><td>按照固定值形式调节设备的有功功率输出。</td></tr></tbody></table>

### **Low Voltage Ride Through**

<table><thead><tr><th width="103">序号</th><th width="214">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Low Penetration Mode</td><td><p><strong>设置低穿模式。低穿模式包括</strong> Reactive power priority,</p><p>Active power priority, Zero current, Constant current.</p></td></tr><tr><td>2</td><td>LVRT Enable</td><td>当设置为<img src="../../.gitbook/assets/15.png" alt="" data-size="line">时，电网异常出现短时低电压时，设备不能立即脱离电网，需要支撑一段时间。</td></tr><tr><td>3</td><td>Trigger Threshold</td><td>当电网电压＞本参数设置值时，将触发低电压穿越。</td></tr><tr><td>4</td><td>Low Penetration Curve</td><td>LVRT曲线。设置设备低电压穿越能力。</td></tr><tr><td>5</td><td>Zero Current Mode Trigger Threshold</td><td>零电流模式触发阈值。当电网电压低于该阈值时，触发零电流模式</td></tr></tbody></table>

### **High Voltage Ride Through**

<table><thead><tr><th width="110">序号</th><th width="159">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>HVRT Enable</td><td><p>当设置为<img src="../../.gitbook/assets/16.png" alt="" data-size="line">时，电网异常出现短时高电压时，设备不能</p><p>立即脱离电网，需要支撑一段时间。</p></td></tr><tr><td>2</td><td>Trigger Threshold</td><td>当电网电压＞本参数设置值时，将触发高电压穿越。</td></tr><tr><td>3</td><td>High Penetration Curve</td><td>HVRT曲线。设置设备高电压穿越能力。</td></tr></tbody></table>

### **Fan parameters**

<table><thead><tr><th width="111">序号</th><th width="176">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>External fan silent mode</td><td>当设置为<img src="../../.gitbook/assets/17.png" alt="" data-size="line">时，风扇最大转速将被限制，从而降低风扇产生的噪音。</td></tr></tbody></table>

### **Startup Grid Connection**

<table><thead><tr><th width="117">序号</th><th width="210">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Startup Grid Connection Enable</td><td><p>当设置为时，设备首次开机并网，需要电网电压满足重连条件才允许并网</p><p><img src="../../.gitbook/assets/18.png" alt="" data-size="original"></p></td></tr><tr><td>2</td><td>Observation Time</td><td>设备首次开机，需要启动等待时间，满足该时间才允许并网。</td></tr><tr><td>3</td><td>Connection Upper Frequency</td><td>设备首次开机并网，电网频率高于“Reconnection Upper Frequency”的设定值时不允许设备并网</td></tr><tr><td>4</td><td>Connection Lower Frequency</td><td>设备首次开机并网，电网频率低于“Reconnection Lower Frequency”的设定值时不允许设备并网</td></tr><tr><td>5</td><td>Connection Upper Voltage</td><td>设备首次开机并网，电网电压高于“Reconnection Upper Voltage”的设定值时不允许设备并网</td></tr><tr><td>6</td><td>Connection Lower Voltage</td><td>设备首次开机并网，电网电压低于“Reconnection Lower Voltage”的设定值时不允许设备并网</td></tr><tr><td>7</td><td>Startup Grid Connection Detection Power Gradient</td><td>设备首次开机，并网后功率上升梯度。</td></tr></tbody></table>

### **Islanding**

<table><thead><tr><th width="127">序号</th><th width="202">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>Active Islanding</td><td>当设置为<img src="../../.gitbook/assets/19.png" alt="" data-size="line">时，可通过控制设备，使其输出功率、频率或相位存在一定的扰动。</td></tr><tr><td>2</td><td>Passive Islanding</td><td>当设置为<img src="../../.gitbook/assets/20.png" alt="" data-size="line">时，利用电网断电时设备输出端电压、频率、相位或谐波的变化进行孤岛效应检测。</td></tr></tbody></table>
