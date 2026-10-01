# Dolby Atmos UI (LunarisDolby)

Clean Dolby Atmos application package (`LunarisDolby`) extracted directly from [Pong-Development/hardware_dolby](https://github.com/Pong-Development/hardware_dolby) (branch `16`).

This repository contains **only the application package**, without any device-specific proprietary hardware blobs or conflicting vendor codecs, making it safe to use across devices (including MediaTek `rodin` / Xiaomi 14T / POCO X7 Pro).

## How to use

1. **Clone this repository** into `packages/apps/DolbyUI` in your ROM source:
   ```bash
   git clone https://github.com/khalifam0/packages_apps_DolbyUI.git packages/apps/DolbyUI
   ```

   Or add it to your ROM local manifest (`.repo/local_manifests/dolby.xml`):
   ```xml
   <?xml version="1.0" encoding="UTF-8"?>
   <manifest>
       <project path="packages/apps/DolbyUI" name="khalifam0/packages_apps_DolbyUI" remote="github" revision="16" />
   </manifest>
   ```

2. **Include in `device.mk`**:
   ```makefile
   # Dolby
   PRODUCT_PACKAGES += \
       LunarisDolby
   ```

## Credits
* [Pong-Development/hardware_dolby](https://github.com/Pong-Development/hardware_dolby)
* Paranoid Android / LineageOS
* Lunaris AOSP
