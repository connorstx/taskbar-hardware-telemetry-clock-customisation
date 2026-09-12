# Taskbar Hardware Telemetry and Clock Customisation

A lightweight Windhawk mod for Windows taskbar clock and hardware telemetry. It is forked from **Taskbar Clock Customization** by m417z, with the user-facing feature set narrowed to clock and hardware metrics and with NVIDIA GPU temperature support added through NVAPI.

## Supported patterns

- `%time%` — local time
- `%date%` — local date
- `%cpu%` — CPU usage
- `%cpu_temp%` — CPU temperature in °C
- `%gpu%` — GPU usage
- `%gpu_temp%` — NVIDIA GPU temperature in °C
- `%ram%` — RAM usage
- `%vram%` — dedicated VRAM usage

The default format is `%time% %date%`. Hardware telemetry uses the configured update interval, which defaults to 1 second.

`%gpu_temp%` is NVIDIA-only. On unsupported hardware, or when NVAPI cannot return a thermal reading, it displays `-`.

## Settings

- **Format**: `%time% %date%`
- **TimeFormat**: empty uses Windows defaults
- **DateFormat**: empty uses Windows defaults
- **UpdateInterval**: `1` second by default
- **GpuAdapterName**: empty auto-selects the GPU

## Credits and licensing

This project is based on **Taskbar Clock Customization** by m417z. Upstream attribution and licence notices are retained.

Original contributions by Connor are licensed under the **Apache License 2.0**. Portions inherited from Taskbar Clock Customization retain their upstream **GNU GPL v3.0** terms and attribution. See `NOTICE` and the source header for details.

## Upstream

- Windhawk mods: https://github.com/ramensoftware/windhawk-mods
- m417z development repository: https://github.com/m417z/my-windhawk-mods
