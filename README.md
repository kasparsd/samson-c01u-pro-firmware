# Samon C01U Pro Firmware

Back in September of 2015 Samson released a firmware upgrade for the [Samson C01U Pro](http://www.samsontech.com/samson/products/microphones/usb-microphones/c01upro/) microphone with [a faulty upgrade tool which wiped out all USB configuration for the microphone](https://twitter.com/konstruktors/status/643539539991089155) which has since been removed from their website.

Use the [CM65XX EEPROM Configuration Tool](cm65xx-configuration-tool/Config65XX.exe) to write the correct firmware to the EEPROM:
[CM6500_Headset_Samson_C01U_Pro-0109.bin](CM6500_Headset_Samson_C01U_Pro-0109.bin) for 6500.
[CM6500B_Headset_Samson_C01U_Pro-0201.bin](CM6500B_Headset_Samson_C01U_Pro-0201.bin) for 6500B.

See [instructions - 6500](docs/c01u-pro-downgrade-instructions.jpg)
See [instructions - 6500B](docs/c01u-pro-6500B-downgrade-instructions.jpg)

- Clone or download this whole repository.

- Run `Config65XX.exe` inside the `cm65xx-configuration-tool` directory.

- In `VID` enter `0d8c`.

- In `PID` enter `0178`(for 6500) or `0170`(for 6500B).

- In `EEPROM TYPE` select `S24C32`.

- Press "Connect". It will probably say "EEPROM empty".

- Click "FILE → EEPROM" and select `CM6500_Headset_Samson_C01U_Pro-0109.bin`(for 6500) or `CM6500B_Headset_Samson_C01U_Pro-0201.bin`(for 6500B).

- Press "Open". It should say "File → EEPROM completely."

- Unplug and re-plug the microphone and it should be back to "Samson C01U Pro Mic".

[Identifying chip](docs/Example-6500B-Chip.jpg)
[Opening mic 1](docs/Opening-Mic-1.jpg)
[Opening mic 2](Opening-Mic-2.jpg)