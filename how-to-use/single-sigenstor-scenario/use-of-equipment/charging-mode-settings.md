# Charging Mode Settings

![](<../../../.gitbook/assets/0 (7).png>)

### **Fast Charging**

After the PV power generation meets the load, the surplus PV power + battery pack discharging power + grid input power are used together for SigenStor EVDC charging.

* When the surplus PV power is greater than or equal to the "Charging power allowed for EVDC" set value, the SigenStor EVDC will charge according to the set value, and the surplus PV power will be used to charge the battery pack.
* When the surplus PV power + total battery pack power is greater than or equal to the "Charging power allowed for EVDC" set value, the SigenStor EVDC charges according to the set value.
* When the surplus PV power + total battery pack power + grid input power is greater than or equal to the "Charging power allowed for EVDC" set value, the SigenStor EVDC will charge according to the set value.
* When the surplus PV power + total battery pack power + grid input power is less than the "Charging power allowed for EVDC" set value, SigenStor EVDC charges according to the surplus PV power + total battery pack power + grid input power.
* The system will send a notification to your vehicle when the surplus PV power + total battery pack power + grid input power is less than 1 kW.

### **PV Surplus Charging (EVDC** ＞ **Battery)**

After the PV power generation meets the load, the surplus PV power is used to charge the SigenStor EVDC and any surplus power is used to charge the battery pack.

* When the surplus PV power is greater than or equal to the "Charging power allowed for EVDC" set value, the SigenStor EVDC will charge according to the set value, and the surplus power is used to charge the battery pack.
* When the surplus PV power is less than the "Charging power allowed for EVDC" set value, SigenStor EVDC charges according to the surplus PV power + battery pack discharging power.
* The system sends a notification to your vehicle when the surplus PV power is zero or negative.

### **PV Surplus Charging (Battery** ＞ **EVDC)**

After the PV power generation meets the load, the surplus PV power is used to charge the battery pack first, and any surplus power is used to charge the SigenStor EVDC.

* When the surplus PV power is sufficient to charge the battery pack, and there is still surplus power greater than or equal to the "Charging power allowed for EVDC" set value, SigenStor EVDC charges according to the set value.
* When the surplus PV power is sufficient to charge the battery pack, and the surplus power is less than the "Charging power allowed for EVDC" set value, SigenStor EVDC will charge according to the surplus power.
* The system sends a notification to your vehicle when the surplus PV power is zero or negative.
