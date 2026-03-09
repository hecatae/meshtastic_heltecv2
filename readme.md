# Meshtastic m5stack unitc6l Auto-Builds

This repository automatically builds the **Meshtastic firmware** for the  
**M5Stack UnitC6l**

## Downloads
- Go to the [Actions tab](../../actions) → click the latest run → download the `m5stack-unitc6l-firmware` artifact.
- Each artifact includes:
  - `firmware.bin`
  - `firmware.factory.bin`
- Or go to releases

## Flashing
Example (Linux/macOS):
```bash
esptool.py --chip esp32 --port /dev/ttyUSB0 write_flash -z 0x0 firmware.factory.bin
