Zabbix-NUT-Template
===================

Zabbix Template for NUT (Network UPS Tools) with automatic UPS discovery
for Zabbix server version 3.2.x

Supported UPSes: http://www.networkupstools.org/stable-hcl.html


# Installation

Value mapping must be done before importing the template. 

1. Import predefined values in **Administration** / **General** / **Value mapping** - **Import** button (zbx_nut_valuemaps.xml)
2. Import the template in **Configuration** / **Templates** - **Import** button (zbx_nut_template.xml)


Predefined value map:

	0  - unknown state
	1  - On line (mains is present)
	2  - On battery (mains is not present)
	3  - Low battery
	4  - The battery needs to be replaced
	5  - The battery is charging
	6  - The battery is discharging (inverter is providing load power)
	7  - UPS bypass circuit is active echo no battery protection is available
	8  - UPS is currently performing runtime calibration (on battery)
	9  - UPS is offline and is not supplying power to the load
	10 - UPS is overloaded
	11 - UPS is trimming incoming voltage (called "buck" in some hardware)
	12 - UPS is boosting incoming voltage
