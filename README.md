# Edge-o-Matic 3000 with Solenoid control

This is a variation of the firmware for the Edge-o-Matic 3000 by Maustec that adds a "Solenoid mode" which outputs a binary on/off at a certain BPM instead of the PWM signal for a vibrator motor.

## Warnings and Cautions

Use at your own risk. BACK UP YOUR CONFIG FILE on your SD Card before using. If you revert to the official firmware you'll need to reload your original config file. 
You can't upload this and then complain to Maustec when something stops working. 

This version adds three new config values to the configuration file. 

|Key|Type|Default|Note|
|---|----|---|---|
|`mode_select`|Boolean|"0"|Default mode, solenoid (0) or motor (1).|
|`minimum_bpm`|Int|40|Minimum beats per minute.|
|`maximum_bpm`|Int|750|Maximum beats per minute.|


### Added functions:
In the main menu, there is now a checkbox that toggles between Solenoid Mode and Motor Mode.
In the Edging Settings menu, there is now an option to set a Minimum and Maximum BPM.

All other functionality remains the same.

---

Maus-Bus and Maus-Link are trademarks of Maus-Tec LLC. Edge-o-Matic is a registered trademark of Maus-Tec LLC. If you are
a 3rd party hardware manufacturer looking to certify your Maus-Bus connected device for use with the Edge-o-Matic, we 
encourage you to contact info@maustec.io and our friendly customer support robot will be glad to assist!
