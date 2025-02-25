# 柴油发电机

{% include "../../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">在接入柴油发电机前，请确保组网中已配置支持连接柴油发电机的Gateway，且已正确接线。Gateway的信息，请查阅对应机型的《安装指南》。</mark>

系统可自动识别并接入柴油发电机。可通过“Device”→ “Generator”查看与设置。

<figure><img src="../../../.gitbook/assets/adddevoce.png" alt="" width="311"><figcaption></figcaption></figure>

### **Manual start by operating the generator's switch**

本模式下，您需要在柴油发电机侧进行开关机。

<table><thead><tr><th width="84">序号</th><th width="143">参数名称</th><th>说明</th></tr></thead><tbody><tr><td><strong>1</strong></td><td>Rated Power</td><td>设置柴油发电机的额定功率。</td></tr><tr><td><strong>2</strong></td><td>Maximum Power Duty</td><td>为保证油机最佳使用状态，建议对柴油发电机输出功率进行控制，推荐设置值为≤80%。</td></tr><tr><td><strong>3</strong></td><td>Minimum Power Duty</td><td>为保证油机不空载运行，建议对柴油发电机输出功率进行控制，推荐默认值为0%。</td></tr><tr><td><strong>4</strong></td><td>Battery Charging Cut-off SOC for Generator</td><td>当电池包的SOC＜“Battery Charging Cut-off SOC for Generator”值时，柴油发电机将为电池包充电至设置值。</td></tr></tbody></table>

### **two - wire – start**

本模式下，您可通过App端进行柴油发电机开关机或柴油发电机可实现自动开关机。

<table><thead><tr><th width="78">序号</th><th width="148">参数名称</th><th>说明</th></tr></thead><tbody><tr><td><strong>1</strong></td><td>Operating Mode</td><td><ul><li>Manual</li><li>Auto</li></ul></td></tr><tr><td><strong>2</strong></td><td>Generator Start</td><td>在“Manual”模式下，设置为 <img src="../../../.gitbook/assets/2 (2).png" alt="" data-size="line">时，您可在App上，通过 <img src="../../../.gitbook/assets/3 (1) (1).png" alt="" data-size="line"> ”对柴油发电机进行开关机。</td></tr><tr><td><strong>3</strong></td><td>Rated Power</td><td>设置柴油发电机的额定功率。</td></tr><tr><td><strong>4</strong></td><td>Maximum Power Duty</td><td>为保证油机最佳使用状态，建议对柴油发电机输出功率进行控制，推荐设置值为≤80%。</td></tr><tr><td>5</td><td>Minimum Power Duty</td><td>为保证油机不空载运行，建议对柴油发电机输出功率进行控制，推荐默认值为0%。</td></tr><tr><td>6</td><td>Battery Charging Cut-off SOC for Generator</td><td>当电池包的SOC＜“Battery Charging Cut-off SOC for Generator”值时，柴油发电机将为电池包充电至设置值。</td></tr><tr><td>7</td><td>Exercise</td><td><p>在“Auto”模式下，设置为 <img src="../../../.gitbook/assets/4 (1) (1).png" alt="" data-size="line">时，可设置启动方式。</p><ul><li>Duration：启动方式：<br>强制启动：按设定时间强制启动<br>智能启动：按设定时间智能启动</li><li>Interval：定时启动间隔 ，周期为1~52周</li><li>Day In Week：定时启动日期，星期一~星期日</li><li>Start Time：定时启动时刻</li></ul></td></tr><tr><td>8</td><td>Load Condition</td><td><p>在“Auto”模式下，设置为 <img src="../../../.gitbook/assets/5 (1) (1).png" alt="" data-size="line">时，负载功率测量类型为</p><ul><li>Total Load Power：负载总功率</li><li>Maximum Power Per-phase：每相负载功率最大值</li></ul></td></tr><tr><td>9</td><td>Generator Start Tatal Load Power Threshold</td><td>油机启动总负载功率阈值。当负载的总功率大于该阈值时，启动油机</td></tr><tr><td>10</td><td>Generator Stop Tatal Load Power Threshold</td><td>油机停止总负载功率阈值。当负载的总功率小于该阈值时，停止油机</td></tr><tr><td>11</td><td>Time of use</td><td>在“Auto”模式下，设置为 <img src="../../../.gitbook/assets/6 (1) (1).png" alt="" data-size="line">时，可以设置计划表启动油机。</td></tr><tr><td>12</td><td>Auto Start SOC</td><td>油机启动SOC阈值。当电池SOC大于该阈值时，启动油机</td></tr><tr><td>13</td><td>Auto Stop SOC</td><td>油机关闭SOC阈值。当电池SOC小于该阈值时，启动停止</td></tr></tbody></table>
