# 近端连接

## Settings

{% include "../.gitbook/includes/tips.md" %}

<mark style="color:blue;">扫描随箱资料上的SN码标签，若丢失可扫描逆变器侧边SN码。</mark>

<table><thead><tr><th width="94.5555419921875">序号</th><th width="201.6666259765625">参数</th><th>参数说明</th></tr></thead><tbody><tr><td>1</td><td>Log Download</td><td>近端连接设备后，下载设备的运行日志</td></tr><tr><td>2</td><td>Software Update</td><td>点击近端设备软件升级</td></tr><tr><td>3</td><td>self-diagnosis</td><td>点击近端设备诊断</td></tr><tr><td>4</td><td>Connectivity</td><td>Ethernet、WLAN、Cellular网络配置</td></tr><tr><td>5</td><td>Maintenance</td><td>设备开关机</td></tr></tbody></table>

## Connectivity

<table><thead><tr><th width="75" valign="middle">序号</th><th width="112" valign="middle">参数名称</th><th valign="top">说明</th></tr></thead><tbody><tr><td valign="middle">1</td><td valign="middle">Ethernet</td><td valign="top"><p>显示FE连接状态。</p><ul><li><p><mark style="color:$danger;">Ethernet：此参数设置后，对Ethernet、WLAN、Cellular都生效。</mark></p><ul><li><mark style="color:$danger;">Primary DNS ：主DNS，用于域名解析的DNS服务器，不可编辑。</mark></li><li><mark style="color:$danger;">Secondary DNS：副DNS，用于域名解析备用DNS服务器，可编辑。</mark></li></ul></li><li><p><mark style="color:$danger;">Obtain IP address automatically：设置为</mark><img src="../.gitbook/assets/未标题-1_画板 1.png" alt="" data-size="line"><mark style="color:$danger;">时，自动获取IP地址。设置为</mark><img src="../.gitbook/assets/image (16).png" alt=""><mark style="color:$danger;">时，用户需设置静态IP地址。</mark></p><ul><li><mark style="color:$danger;">IP Address：当前SigenStor/SigenStack Unit的FE的IP地址。</mark></li><li><mark style="color:$danger;">Gateway：当前SigenStor/SigenStack Unit的FE的网关。</mark></li><li><mark style="color:$danger;">Subnet Mask：当前SigenStor/SigenStack Unit的FE的子网掩码。</mark></li></ul></li><li>FE网络连接参数默认DHCP自动获取。若您需要更改，请按以下步骤操作：</li></ul><ol><li>将“Obtain IP address automatically”设置为<img src="../.gitbook/assets/image (16).png" alt="">，修改参数。</li><li>重新将用于连接网络的网线插入设备。</li></ol></td></tr><tr><td valign="middle">2</td><td valign="middle">WLAN</td><td valign="top"><p>显示WLAN连接状态。</p><p>若此处显示未连接，但您想采用WLAN连接网络，请按以下说明操作：</p><ul><li>配置WLAN通信前，请确认设备已安装天线。</li><li>连接非加密WLAN，可能导致网络不可用，不推荐使用。</li><li>当设备仅可用WLAN连接网络时，不可切换其他无线路由器WLAN。</li><li><mark style="color:$danger;">点击“Go Set Up”配置WLAN网络。</mark></li></ul></td></tr><tr><td valign="middle">3</td><td valign="middle">Cellular</td><td valign="top"><p>显示4G连接状态。</p><p>若此处显示未连接，但您想采用4G连接网络，请按以下说明操作：</p><ul><li>配置4G通信前，请确保Sigen CommMod已插入。</li><li>当采用4G通信时，可查看当前每月使用的流量。</li></ul></td></tr></tbody></table>

## <mark style="color:$danger;">（可选）离网自供电设置</mark>

{% include "../.gitbook/includes/tips.md" %}

* <mark style="color:$danger;">仅工商业电站有此功能。</mark>
* <mark style="color:red;">启动离网自供电后，设备能够离网运行，为施工设备供电。</mark>

<figure><img src="../.gitbook/assets/MSA1CM00081-离网自供电 (1).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="85.5555419921875" align="center" valign="middle">序号</th><th width="217.945556640625" valign="middle">参数名称</th><th valign="middle">说明</th></tr></thead><tbody><tr><td align="center" valign="middle">1</td><td valign="middle"><mark style="color:red;">Off-grid self-powered device</mark></td><td valign="middle"><mark style="color:$danger;">设置为</mark><img src="../.gitbook/assets/7 (2) (1).png" alt="" data-size="line"><mark style="color:red;">时，使能离网自供电功能。</mark></td></tr><tr><td align="center" valign="middle">2</td><td valign="middle"><mark style="color:$danger;">Output Mode</mark></td><td valign="middle"><ul><li><mark style="color:$danger;">Single Phase：此模式下，逆变器从三相电网的L1、L2两相取电，给单相负载供电。（Sigen PV (50–110)M1-HYB 系列为负载口）。</mark></li><li><mark style="color:$danger;">Three Phase Three Wire：此模式下，逆变器从三相电网的L1、L2、L3三相取电，给三相负载供电（Sigen PV (50–110)M1-HYB 系列为负载口）。</mark></li></ul></td></tr><tr><td align="center" valign="middle">3</td><td valign="middle"><mark style="color:$danger;">Serial number of the connected device</mark></td><td valign="middle"><mark style="color:$danger;">输入自供电设备的SN号。</mark></td></tr></tbody></table>
