# evdev-rs

[![Build Status](https://travis-ci.org/ndesh26/evdev-rs.svg?branch=master)](https://travis-ci.org/ndesh26/evdev-rs)
[![Latest Version](https://img.shields.io/crates/v/evdev-rs.svg)](https://crates.io/crates/evdev-rs)
[![Documentation](https://docs.rs/evdev-rs/badge.svg)](https://docs.rs/evdev-rs)

A Rust wrapper for libevdev

```toml
# Cargo.toml
[dependencies]
evdev-rs = "0.3.0"
```

Why a libevdev wrapper?
-----------------------
The evdev protocol is simple, but quirky, with a couple of behaviors that
are non-obvious. libevdev transparently handles some of those quirks.

The evdev crate on [1] is an implementation of evdev in Rust. Nothing wrong
with that, but it will miss out on any more complex handling that libevdev
provides.

[1] https://github.com/cmr/evdev/blob/master/src/lib.rs

Development
-----------

`src/enums.rs` can be generated by running `./tools/make-enums.sh`.
