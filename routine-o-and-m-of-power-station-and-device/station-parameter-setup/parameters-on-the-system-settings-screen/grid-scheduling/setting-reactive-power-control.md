# 设置无功功率控制

{% include "../../../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">电网公司要求大型电站对并网点电压具备一定得调节能力，电网调度人员根据电网中实时无功功率传输情况，要求电站向并网点吸收或注入无功功率，即无功功率补偿。</mark>

![](<../../../../.gitbook/assets/3 (1).jpeg>)

<table><thead><tr><th width="72">序号</th><th width="139">参数名称</th><th>说明</th></tr></thead><tbody><tr><td><strong>1</strong></td><td>无功功率控制方式</td><td><ul><li>无输出：如果电网公司不要求电站调节并网点电压，且不需要配合电网实施无功功率补偿，设备可以保持纯有功功率输出状态运行，设置为“无输出”。</li><li>DI模式：设置无功干接点调度参数时，需设置为“DI模式”。</li></ul><ul><li>并网点功率因数控制：当分布式电站需要执行分布式无功功率补偿功能，以减少或避免力调电费，提高电站收益时，需要设置“并网点功率因数控制”。</li></ul><p>选择DI模式后，单台设备无需设置SN号，多台设备需下拉选择Ripple Control Receiver连接的设备SN号，SN号可通过设备侧边的SN查看。</p></td></tr><tr><td><strong>2</strong></td><td>DI1, DI2, DI3, DI4</td><td><p><img src="../../../../.gitbook/assets/settingactive.png" alt="" data-size="line"> 表示所设置的DI线缆上的开关闭合，为低电平。<br><img src="../../../../.gitbook/assets/seetingdeactive.png" alt="" data-size="line"> 表示所设置的DI线缆上的开关断开，为高电平。</p><ul><li>图示参数仅为示例，设置时请根据实际情况进行配置。</li><li>DI1～DI4的状态组合不得有重复，否则命令解析将执行异常。</li><li>如果实际输入DI信号与App设置不匹配，设备将会以最小无功功率指令（0%）运行。</li></ul></td></tr><tr><td><strong>3</strong></td><td>百分比(%)</td><td><ul><li>百分数值为设备最终执行的功率百分比，需根据当地电网要求设置为对应数值。</li><li>百分比正值表示输出容性无功（抬升电压），负值表示输出感性无功（降低电压）。</li><li>最大支持添加16个百分比数值配置。</li></ul></td></tr></tbody></table>
