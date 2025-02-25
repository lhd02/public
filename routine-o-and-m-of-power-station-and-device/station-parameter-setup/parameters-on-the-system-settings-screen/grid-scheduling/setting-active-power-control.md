# 设置有功功率控制

{% include "../../../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">电站有限功率需求时，电网调度人员需临时限制电站的有功馈入，或直接断开电站的所有有功功率馈入，即有功功率降额。</mark>

<figure><img src="../../../../.gitbook/assets/3 (1).jpeg" alt="" width="228"><figcaption></figcaption></figure>

<table><thead><tr><th width="100">序号</th><th width="144">参数名称</th><th>说明</th></tr></thead><tbody><tr><td><strong>1</strong></td><td>干接点有功调度使能</td><td>设置为 <img src="../../../../.gitbook/assets/2 (9).png" alt="" data-size="line">后，单台设备无需设置SN号，多台设备需下拉选择Ripple Control Receiver连接的设备SN号，SN号可通过设备侧边的SN查看。</td></tr><tr><td><strong>2</strong></td><td>DI1, DI2, DI3, DI4</td><td><p><img src="../../../../.gitbook/assets/settingactive.png" alt="" data-size="line"> 表示所设置的DI线缆上的开关闭合，为低电平。<br><img src="../../../../.gitbook/assets/seetingdeactive.png" alt="" data-size="line"> 表示所设置的DI线缆上的开关断开，为高电平。<br>图示参数仅为示例，设置时请根据实际情况进行配置。</p><ul><li>DI1～DI4的状态组合不得有重复，否则命令解析将执行异常。</li><li>如果实际输入DI信号与App设置不匹配，设备将会以最大有功功率指令（100%）运行。</li></ul></td></tr><tr><td><strong>3</strong></td><td>百分比(%)</td><td><ul><li>百分数值为设备最终执行的功率百分比，需根据当地电网要求设置为对应数值。</li><li>百分比正值表示逆变（逆变器输出有功功率），负值表示整流（逆变器吸收有功功率）。</li><li>最大支持添加16个百分比数值配置。</li></ul></td></tr></tbody></table>
