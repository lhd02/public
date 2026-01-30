# 防逆流参数设置

{% include "../../../.gitbook/includes/tips.md" %}

* <mark style="color:$danger;">点击跳转到EMS设置，若业主设置此参数，以参数小的生效。</mark>
* <mark style="color:blue;">开局时，安装商根据用户需求设置防逆流参数。</mark>
* <mark style="color:blue;">若开局后要更改参数，请根据当地法律法规和电网协议手动设置防逆流参数。</mark>
* <mark style="color:blue;">在设置防逆流参数前，请确保组网中已连接电表或Gateway。</mark>
* <mark style="color:blue;">不同的设备，显示参数会有所不同，请以实际界面为准。</mark>

<figure><img src="../../../.gitbook/assets/MSA1CM00083-防逆流参数设置.png" alt="" width="297"><figcaption></figcaption></figure>

<table><thead><tr><th width="69" align="center" valign="middle">序号</th><th width="243.4444580078125" valign="middle">参数名称</th><th valign="middle">说明</th></tr></thead><tbody><tr><td align="center" valign="middle">1</td><td valign="middle">Export Limitation</td><td valign="middle">设置为<img src="../../../.gitbook/assets/未标题-1_画板 1.png" alt="" data-size="line">时，并网点向电网的输出功率将受到限制。</td></tr><tr><td align="center" valign="middle">2</td><td valign="middle">Maximum Power Export Limitation</td><td valign="middle">设置并网点输出的最大功率值。</td></tr><tr><td align="center" valign="middle">3</td><td valign="middle">Import Limitation</td><td valign="middle">设置为<img src="../../../.gitbook/assets/未标题-1_画板 1.png" alt="" data-size="line">时，从电网输入的功率将受到限制。</td></tr><tr><td align="center" valign="middle">4</td><td valign="middle">Maximum Power Import Limitation</td><td valign="middle">设置并网点输入的最大功率值。</td></tr><tr><td align="center" valign="middle">5</td><td valign="middle">Grid Connection Point Power Control Method</td><td valign="middle"><ul><li>Total Power：并网点按照三相总功率控制，即三相功率之和不能够超过Maximum Power Export Limitation和Maximum Reverse Charging Power 。</li><li>Power Per Phase：并网点按照每相独立控制，即每相功率不能超过Maximum Power Export Limitation的1/3 和Maximum Reverse Charging Power的1/3。</li></ul></td></tr></tbody></table>
