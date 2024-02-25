# HP ProBook 440 G1 EFI Boot loader

![Screen Shot 2567-02-25 at 19 49 44](https://github.com/whyzotee/hp-probook-440-g1-hackintosh-efi/assets/53619535/c56d1a90-2772-49a4-b2e2-2751113ea6cb)

Setup for usb device or flashdrive to boot macos recovery mode and install macOS Monterey 12.7.3 on laptop hp probook 440 g1

### Requiment

**Hardware:** HP Probook 440 G1, Flashdrive 16gb format type FAT32, Lan Network

**Softwave:** OpenCore 0.9.8, ProperTree (For adding extension), Python 3

### follow steps

```py
1. paste this link in browser and download OpenCore-0.9.8-RELEASE.zip file
https://github.com/acidanthera/OpenCorePkg/releases/tag/0.9.8

2. extract OpenCore-0.9.8-RELEASE.zip file

3. go to folder
OpenCore-0.9.8-RELEASE/Utilities/macrecovery

4. run this command in cmd
python macrecovery.py -b Mac-FFE5EF870D7BA81A -m 00000000000000000 download

5. git clone https://github.com/whyzotee/hp-probook-440-g1-hackintosh-efi.git

6. go to folder
OpenCore-0.9.8-RELEASE/Utilities/macrecovery/com.apple.recovery.boot

7. copy all files in folder
BaseSystem.chunklist and BaseSystem.dmg

8. go to folder and paste it
hp-probook-440-g1-hackintosh-efi/com.apple.recovery.boot

9. copy all files and folder in hp-probook-440-g1-hackintosh-efi to your usb
```

### BIOS SETTING

Disable

- Fast Boot
- SecureBoot
- Clear SecureBoot Keys

Enable

- User Mode Hp Factory Keys
- Boot Mode UEFI Hybrid (With CSM)
- Virtualization Technology (VRx)
- Video memory size 512MB

### Specs

#### HP ProBook 440 G1

| Name  | Hardware          |
| :---- | :---------------- |
| `CPU` | `Intel i7-4712MQ` |
| `GPU` | `Intel HD 4600`   |
| `RAM` | `8GB DDR3`        |
| `SSD` | `256GB`           |
