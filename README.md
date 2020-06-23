# deb-zephyr
Debian/Ubuntu packages for Zephyr RTOS development tools

## Release Procedure

### zephyr-crosstool-*

1. Build `zephyr-crosstool-ng` package
    1. Update [`zephyr-crosstool-ng` package `changelog`](https://github.com/stephanosio/deb-zephyr/blob/master/zephyr-crosstool-ng/changelog)
    2. Sync [LaunchPad `zephyr-crosstool-ng` repository](https://code.launchpad.net/~zephyrproject-rtos/zephyr-crosstool-ng/+git/zephyr-crosstool-ng)
    3. Sync [LaunchPad `deb-zephyr` repository](https://code.launchpad.net/~zephyrproject-rtos/deb-zephyr/+git/deb-zephyr)
    4. Build [LaunchPad `release-zephyr-crosstool-ng` recipe](https://code.launchpad.net/~zephyrproject-rtos/+recipe/release-zephyr-crosstool-ng)

2. Build `zephyr-crosstool-*` packages
    1. Update `zephyr-crosstool-*` package `changelog`s
    2. Sync [LaunchPad `zephyr-crosstool-ng-cache` repository](https://code.launchpad.net/~zephyrproject-rtos/zephyr-crosstool-ng-cache/+git/zephyr-crosstool-ng-cache)
    3. Sync [LaunchPad `zephyr-crosstool-deb-template` repository](https://code.launchpad.net/~zephyrproject-rtos/zephyr-crosstool-deb-template/+git/zephyr-crosstool-deb-template)
    4. Sync [LaunchPad `deb-zephyr` repository](https://code.launchpad.net/~zephyrproject-rtos/deb-zephyr/+git/deb-zephyr)
    5. Build [LaunchPad `release-zephyr-crosstool-*` recipes](https://code.launchpad.net/~zephyrproject-rtos/zephyr-crosstool-deb-template/+git/zephyr-crosstool-deb-template/+recipes)
 
 3. Build `zephyr-crosstool` metapackage
    1. Update [`zephyr-crosstool` package `changelog`](https://github.com/stephanosio/deb-zephyr/blob/master/zephyr-crosstool/changelog)
    2. Update [`zephyr-crosstool` package `control` dependency version](https://github.com/stephanosio/deb-zephyr/blob/master/zephyr-crosstool/control)
    3. Sync [LaunchPad `deb-zephyr` repository](https://code.launchpad.net/~zephyrproject-rtos/deb-zephyr/+git/deb-zephyr)
    4. Build [LaunchPad `release-zephyr-crosstool` recipe](https://code.launchpad.net/~zephyrproject-rtos/+recipe/release-zephyr-crosstool)

### zephyr-qemu

1. Sync [LaunchPad `zephyr-qemu` submodule repositories](https://code.launchpad.net/~zephyrproject-rtos/zephyr-qemu)
    1. Sync [LaunchPad `zephyr-qemu/capstone` repository](https://code.launchpad.net/~zephyrproject-rtos/zephyr-qemu/+git/capstone)
    2. Sync [LaunchPad `zephyr-qemu/dtc` repository](https://code.launchpad.net/~zephyrproject-rtos/zephyr-qemu/+git/dtc)
    3. Sync [LaunchPad `zephyr-qemu/berkeley-testfloat-3` repository](https://code.launchpad.net/~zephyrproject-rtos/zephyr-qemu/+git/berkeley-testfloat-3)
    4. Sync [LaunchPad `zephyr-qemu/berkeley-softfloat-3` repository](https://code.launchpad.net/~zephyrproject-rtos/zephyr-qemu/+git/berkeley-softfloat-3)
    5. Sync [LaunchPad `zephyr-qemu/keycodemapdb` repository](https://code.launchpad.net/~zephyrproject-rtos/zephyr-qemu/+git/keycodemapdb)

2. Sync [LaunchPad `zephyr-qemu` repository](https://code.launchpad.net/~zephyrproject-rtos/zephyr-qemu/+git/zephyr-qemu)

3. Build [LaunchPad `release-zephyr-qemu` recipe](https://code.launchpad.net/~zephyrproject-rtos/+recipe/release-zephyr-qemu)
