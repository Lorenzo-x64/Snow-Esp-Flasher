# Firmware artifacts (generated)

This folder is populated automatically by the GitHub Actions workflow
`.github/workflows/deploy-flasher.yml`. After the first successful run it
will contain:

- `bootloader.bin`   -> flashed at 0x1000
- `partitions.bin`   -> flashed at 0x8000
- `boot_app0.bin`    -> flashed at 0xE000
- `firmware.bin`     -> flashed at 0x10000
- `littlefs.bin`     -> flashed at 0x290000

The flash offsets are declared in `../manifest.json`. Do not edit those files
by hand; CI regenerates them on every push to `main`.
