# SG热泵

{% include "../../../.gitbook/includes/tips.md" %}

<mark style="color:blue;">在接入热泵前，请确保以下信息：</mark>

* <mark style="color:blue;">热泵已经正确连接至本公司逆变器的DO端口，且逆变器软件版本支持连接热泵。</mark>
* <mark style="color:blue;">请确保，已经在“System Settings”菜单下，将“DO Custom Function Enable”设置为</mark> <img src="../../../.gitbook/assets/3 (8).png" alt="" data-size="line">

<figure><img src="../../../.gitbook/assets/sgheart.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="75">序号</th><th width="142">参数名称</th><th>说明</th></tr></thead><tbody><tr><td><strong>1</strong></td><td>Operating Mode</td><td><ul><li>Manual</li><li>Auto</li></ul></td></tr><tr><td><strong>2</strong></td><td>Manual</td><td>在“Manual”模式下，设置为 <img src="../../../.gitbook/assets/3 (7).png" alt="" data-size="line">时，业主可在App上通过 <img src="../../../.gitbook/assets/4 (4).png" alt="" data-size="line"> 对SG热泵进行开关机。</td></tr><tr><td><strong>3</strong></td><td>Min Running Time</td><td>设置热泵启动后，热泵运行的最小时间。</td></tr><tr><td><strong>4</strong></td><td>PV Residual Power Control</td><td><p>在“Auto”模式下，设置为 <img src="../../../.gitbook/assets/5 (4).png" alt="" data-size="line">:</p><ul><li>当PV余电功率＞“SG Ready Heat Pump Min Starting Power”值，热泵开机。</li><li>当PV余电功率＜“SG Ready Heat Pump Min Starting Power”，热泵关机。</li><li>PV余电功率 = PV功率 - 交流负载功率 - 储能充电功率。</li></ul></td></tr><tr><td><strong>5</strong></td><td>SG Ready Heat Pump Power</td><td>在“Auto”模式下，设置热泵运行时的额定功率。</td></tr><tr><td><strong>6</strong></td><td>SG Ready Heat Pump Min Starting Power</td><td>在“Auto”模式下，设置热泵最小启动功率。</td></tr><tr><td><strong>7</strong></td><td>Max Daily Running Time</td><td>在“Auto”模式下，设置热泵在当天运行的累计最长时间。</td></tr><tr><td><strong>8</strong></td><td>Time of Use</td><td>在“Auto”模式下，设置SG热泵自动开关机的时间段和SOC阈值。</td></tr></tbody></table>
