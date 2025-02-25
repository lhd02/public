# 充放电与备电量

<figure><img src="../../../.gitbook/assets/charge&#x26;discharge.png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="73">序号</th><th width="138">参数名称</th><th>说明</th></tr></thead><tbody><tr><td><strong>1</strong></td><td>Charge Cut-off SOC</td><td>设置电池包停止充电的容量。</td></tr><tr><td><strong>2</strong></td><td>Discharge Cut-off SOC</td><td><p>设置电池包停止放电的容量。</p><ul><li>此参数不建议设置为0，避免电池包未及时充电造成不可逆的衰减。</li><li>在备电组网时，优先执行“Backup Capacity”；非备电组网时，执行此参数。</li></ul></td></tr><tr><td><strong>3</strong></td><td>Backup Reserve SOC</td><td><ul><li>组网中含有Gateway时，可设置此参数。</li><li>并网场景时，电池包放电至备电量值时不再放电；离网场景时，电池包给用电设备供电，放电至设置的Discharge Cut-off SOC时，停止放电。</li><li>用户根据地区断电频率和离家时间手动设置。不建议设置为0，避免电池包未及时充电造成不可逆的衰减.</li></ul></td></tr></tbody></table>
