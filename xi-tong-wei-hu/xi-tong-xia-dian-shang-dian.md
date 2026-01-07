# 系统下电/上电

{% include "../.gitbook/includes/danger.md" %}

<mark style="color:red;">高电压、危险：</mark>

<mark style="color:red;">操作设备时，请穿戴绝缘手套、绝缘鞋、安全帽等防护用具。禁止佩戴金属手镯、戒指、项链等导电饰品。</mark>

## 系统下电

1. 通过App下发关机指令。

### **户主账号**

<figure><img src="../.gitbook/assets/MSA1CM00071-系统下电zh.png" alt=""><figcaption></figcaption></figure>

### **安装商账号**

<figure><img src="../.gitbook/assets/MSA1CM00078-系统下电zh (1).png" alt=""><figcaption></figcaption></figure>

2. 断开备电配电单元内与设备连接的开关。
3. 用钳流表直流电流档测量逆变器每一路输入组串的直流电流。

* 若电流≤0.01A，请执行下一步操作。
* 若电流＞0.01A，需待光伏组串电流降低至0.01A以下时，执行下一步操作。

4. 打开维护腔门，用万用表测量交流端子排对地电压，确保逆变器交流侧已断电。
5. 将逆变器上的所有“DC SWITCH”旋转至“OFF”状态。
6. 长按BC/BC-BST的ON/OFF按钮10s。
7. 逆变器和BC/BC-BST的LED指示灯均熄灭后，请参考设备上延时标签，等待对应的时间后，将BC/BC-BST的隔离开关置于OFF位置。

{% include "../.gitbook/includes/warning.md" %}

<mark style="color:orange;">下电后，设备存在残余电流与余热。下电后立马操作，可能会造成触电与灼伤。</mark>

## 系统上电

1. 将BC/BC-BST的隔离开关置于ON位置。
2. 长按BC/BC-BST的ON/OFF按钮10s。
3. 闭合备电配电单元内与设备连接的开关。
4. 将逆变器上的所有“DC SWITCH”旋转至“ON”状态。
5. 观察逆变器和BC/BC-BST的LED指示灯状态，通过App下发开机指令，（操作步骤参见“系统下电”的步骤1描述）
