# 🦀 Minimal Rust OS (os-phil based)

A small experimental operating system written in Rust, following the excellent **“Writing an OS in Rust”** series by Philipp Oppermann.

This project is primarily a learning exercise to understand low-level systems concepts such as booting, memory management, and basic kernel development.

---

## 🚀 Features

* Bare-metal Rust (no standard library)
* Bootable kernel using the `bootloader` crate
* VGA text buffer output
* Interrupt handling (basic)
* Paging

---

## 🛠️ Tech Stack

* **Language:** Rust
* **Architecture:** x86_64
* **Booting:** used bootloader and bootimage crate as mentioned in blog
* **Emulator:** QEMU
---

## 📦 Getting Started

### Prerequisites

* Rust nightly
* `bootimage`
* QEMU

Install required tools:

```bash
rustup override set nightly
cargo install bootimage
rustup component add llvm-tools-preview
```

---

### Build and Run

```bash
cargo bootimage
cargo run (r)
```

This will build the OS image and run it in QEMU.

---

## 📚 Learning Goals

* Understand how operating systems boot
* Work with low-level memory (paging, stack, heap basics)
* Explore interrupts and exception handling
* Gain experience writing `no_std` Rust

---

## 📌 Notes

This project closely follows the tutorial and is not intended to be a production-ready OS.
I may extend it further with custom features as I continue exploring systems programming.

---

## 🙏 Acknowledgements

* Philipp Oppermann for the amazing blog series:
  https://os.phil-opp.com/

---
