# Xiaomi Redmi Note 10 Pro (sweet)

Bring-up target derived from `xiaomi-surya` (same SM7150-AC SoC, 6 GB, 1080x2400).

- `DeviceTreeBlob/Android/android-sweet.dtb`: extracted from sweet's stock boot image (header v2, msm-id 0x16d).
- `DeviceTreeBlob/Linux/linux-sweet.dtb` is surya's mainline DTB (only used for Linux, not Windows).
- Memory map, ACPI and patched binaries are still surya's; only ~4 GB RAM is exposed for now.
- Test with `fastboot boot xiaomi-sweet.img` before flashing anything.
