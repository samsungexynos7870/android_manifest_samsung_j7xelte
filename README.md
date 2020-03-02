# Skyhawk Recovery Project

### How to build ###

```bash
# Create dirs
$ mkdir skyhawk ; cd skyhawk

# Init repo
$ repo init --depth=1 -u git://github.com/SKYHAWK-Recovery-Project/platform_manifest_twrp_omni.git -b 9.0

# Clone my local repo
$ git clone https://gitlab.com/android_samsung_universal7870/manifest/android_manifest_samsung_j7xelte.git -b skyhawk .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc`

# Build
$ mv device/samsung/j7xelte/build_skyhawk.sh .
$ . build_skyhawk.sh j7xelte
```

## Credits
2019 @Astrako

## Contact
Telegram support group: https://t.me/joinchat/D1Jk_VbieGBXOWZt2y8O7A
