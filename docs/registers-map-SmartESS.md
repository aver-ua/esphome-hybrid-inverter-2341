System Info [4501-4515,4517-4529,4535-4553], Fault [4529-4530], Other [4531-4534]:
- 4501 : Working State ["7": "ShutDown", "3": "Invert Mode", "4": "Line Mode", "0": "Power On", "5": "Bypass", "1": "Test", "6": "Fault Mode", "2": "Stand By"]
- 4502 : AC input voltage, V
- 4503 : AC input frequency, Hz
- 4504 : PV input voltage, V
- 4505 : PV input power, W
- 4506 : Battery Voltage, V
- 4507 : Battery capacity %
- 4508 : Charging current, A
- 4509 : Battery discharge current, A
- 4510 : Output voltage, V, scale: 0.1
- 4511 : Output frequency, Hz, scale: 0.1
- 4512 : Output apparent power, VA
- 4513 : Output active power, W
- 4514 : AC output Load %
- 4515 : Load Percent
- 4517 : Machine Type ["0": "Solar Inverter", "1": "Voltage regulator"]
- 4518 : Main CPU version
- 4519 : Secondary CPU version
- 4520 : Battery Piece ["0": "no battery", "1": "24V（3KW）", "2": "48V（5KW)"]
- 4521 : Nonimal output apparent power, VA
- 4522 : Nonimal output active power, W
- 4523 : Nominal AC voltage, V
- 4524 : Nominal AC current, A
- 4525 : Rated battery voltage, V, scale: 0.1
- 4526 : Nominal output voltage, V
- 4527 : Nominal output frequency, Hz, scale: 0.1
- 4528 : Nominal output current, A
- 4529 : Error Code, binary: "0" - normal, "1" - fault. 
         Bits: [0:"Fan locked",1:"Over Temperater",2:"Battery Voltage High",
		        3:"Battery Voltage Low",4:"Output shorted",5:"INV Voltage Over",
				6:"Over Load",7:"Bus Voltage Over",8:"Bus Soft Failed",
				9:"PV Voltage High",10:"Over Current",11:"Bus Voltage Under",
				12:"INV Soft Failed",13:"DC Voltage Over",14:"CT Fault",
				15:"INV Voltage Low"] 
- 4530 : Alarm Code, binary: binary: "0" - normal, "1" - alarm.
         Bits: [0:"Fan locked",1:"Over Temperater",2:"Battery Over Charged",
		        3:"Battery Voltage Low",4:"Over Load",5:"Output Power Derating",
				6:"PV Energy Weak",7:"AC Voltage High",8:"No Battery"]
- 4531 : ID1
- 4532 : ID2
- 4533 : ID3
- 4534 : ID4
- 4535 : Settings state, binary: "0" - disable, "1" - enable.
         Bits: [0:"Buzzer alarm",1:"Power saving mode",2:"LCD backlight",
                3:"Overload auto restart",4:"Over temperature auto restart",5:"Beeps while primary source interupt",
				6:"Auto return to default display screen",7:"Transfer to bypass @ overload,8:"Record fault code",
				9:"Battery Equalization",10:"Battery Equalization activated immediately"]
- 4536 : Charger Source Priority 
- 4537 : Output Source Priority ["0": "Utility (default)", "1": "Solar", "2": "SBU"]
- 4538 : AC input range ["0": "Appliances (default)", "1": "UPS"]
- 4539 : Battery type ["0": "AGM (default)","1": "Flooded","2": "User"]
- 4540 : Output Frequency ["0": "50Hz(default)","1": "60Hz"]
- 4541 : Max total charge current
- 4542 : Output voltage ["220": "220V", "230": "230V", "240": "240V"]
- 4543 : Max utility charge current
- 4544 : Comeback utility mode voltage point under "SBU priority"
- 4545 : Comeback battery mode voltage point under "SBU priority"
- 4546 : Bulk charging voltage, V, scale: 0.1
- 4547 : Floating charging voltage, V, scale: 0.1
- 4548 : Low Battery cut-off voltage, V, scale: 0.1
- 4549 : Battery Equalization voltage, V, scale: 0.1
- 4550 : Battery Equalized time, min
- 4551 : Battery Equalized timeout, min
- 4552 : Battery Equalization interval, day
- 4553 : APPShows, binary.
         * bits 0-1: Battery state ["3": "Ok","1": "Discharging","2": "Charging","0": "Disconnected"]
         * bits 2-3: PV state ["3": "Ok","1": "Discharging","2": "Overvoltage","0": "Undervoltage"]
         * bits 4-5: Mains supply state ["3": "Ok","1": "Absorption","2": "Discharging","0": "Abnormal"]
         * bits 6-7: Load state ["0": "Off","1": "Normal","2": "Overload"]
		 
