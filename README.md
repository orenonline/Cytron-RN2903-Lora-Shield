# Cytron-RN2903-Lora-Shield
Arduino UNO RN2903 Lora Shield code.  The Lora shield is from Cytron Malaysia.  The code was based on Haxiot example.

The code is tailored to work with my Single Channel Packet Forwarder (Raspberry Pi + RFM95 Lora Shield).  
FYI, i requested Cytron to flash Australia firmware into the shield. The tricky part is to wash off all the unwanted channels from being used. There are 71 channels altogether (original code has 64 channels - US region), ie from 915.2 to 928 MHz. Since we want to only work with 1 channel (in this case is Channel 24), i need to off the rest of the channels.

Since SCPF is set to use SF7, i also forced the channel to use SF7.

How to use?

Download Haxiot RN2903 library first.  The you can replace the library files with the files here.  Run the .ino, flash to the Arduino as usual.



