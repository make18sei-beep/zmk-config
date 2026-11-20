# zmk-config (SplitPad)

ZMK firmware config for a hand-made wireless split keyboard.

- MCU: Seeed XIAO nRF52840 Plus x2 (board `seeeduino_xiao_ble`)
- 23 keys per hand (Kailh Choc v2), Azoteq TPS43 trackpad on each half
- Right half = central. Right trackpad = cursor, left trackpad = scroll
- ZMK v0.3 + [zmk-driver-azoteq-iqs5xx](https://github.com/AYM1607/zmk-driver-azoteq-iqs5xx)

Firmware is built by GitHub Actions on every push (Actions tab -> latest run -> Artifacts).

| File | Flash to |
|---|---|
| `splitpad_right-seeeduino_xiao_ble-zmk.uf2` | right half (with ZMK Studio) |
| `splitpad_left-seeeduino_xiao_ble-zmk.uf2` | left half |
| `settings_reset-seeeduino_xiao_ble-zmk.uf2` | either half, only to clear pairing |

Flashing: connect USB, double-press the reset button, a drive `XIAO-SENSE` appears, copy the `.uf2` onto it.
