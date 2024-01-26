# Lineage OS Android 12.1

### How to build ###

```bash
# Create dirs
$ mkdir lineage && cd lineage

# Init repo
$ repo init -u https://github.com/LineageOS-UL/android.git -b lineage-19.1 --git-lfs
(already patched for ultra legacy devices) or use
$ repo init -u https://github.com/LineageOS/android.git -b lineage-19.1 --git-lfs
(still needs to be patched for ultra legacy devices)

# Clone my local repo
$ git clone https://github.com/samsungexynos7870/android_manifest_samsung_j7xelte.git -b lineage-19.1-oss_bsp-vndk .repo/local_manifests

# Sync
$ repo sync --no-repo-verify -c --force-sync --no-clone-bundle --no-tags --optimized-fetch --prune -j`nproc` -v

# Build
$ . build/envsetup.sh && brunch lineage_j7xelte-user
```

## Credits
2021 @Astrako 2022 @FlominatorGD 2024 @GonicDroid

## Contact
None.
