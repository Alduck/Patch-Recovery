# Fastbootd Recovery Patch for Samsung devices.
This script patches recovery images of Samsung devices to enable Fastbootd. 
Based on Phh's [script.](https://github.com/phhusson/samsung-galaxy-a51-gsi-boot)

# How to use:

# FOR A ONLY DEVICES 
- Download your desired build from samfw or any other reliable source.
- Extract it, and then extract the AP file.
- Look at the AP file for recovery.img.lz4. Copy it to somewhere you'll remember.
- Fork this repo.
- Extract your recovery.img.lz4 and upload recovery.img or *img.lz4 to [catbox.](https://catbox.moe/) 
- Head over to Actions tab. Click on RECOVERY -> Run workflow. Insert the copied URL in the RECOVERY URL field and Start the workflow
- The Patching process will start.
- A Patched-Recovery.zip will be uploaded at the end of the process. Download it and extract your patched recovery image. The Image will already also be repacked to .tar for flashing directly through Odin.
- Flash your own patched vbmeta if needed.

```
ODIN AP Slot: fastbootd-recovery.tar.md5
ODIN Userdata Slot: vbmeta_disabled.tar
```

# FOR A/B DEVICES (example: Galaxy S25 series)
- Download your desired build from samfw or any other reliable source.
- Extract it, and then extract the AP file.
- Look at the AP file for vendor_boot.img.lz4. Copy it to somewhere you'll remember.
- Fork this repo.
- Extract your vendor_boot.img.lz4 and upload vendor_boot.img or *img.lz4 to [catbox.](https://catbox.moe/) 
- Head over to Actions tab. Click on VENDOR_BOOT -> Run workflow. Insert the copied URL in the VENDOR_BOOT URL field and Start the workflow
- The Patching process will start.
- A Patched-VENDOR_BOOT.zip will be uploaded at the end of the process. Download it and extract your patched vendor_boot image. The Image will already also be repacked to .tar for flashing directly through Odin.
- Flash your own patched vbmeta if needed.

```
ODIN AP Slot: fastbootd-vendor_boot.tar.md5
ODIN Userdata Slot: vbmeta_disabled.tar
```

# Important note
- Make sure you can download the file with the wget command. Catbox works fine.

# Credits
- [Phhusson](https://github.com/phhusson) Without his script nothing would be possible at the first place
- [James Nguyen](https://github.com/thongass000) Helping me in simplifying the scripts and tweaking it
- [Johx22](https://github.com/Johx22) Revamped scripts
