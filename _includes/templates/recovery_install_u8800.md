## Installing a custom recovery

{% include note.html content="The steps below only need to be run once per device." %}
Legacy Huawei devices come with a "pink screen mode" which basically mounts an EMMC partition that gives access to various system images like recovery.img and boot.img.
This guide will teach you how to access this mode using the correct bootloader that is not locked by later versions from Huawei as well as on how to install the recovery. 

1. Download and install [update-B518-bootloader.zip](http://www.mediafire.com/?l5ja3ficb39bnud) for u8800.
    1. Save it to the root of your SD Card.
    2. Select "install zip from sdcard"
    3. Select "chooze zip from sdcard"
    4. Select the zip you downloaded before.
    5. Select yes.
2. Reboot into "pink screen mode" by pressing the VOLUME-UP, VOLUME-DOWN and POWER buttons simultaneously until a pink screen appears.
3. Insert the USB cable into the device and replace the recovery.img file in the root directory with your custom recovery.
    {% include note.html content="Be sure that your custom recovery image is renamed to recovery.img and you might want to back up the original recovery.img." %}
4. Manually reboot into recovery: {{ site.data.devices[page.device].recovery_boot }}
5. Congratulations! Your {{ site.data.devices[page.device].name }} now has a custom recovery installed. Continue on to the next section.
