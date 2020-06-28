# POSP Croquette

### How to build ###

```bash
# Create dirs
$ mkdir posp ; cd posp

# Init repo
$ repo init --depth=1 -u https://github.com/PotatoProject/manifest -b croquette-release

# Clone local manifest
$ git clone https://gitlab.com/android_samsung_universal7870/manifest/android_manifest_samsung_j7xelte.git -b potato .repo/local_manifests

# Sync
$ repo sync --force-sync

# Build
For 8GB RAM
$ . build/envsetup.sh && lunch potato_j7xelte-userdebug && mka clean && mka api-stubs-docs && mka hiddenapi-lists-docs && mka system-api-stubs-docs && mka test-api-stubs-docs && mka bacon -j`nproc`

For 16GB RAM or more 
$ . build/envsetup.sh && mka clean && brunch potato_j7xelte-userdebug
```

## Credits
2019 @Astrako, POSP and LOS branches kept up to date by @Sap1k

## Contact
Telegram support group: https://t.me/joinchat/D1Jk_VbieGBXOWZt2y8O7A
