# NS保护参数

VDE4105标准的区域（如VDE-AR-N-4105、VDE-AR-N 4110、VDE-AR-N 4120）要求电站发电设备支持连接NS（Network and System Protection）保护装置。

图 接线关系

<figure><img src="../../../../.gitbook/assets/nspro.png" alt=""><figcaption></figcaption></figure>

{% include "../../../../.gitbook/includes/tips.md" %}

* <mark style="color:blue;">推荐连接至DI5，若DI1～DI4未被占用，DI1～DI5均可接入NS保护装置。</mark>
* <mark style="color:blue;">设置参数前，请确保已正确连接NS保护装置。</mark>

<table><thead><tr><th width="79">序号</th><th width="156">参数名称</th><th>设置值</th></tr></thead><tbody><tr><td><strong>1</strong></td><td>DI Custom Function Enable</td><td><img src="../../../../.gitbook/assets/3 (8).png" alt="" data-size="line"></td></tr><tr><td><strong>2</strong></td><td>DI Custom Function Input Port</td><td>DI Input 5 (若NS保护装置连接在其他DI端口，请根据实际端口设置)</td></tr><tr><td><strong>3</strong></td><td>DI Custom Function Mode</td><td>DRM0 mode (switch ON, INV OFF)<br>注：<br>电网异常时，NS保护装置开关闭合，逆变器自动关机；电网恢复正常时，NS保护装置开关断开，逆变器开机。</td></tr><tr><td><strong>4</strong></td><td>Connected AIO Machine SN</td><td>连接NS保护装置的逆变器SN。</td></tr></tbody></table>
