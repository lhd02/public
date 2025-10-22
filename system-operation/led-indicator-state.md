# LED Indicator State

## **Inverter Indicator**

{% include "https://app.gitbook.com/s/LphsQhUSDX9PgTtjDfX5/~/reusable/ufcMPIm1Yd46Pj7Ir1ce/" %}

<mark style="color:blue;">There are two types of indicators: a yellow indicator, see Light Language 1, and a blue indicator, see Light Language 2.</mark>

### Light Language 1

![](../.gitbook/assets/SSA1OV00015-EN.png)

<figure><img src="../.gitbook/assets/SHA1OV00012-en黄.png" alt=""><figcaption></figcaption></figure>

### Light Language 2

![](../.gitbook/assets/SSA1OV00015-EN.png)

<figure><img src="../.gitbook/assets/SHA1OV00012-en蓝.png" alt=""><figcaption></figcaption></figure>

## **Sigen CommMod Indicator**

<figure><img src="../.gitbook/assets/SCA1OV00001.jpg" alt="" width="188"><figcaption></figcaption></figure>

<table><thead><tr><th width="57.50506591796875" align="center">S/N</th><th>Name</th><th>State</th><th>Description</th></tr></thead><tbody><tr><td align="center">1</td><td>Power indicator</td><td>-</td><td>-</td></tr><tr><td align="center">2</td><td>Network state indicator</td><td>Slow flashing (200 ms on/1800 ms off)</td><td>The network is being connected</td></tr><tr><td align="center">2</td><td>Network state indicator</td><td>Slow flashing (1800 ms on/200 ms off)</td><td>Standby</td></tr><tr><td align="center">2</td><td>Network state indicator</td><td>Quick flashing (125 ms on/125 ms off)</td><td>Data is being transferred</td></tr></tbody></table>

## Sigen Data Logger indicator

<figure><img src="../.gitbook/assets/SLA1OV00004-01.png" alt="" width="237"><figcaption></figcaption></figure>

<table><thead><tr><th width="68.99993896484375" align="center" valign="middle">No.</th><th width="189.22216796875" valign="middle">Indicator</th><th width="105.6666259765625" align="center" valign="middle">Color</th><th width="100.111083984375" valign="middle">Status</th><th valign="top">Meaning</th></tr></thead><tbody><tr><td align="center" valign="middle">1</td><td valign="middle">Running light</td><td align="center" valign="middle"><img src="../.gitbook/assets/绿 闪 (1) (1).png" alt="" data-size="original"></td><td valign="middle">Always on</td><td valign="top">Normal operation (500ms ON / 500ms OFF cycle)</td></tr><tr><td align="center" valign="middle">2</td><td valign="middle">Running light</td><td align="center" valign="middle"><img src="data:image/png;base64,R0lGODlhTAANAHcAMSH+GlNvZnR3YXJlOiBNaWNyb3NvZnQgT2ZmaWNlACH5BAEAAAAALAAAAABMAA0AgwAAALOys7i3uLOxs7y7vLm4uba1tra0trSxtMLBwgECAwECAwECAwECAwECAwECAwRYEARJp6346sy37+A0EGRpnmiqrmyrJkEsz3Rt33iu48Xu/8AgrScsGo/Eo3KZSzKfUCd0iqRaq9csUKrt2nqGsHhMLpvP6LT6TAgM3vC4fE6v2+/4+gERAQA7" alt="" data-size="original"></td><td valign="middle">–</td><td valign="top">Abnormal operation</td></tr><tr><td align="center" valign="middle">3</td><td valign="middle">Communication light</td><td align="center" valign="middle"><img src="data:image/png;base64,R0lGODlhTAANAHcAMSH+GlNvZnR3YXJlOiBNaWNyb3NvZnQgT2ZmaWNlACH5BAEAAAAALAAAAABMAA0AgwAAAC+fTy6fTjCkUTCnUjKsVS6gTy+iTzGnUi+iUC2gTgECAwECAwECAwECAwECAwRTEARJp6346sy37+AkEGRpnmiqrmyrFoYgz3Rt33iu7/gQ88CgcDjzEY/IpDHJbOqWzqgUKq0qf9Yskart7rjesM13KJvP6LR6zW671wiseE5LKCIAOw==" alt=""></td><td valign="middle">Always on</td><td valign="top">The management system has been connected via FE or WLAN.</td></tr><tr><td align="center" valign="middle">4</td><td valign="middle">Communication light</td><td align="center" valign="middle"><img src="data:image/png;base64,R0lGODlhTAANAHcAMSH+GlNvZnR3YXJlOiBNaWNyb3NvZnQgT2ZmaWNlACH5BAEAAAAALAAAAABMAA0AgwAAALOys7i3uLOxs7y7vLm4uba1tra0trSxtMLBwgECAwECAwECAwECAwECAwECAwRYEARJp6346sy37+A0EGRpnmiqrmyrJkEsz3Rt33iu48Xu/8AgrScsGo/Eo3KZSzKfUCd0iqRaq9csUKrt2nqGsHhMLpvP6LT6TAgM3vC4fE6v2+/4+gERAQA7" alt=""></td><td valign="middle">–</td><td valign="top">Communication error.</td></tr><tr><td align="center" valign="middle">5</td><td valign="middle">Fault light</td><td align="center" valign="middle"><img src="data:image/png;base64,R0lGODlhTAANAHcAMSH+GlNvZnR3YXJlOiBNaWNyb3NvZnQgT2ZmaWNlACH5BAEAAAAALAAAAABMAA0AgwAAANgdHdweHtcdHd8eHtwdHdceHucfH+MeHgECAwECAwECAwECAwECAwECAwECAwRYEARJp6346sy37+A0EGRpnmiqrmyrHkEsz3Rt33iu48Tu/8AgrScsGo/Eo3KZSzKfUCd0iqRaq9csUKrt2nqFsHhMLpvP6LT6jAgM3vC4fE6v2+/4usAQAQA7" alt=""></td><td valign="middle">Always on</td><td valign="top">System alarm.</td></tr><tr><td align="center" valign="middle">6</td><td valign="middle">Fault light</td><td align="center" valign="middle"><img src="data:image/png;base64,R0lGODlhTAANAHcAMSH+GlNvZnR3YXJlOiBNaWNyb3NvZnQgT2ZmaWNlACH5BAEAAAAALAAAAABMAA0AgwAAALOys7i3uLOxs7y7vLm4uba1tra0trSxtMLBwgECAwECAwECAwECAwECAwECAwRYEARJp6346sy37+A0EGRpnmiqrmyrJkEsz3Rt33iu48Xu/8AgrScsGo/Eo3KZSzKfUCd0iqRaq9csUKrt2nqGsHhMLpvP6LT6TAgM3vC4fE6v2+/4+gERAQA7" alt=""></td><td valign="middle">–</td><td valign="top">The system has no alarms.</td></tr></tbody></table>
