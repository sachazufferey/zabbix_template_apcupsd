Zabbix Template "apcupsd extended"
==========================

Based on https://github.com/cavazquez/zabbix_template_apcupsd

*A big thanks to cavazquez for the work*

Requirements
------------
* Zabbix Server, tested on :
  * 5.0.4
  * 5.2.1
 * Zabbix Agent
 * apcupsd
 

Installation
------------
* Agent side
  * apcupsd
   > apt install apcupsd -y
   
   * edit the configuration file __/etc/apcupsd/apcupsd.conf__ and comment the following line 
   
   > #DEVICE /dev/ttyS0
   
   reboot and verify by running the following command
   
   > apcaccess
   
   you will get something like this :
   
   > MODEL    : Back-UPS RS  650MI
   > STATUS   : ONLINE
   > LINEV    : 235.0 Volts
  
  * Zabbix Agent
  

* Server side


Values
------------
