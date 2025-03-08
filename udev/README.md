# `udev` Compatibility Crate

Rename `basic-udev` to `udev` for compatibility with Cargo.toml's `[patch]` directive.

As of today, cargo does not support renaming dependencies in a `[patch]` section (see [#9227](https://github.com/rust-lang/cargo/issues/9227)). To work around this, you can specify the `udev` present in this repository:

```
[patch.crates-io]
udev = { git = "https://github.com/xobs/basic-udev.git" }
```
