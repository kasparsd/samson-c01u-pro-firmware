# Samon C01U Pro Firmware

Back in September of 2015 Samson released a firmware upgrade for the [Samson C01U Pro](http://www.samsontech.com/samson/products/microphones/usb-microphones/c01upro/) microphone with [a faulty upgrade tool which wiped out all USB configuration for the microphone](https://twitter.com/konstruktors/status/643539539991089155) which has since been removed from their website.

Use the [CM65XX EEPROM Configuration Tool](cm65xx-configuration-tool/Config65XX.exe) to write the [CM6500_Headset_Samson_C01U_Pro-0109.bin](CM6500_Headset_Samson_C01U_Pro-0109.bin) firmware to the EEPROM.

See [instructions](docs/c01u-pro-downgrade-instructions.jpg):

- Clone or download this whole repository.

- Run `Config65XX.exe` inside the `cm65xx-configuration-tool` directory.

- In `VID` enter `0d8c`, in `PID` enter `0178`.

- In `EEPROM TYPE` select `S24C32`.

- Press "Connect". It will probably say "EEPROM empty".

- Click "FILE → EEPROM" and select `CM6500_Headset_Samson_C01U_Pro-0109.bin`.

- Press "Open". It should say "File → EEPROM completely."

- Unplug and re-plug the microphone and it should be back to "Samson C01U Pro Mic".