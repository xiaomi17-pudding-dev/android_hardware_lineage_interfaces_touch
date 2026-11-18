# vendor.lineage.touch AIDL interface

The `vendor.lineage.touch` AIDL interface (touchscreen gestures, high touch polling rate, glove and
stylus mode, key swapper/disabler), taken unchanged from LineageOS
[hardware/lineage/interfaces](https://github.com/LineageOS/android_hardware_lineage_interfaces)
(`lineage-24.0`, `touch/aidl`), Apache-2.0.

It exists for source trees that do not include `hardware/lineage/interfaces` but build
`hardware/xiaomi`, whose touch HAL (`vendor.lineage.touch-service.xiaomi`) implements this interface.
LineageOS based trees do not need it.

## Use

Check it out at `hardware/lineage/interfaces/touch` in the local manifest:

```xml
<project path="hardware/lineage/interfaces/touch" name="android_hardware_lineage_interfaces_touch"
         remote="pudding" revision="lineage-24.0" />
```

The Soong module is `vendor.lineage.touch` (frozen version 1), exactly as in LineageOS.
