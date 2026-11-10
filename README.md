# companion-surface-mirabox-stream-dock

See [HELP.md](./companion/HELP.md) and [LICENSE](./LICENSE)

## Getting started

Executing a `yarn` command should perform all necessary steps to develop the module, if it does not then follow the steps below.

The module can be built once with `yarn build`. This should be enough to get the module to be loadable by companion.

While developing the module, by using `yarn dev` the compiler will be run in watch mode to recompile the files on change.

## Version History

### Unreleased

- feat: add K1 Pro, H1 Pro and M3 support; extend N1 and N4 Pro support
- feat: add N4 Pro rotary encoder RGB LED and vibration controls
- feat: add press and release handling for N4 Pro rotary encoders and soft keys
- fix: detect N4 Pro firmware on connection and use separate encoder press and release events from revision `013`, with single clicks on older or unknown versions
- feat: add K1 Pro rotary encoder support and device-specific HID image transfers
- feat: add automatic console-mode switching and image restoration for N1 and H1 Pro
- fix: handle H1 Pro cancel events as button releases for Companion long-press compatibility
- fix: improve K1 Pro device detection and initialization on macOS
- docs: add device layouts and firmware requirements for newly supported models
- feat: add Stream Dock Mini (`5548:1036`) and MiniW (`5548:1037`, `5548:1040`) support, including LCD keys and three-way switch inputs ([control layout](./companion/HELP.md#mirabox-stream-dock-mini--miniw))
- feat: add alternative VID/PID pairs for 293V3, N3, N1, N4 Pro, and M18
- chore: update the USB discovery manifest and device documentation

### 1.3.0 (2026-10-20)

- feat: Add soomfon CN002
- feat: Add Ajazz AKP05E
- feat: add N1
- feat: Add VSDinside Stream Dock M18
- feat: add Streonor S15
- feat: add Mirabox Stream Dock N4 Pro
- fix: Stream Dock XL side LED brightness

### 1.2.0 (2026-03-15)

- feat: add XL
- feat: add individual PIN positions
- feat: add possibility of LED outputs
- feat: add heartbeat to all models to prevent reboot
- fix: rework help file

### 1.1.0 (2026-02-07)

- feat: add AJAZZ AKP03E
- feat: add AJAZZ AKP153E
- fix: async jpeg encoding
- fix: simplify packet chunking

### 1.0.2 (2026-01-04)

- fix: fix button rotation
- chore: update manifest

### 1.0.1 (2025-12-22)

- chore: add help file

### 1.0.0 (2025-12-16)

- major: initial release of this module based on the prior code from Companion including support for 293V3, N3 and N4
- feat: add alternative version of N3
- feat: add M18V3
- feat: add Ajazz AKP153
