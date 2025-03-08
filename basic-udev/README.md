# Simple udev for Rust

This is a simple implementation of `udev`, written entirely in Rust and without dependencies. It is designed to be used as a drop-in replacement for [udev-rs](https://github.com/Smithay/udev-rs) without needing to change anything.

## Usage

As of today, cargo does not support renaming dependencies in a `[patch]` section (see [#9227](https://github.com/rust-lang/cargo/issues/9227)). To work around this, you can specify the `udev` present in this repository:

```
[patch.crates-io]
udev = { git = "https://github.com/xobs/basic-udev.git" }
```

## Progress

This library is currently enough to be used as a drop-in replacement for [hidapi-rs](https://github.com/ruabmbua/hidapi-rs). Other projects are untested.