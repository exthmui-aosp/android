# <img src="https://github.com/exthmui-aosp/android/blob/baka/logo.png" width="400"> #

## [EN](https://github.com/exthmui-aosp/android) | CN ##

### 这是什么？ ###

``exTHmUI`` 是一个由国内东方众维护的，基于AOSP的东方化系统。

### 如何同步 ###

```bash
# 初始化空的索引仓库
$ repo init -u https://github.com/exthmui-aosp/android -b baka

# 开始同步仓库
$ repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### 如何编译 ###

```bash
# 初始化编译环境
$ . build/envsetup.sh

# 选择编译设备
$ lunch exthm_$device-$aosp_target_release-userdebug

# 开始编译!!
$ m baka -j$(nproc --all)
