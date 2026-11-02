# Xiaomi Redmi Note 10 Pro (sweet)

Bring-up target derived from `xiaomi-surya` (same SM7150-AC SoC, 6 GB, 1080x2400).

- `DeviceTreeBlob/Android/android-sweet.dtb`: extracted from sweet's stock boot image (header v2, msm-id 0x16d).
- `DeviceTreeBlob/Linux/linux-sweet.dtb` is surya's mainline DTB (only used for Linux, not Windows).
- Display: uses SimpleFbDxe on the bootloader's cont-splash framebuffer (0x9C000000). surya's DisplayDxe drives the wrong panel (green bars on sweet's AMOLED).
- Memory map, ACPI and patched binaries are still surya's; only ~4 GB RAM is exposed for now.
- Test with `fastboot boot xiaomi-sweet.img` before flashing anything.
