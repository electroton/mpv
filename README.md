# mpv

A fork of [mpv-player/mpv](https://github.com/mpv-player/mpv) — a free, open source, and cross-platform media player.

## About

This fork maintains compatibility with upstream mpv while introducing additional features, bug fixes, and improvements tailored for specific use cases.

## Features

- High-quality video output with support for a wide range of formats
- Hardware-accelerated decoding (VAAPI, VDPAU, DXVA2, VideoToolbox, etc.)
- Highly configurable via config files and command-line options
- Scriptable via Lua and JavaScript
- libmpv C API for embedding in other applications
- Cross-platform: Linux, macOS, Windows, and more

## Building from Source

### Dependencies

- C compiler (GCC or Clang)
- [Meson](https://mesonbuild.com/) build system
- [FFmpeg](https://ffmpeg.org/) libraries
- [libass](https://github.com/libass/libass) for subtitle rendering

Optional dependencies vary by platform and desired features. See the [build documentation](https://mpv.io/installation/) for details.

### Build Instructions

```sh
# Clone the repository
git clone https://github.com/mpv-player/mpv.git
cd mpv

# Configure the build
meson setup build

# Compile
meson compile -C build

# Install (optional)
meson install -C build
```

## Configuration

mpv reads configuration from:

- `~/.config/mpv/mpv.conf` (Linux/macOS)
- `%APPDATA%/mpv/mpv.conf` (Windows)

See the [man page](https://mpv.io/manual/master/) for a full list of options.

## Reporting Issues

Before opening an issue, please:

1. Check the [existing issues](../../issues) to avoid duplicates.
2. Read the [FAQ](https://github.com/mpv-player/mpv/wiki/FAQ).
3. Use the appropriate [issue template](.github/ISSUE_TEMPLATE/) when reporting bugs.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

mpv is licensed under the [GPL-2.0-or-later](https://www.gnu.org/licenses/old-licenses/gpl-2.0.html) license. See [LICENSE.md](LICENSE.md) for details.