- 4554 : Today Energy, KWH, scale: 0.01 (? 2 registers, 4 bytes)
- 4556 : Month Energy, KWH, scale: 0.01 (? 2 registers, 4 bytes)
- 4558 : Year Energy, KWH, scale: 0.01 (? 2 registers, 4 bytes)
- 4560 : All Energy, KWH, scale: 0.01 (? 2 registers, 4 bytes)

System settings [5001-5012, 5016-5033]:
- 5001 : Remove all power history ["0": "Do nothing","1": "Remove all power history"]
- 5002 : Buzzer alarm ["0": "disable","1": "enable"]
- 5003 : Power saving mode ["0": "disable","1": "enable"]
- 5004 : LCD backlight ["0": "disable","1": "enable"]
- 5005 : Overload auto restart ["0": "disable","1": "enable"]
- 5006 : Over temperature auto restart ["0": "disable","1": "enable"]
- 5007 : Beeps while primary source interupt ["0": "disable","1": "enable"]
- 5008 : Auto return to default display screen ["0": "disable","1": "enable"]
- 5009 : Transfer to bypass @ overload ["0": "disable","1": "enable"]
- 5010 : Record fault code ["0": "disable","1": "enable"]
- 5011 : Battery Equalization ["0": "disable","1": "enable"]
- 5012 : Battery Equalization activated immediately ["0": "disable","1": "enable"]
- 5016 : Restore Defaults ["0": "disable","1": "enable"]
- 5017 : Charger source priority ["3": "Solar only","1": "Solar","2": "Utility or Solar (default)","0": "Utility"]
- 5018 : Output Source priority ["0": "Utility (default)","1": "Solar","2": "SBU"]
- 5019 : AC input range ["0": "Appliances (default)","1": "UPS"]
- 5020 : Battery type ["0": "AGM (default)","1": "Flooded","2": "User"]
- 5021 : Output Frequency ["0": "50Hz (default)","1": "60Hz"]
- 5022 : Max total charge current
- 5023 : Output voltage ["220": "220V","230": "230V (default)","240": "240V"]
- 5024 : Max utility charge current
- 5025 : Comeback utility mode voltage point under "SBU priority". 12V: 10.5-15.0 (step 0.5) 24V: 21.0-25.5 (step 0.5) 48V: 45-51 (step 1). multiply: 10
- 5026 : Comeback battery mode voltage point under "SBU priority". 12V: 12.0-17.0 (step 0.5) 24V: 24.0-29.0 (step 0.5) 48V: 48-58 (step 1). multiply: 10
- 5027 : Bulk charging voltage. 12V: 12.5-15.5 24V: 25.0-31.5 48V: 48-61 (step 0.1). multiply: 10
- 5028 : Floting charging voltage. 12V: 12.5-15.5 24V: 25.0-31.5 48V: 48-61 (step 0.1). multiply: 10 
- 5029 : Low Battery cut-off voltage. 12V: 10-12 24V: 20-24 48V: 40-48 (step 0.1). multiply: 10
- 5030 : Battery Equalization voltage. 24V: 25.0-31.5 48V: 48-61 (step 0.1). multiply: 10
- 5031 : Battery Equalized time. 5-900 min (step 5)
- 5032 : Battery Equalized timeout. 5-900 min (step 5)
- 5033 : Battery Equalization interval. 0-90 day (step 1)

Time settings [6030-6035]:
- 6030 : System time setting - year
- 6031 : System time setting - month
- 6032 : System time setting - day
- 6033 : System time setting - hour
- 6034 : System time setting - min
- 6035 : System time setting - second