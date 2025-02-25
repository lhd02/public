# 智能负载

{% include "../../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">在接入智能负载前，请确保组网中已配置Gateway。</mark>
* <mark style="color:blue;">智能负载接入的台数，由Gateway支持接入智能负载的台数决定。</mark>
* <mark style="color:blue;">App添</mark>加智<mark style="color:blue;">能负载后，可通过App对智能负载进行开关机，或系统根据您设置的SOC阈值，结合设备实际的运行情况实现远程控制设备开关机。</mark>

<figure><img src="../../../.gitbook/assets/smartload.png" alt="" width="375"><figcaption></figcaption></figure>

若您未找到所接设备的图标（如热得快），可选择“Other”进行接入。智能负载接入后，可在“Device”界面查看。

### Control Mode

<table><thead><tr><th width="75">序号</th><th width="141">参数名称</th><th width="135">参数名称</th><th>说明</th></tr></thead><tbody><tr><td><strong>1</strong></td><td>Manual</td><td>-</td><td><ul><li>显示为In Use时，您可在App上，通过 "<img src="../../../.gitbook/assets/2 (11).png" alt="" data-size="line">" 对智能负载进行开关机。</li><li>显示为Disable时，可添加Schedule和Ready by，自动控制智能负载。</li></ul></td></tr><tr><td><strong>2</strong></td><td>Schedule</td><td>Load Consumption Mode</td><td><ul><li>Depends on System：Automatically selects the most available power source from the system– solar, battery, or grid.</li><li>Solar Excess only：Operates appliances exclusively on solar surplus energy.</li><li>Battery Level Control：Allows precise energy management by setting start and stop thresholds for battery usage(e. g., start at 60%, stop at 20%). Recommended for users who demand detailed control of their system.</li></ul></td></tr><tr><td><strong>3</strong></td><td>Schedule</td><td>Auto charge</td><td>设置为<img src="../../../.gitbook/assets/3 (8).png" alt="" data-size="line">时，允许储能放电。 Use Battery Stop SOC：当储能电池SOC值小于该阈值时，关闭该负载。</td></tr><tr><td><strong>4</strong></td><td>Ready by</td><td>Activation For</td><td>运行总时间。在Be Ready By设置的时刻前，当天运行时间不足该设置值时，会启动负载</td></tr><tr><td><strong>5</strong></td><td>Ready by</td><td>Be Ready By</td><td>设置运行时刻。和运行总时间配合使用</td></tr></tbody></table>
