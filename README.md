# <img src="logo.png" width="400"> #

## EN | [CN](https://github.com/exTHmUI/android/blob/Violet/README_CN.md) ##

### What is this? ###

``exTHmUI`` is an open sourced Chinese localization features Android Project founded by Touhou fans.

### To Sync ###

```bash
# Initialize local repository
$ repo init -u https://github.com/exTHmUI/android -b Violet

# Sync
$ repo sync -j4
```

### To Build ###

```bash
# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch exthm_$device-userdebug

# To build
$ make reimu -j$(nproc --all)
