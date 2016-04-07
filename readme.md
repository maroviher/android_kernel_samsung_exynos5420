## SM-T520 WiFi CyanogenMod 12.1 Kernel lite
This is an original CyanogenMod 12.1 Kernel for SM-T520 WiFi with a lot of removed debug stuff, that normal users do not need in a daily use.
Kernel size reduced by about 13%, from original 6221824 to 5492736 bytes.
It brings better battery life and performance.

## removed:
- CONFIG_PRINTK
- CONFIG_SEC_LOG
- CONFIG_ANDROID_LOGGER (the android Logger is since Android 5.1 in the userspace)
- CONFIG_EXT2_FS (ext2 is still supported throught ext4 backward compatibility)
- CONFIG_SCHED_DEBUG
- CONFIG_DEBUG_PREEMPT
- CONFIG_DEBUG_RT_MUTEXES
- CONFIG_DEBUG_PI_LIST
- CONFIG_DEBUG_SPINLOCK
- CONFIG_DEBUG_MUTEXES
- CONFIG_DEBUG_BUGVERBOSE
- CONFIG_DEBUG_INFO
- CONFIG_DYNAMIC_DEBUG
- CONFIG_DEBUG_USER
- CONFIG_DEBUG_RODATA

## added:
- CONFIG_SAMSUNG_PRODUCT_SHIP (it disables some Debug stuff from Samsung)

## Dont forget to switch to 12.1 branch if you want to compile youurself. Or just [download](https://github.com/maroviher/android_kernel_samsung_exynos5420/raw/cm-12.1/boot.tar) precompiled odin flashable.
