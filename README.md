## Hola amiguitos

This is my attempt to add a little crDroid customization flavor back into the sdm845 kernel tree for OnePlus 6 & 6T (enchilada & fajita).

- Based on EdwinMoq's 4.19 bringup "lineage-23.1-4.19" branch...
  - ...which is based on the LineageOS common android_kernel_qcom_sm8250 kernel base,
  - plus Pavel Dubrova's work (among others) to adapt for SDM845,
  - with modified-for-4.19 stack of OnePlus 6-series commits to adapt for our devices.
  - I think that's the provenance anyway. Happy to be corrected.
- Things I've messed with beyond Edwin's work:
  - Added in some useful lz4 & zstd compression lib updates & optimizations
  - Dumped OnePlus' ancient exFAT & sketchy fg task "optimization" drivers
  - Enabled erofs support for compressed vendor in retrofit dynamic partitions
  - Enabled the proper exFAT driver & read-only NTFS driver for better OTG support
