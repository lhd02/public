# 逆变器设置

<figure><img src="../.gitbook/assets/MSA1CM00078-逆变器设置.png" alt=""><figcaption></figcaption></figure>

## IPS（仅意大利CEI-021电网标准码存在）

<table><thead><tr><th width="83" align="center">序号</th><th width="264">参数名称</th><th>说明</th></tr></thead><tbody><tr><td align="center">1</td><td>IPS external command signal</td><td>设置IPS外部指令信号。</td></tr><tr><td align="center">2</td><td>IPS local command signal</td><td>设置IPS内部指令信号。</td></tr></tbody></table>

## **Power**

<table><thead><tr><th width="79" align="center">序号</th><th width="264">参数名称</th><th>说明</th></tr></thead><tbody><tr><td align="center">1</td><td>Maximum apparent power</td><td>设置本参数可调整设备的最大视在功率。</td></tr><tr><td align="center">2</td><td>Maximum Active Power Output</td><td>设置本参数可调整设备的最大输出有功功率。</td></tr><tr><td align="center">3</td><td>Maximum Active Power Input</td><td>设置本参数可调整设备的最大输入有功功率。</td></tr><tr><td align="center">4</td><td><mark style="color:$danger;">Max. Continuous Current</mark></td><td>设置最大视在电流。</td></tr></tbody></table>

## **System Parameters**

<table><thead><tr><th width="91" align="center" valign="middle"></th><th width="250" valign="middle">参数名称</th><th valign="top">说明</th></tr></thead><tbody><tr><td align="center" valign="middle">1</td><td valign="middle">Insulation impedance threshold</td><td valign="top">为保护设备安全，当设备检测到实际光伏阵列输出的对地绝缘阻抗值＜此参数所设置的值时，设备无法运行。</td></tr><tr><td align="center" valign="middle">2</td><td valign="middle">PV input start voltage</td><td valign="top">当接入的PV组串较少时，可设置更低的启动电压。</td></tr><tr><td align="center" valign="middle">3</td><td valign="middle">Ground fault detection</td><td valign="top">当设置为<img src="../.gitbook/assets/11 (1) (2).png" alt="" data-size="line">时，当设备未接地或接地不良时，将产生接地异常告警。</td></tr><tr><td align="center" valign="middle">4</td><td valign="middle">MPPT Multi-Peak Scanning</td><td valign="top"><p>当设置为<img src="../.gitbook/assets/11 (1) (2).png" alt="" data-size="line">时，可触发多峰扫描。</p><ul><li>MPPT Multi-Peak Scanning Interval: 设置多峰扫描周期时间，每隔设置时间扫描一次。</li></ul></td></tr><tr><td align="center" valign="middle">5</td><td valign="middle">Leakage current optimization enabled</td><td valign="top">当设置为<img src="../.gitbook/assets/11 (1) (2).png" alt="" data-size="line">时，可减少机器对地的漏电流，但是同时可能会增加设备功率损耗。</td></tr><tr><td align="center" valign="middle">6</td><td valign="middle"><mark style="color:$danger;">Grid Power Loss No-Auto-Start Endble</mark></td><td valign="top"><mark style="color:$danger;">电网故障后，逆变器无法自动恢复，需要人工确认后在APP上清除故障告警。</mark></td></tr></tbody></table>

## **Fan parameters**

<table><thead><tr><th width="254" valign="middle">参数名称</th><th valign="top">说明</th></tr></thead><tbody><tr><td valign="middle">External fan silent mode</td><td valign="top">当设置为<img src="../.gitbook/assets/11 (1) (2).png" alt="" data-size="line">时，风扇最大转速将被限制，从而降低风扇产生的噪音。</td></tr></tbody></table>

## **EMS Control**

<table><thead><tr><th width="250" valign="middle">参数名称</th><th valign="top">说明</th></tr></thead><tbody><tr><td valign="middle">Single-Machine Active Power Dispatch Enable</td><td valign="top"><p>设置为<img src="../.gitbook/assets/11 (1) (2).png" alt="" data-size="line">时，针对单台设备进行功率调度，可设置有功功率模式，无功功率模式。</p><p><img src="../.gitbook/assets/warning (1).png" alt="" data-size="original"></p><p><mark style="color:orange;">设置了本参数的逆变器，将无法参与EMS控制。</mark></p></td></tr></tbody></table>

## Pack Delayed Activation

<table><thead><tr><th width="241">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>Pack Delay Activation Enable</td><td>设置为<img src="../.gitbook/assets/10 (1) (2).png" alt="" data-size="line"> 时, PACK 延时激活，开局时，不激活PACK。开局完成后，根据需要在APP界面手动激活PACK。</td></tr></tbody></table>

## PV- positive bias

<table><thead><tr><th width="79">序号</th><th>参数名称</th><th>说明</th></tr></thead><tbody><tr><td>1</td><td>PID Compensation Direction</td><td><p>PID 补偿方向。仅支持 P 型电池板或者 PV - 正偏置。</p><ul><li>PV Positive Bias：设置为<img src="../.gitbook/assets/10 (1) (2).png" alt="" data-size="line">时, 可设置PV - 正偏置。</li></ul></td></tr><tr><td>2</td><td>Pid Repair Enable</td><td>设置为<img src="../.gitbook/assets/10 (1) (2).png" alt="" data-size="line">时, PID 修复使能。仅在夜间且并网继电器断开的情况下工作。</td></tr><tr><td>3</td><td>Pid Protection Enabled</td><td>设置为<img src="../.gitbook/assets/10 (1) (2).png" alt="" data-size="line">时, PID 防护使能。仅限IT电网，即输出带有隔离变压器的电网。</td></tr><tr><td>4</td><td>Nighttime PID Protection Enabled</td><td>设置为<img src="../.gitbook/assets/10 (1) (2).png" alt="" data-size="line">时, 夜间PID保护使能。夜间工作时，检测到 PID 模块异常，关机保护。</td></tr></tbody></table>

## **Islanding**

<table><thead><tr><th width="80" align="center" valign="middle">序号</th><th width="215.44451904296875" valign="middle">参数名称</th><th valign="top">说明</th></tr></thead><tbody><tr><td align="center" valign="middle">1</td><td valign="middle">Active Anti-islanding</td><td valign="top">当设置为<img src="../.gitbook/assets/未标题-1_画板 1.png" alt="" data-size="line">时，主动防孤岛使能。</td></tr><tr><td align="center" valign="middle">2</td><td valign="middle">Passive Islanding Enable</td><td valign="top"><p>当设置为<img src="../.gitbook/assets/未标题-1_画板 1.png" alt="" data-size="line">时，利用电网断电时设备输出端电压、频率、相位或谐波的变化进行孤岛效应检测。</p><ul><li><mark style="color:$danger;">被动孤岛的相位角保护值：当电网电压的相位跳变超过设置的保护值后，会触发被动孤岛保护动作。</mark></li></ul></td></tr></tbody></table>

## AFCI <a href="#afci" id="afci"></a>

<table><thead><tr><th width="156.5555419921875">参数名称</th><th>说明</th></tr></thead><tbody><tr><td>AFCI Enables</td><td>设置为<img src="../.gitbook/assets/10 (1) (2).png" alt="" data-size="line"> 时, 该设备将进行直流电弧测试。</td></tr></tbody></table>
