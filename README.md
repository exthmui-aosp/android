# <img src="https://github.com/exthmui-aosp/android/blob/baka/logo.png" width="400"> #

## EN | [CN](https://github.com/exthmui-aosp/android/blob/baka/README_CN.md) ##

### What is this? ###

``exTHmUI`` is an open sourced Android Project founded by Touhou fans.

### To Sync ###

```bash
# Initialize local repository
$ repo init -u https://github.com/exthmui-aosp/android -b baka

# Sync
$ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### To Build ###

```bash
# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch exthm_$device-$aosp_target_release-userdebug

# To build
$ m baka -j$(nproc --all)
