# about-android-device-tree

for beaglebone black android

in .dts part-number="XXXXX" should match lcd EEPROM

and build .dts to .dtbo

dtc -O dtb -o XXX.dtbo -b 0 -@ XXX.dts

copy .dtbo into /system/vendor/firmware 

and echo XXXXX > /sys/devices/bone_capemgr.9/slots

           ^
           |
           |
           |
       part-number
