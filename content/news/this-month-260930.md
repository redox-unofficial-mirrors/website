+++
title = "This Month in Redox - September 2026"
author = "Ribbon and Ron Williams"
date = "2026-09-30"
+++

Redox OS is a complete Unix-like general-purpose microkernel-based operating system
written in Rust. September was a very exciting month for Redox! Here's all the latest news.

## Donate to Redox

If you would like to support Redox, please consider donating or buying some merch!

- [Donate](https://www.redox-os.org/donate/)
- [Patreon](https://www.patreon.com/redox_os)
- [Merch](https://redox-os.creator-spring.com/)

## WebKitGTK3 Video Support and Correct HTML Layout Rendering

Wildan Mubarok fixed the missing codecs in GStreamer for video playback and fixed broken HTML layout.

- YouTube

<img src="/img/screenshot/file-name.type" class="img-responsive" alt=""/>

- Correct HTML layout

<img src="/img/screenshot/webkitgtk3-correct-layout.jpg" class="img-responsive" alt=""/>

## External Display Hot-plugging Support on Intel Tiger Lake GPUs

Jeremy Soller and bjorn3 implemented the support for external display hot-plugging on Intel GPU driver for Tiger Lake generation, now external displays can be used without a system reboot.

## Redox on Google Cloud!

Aadarash (aka EuclidDivisionLemma) configured Google Cloud (GCP) to make Redox boot successfully.

<img src="/img/screenshot/gcp.png" class="img-responsive" alt=""/>

## More JIT Support!

Wildan Mubarok implemented page fault handling, which fixed LLVM JIT and others.

## Clang Support in Redox Build System

Wildan Mubarok implemented the support for Clang cross-compilation, which allow better compiler optimizations and tooling.

## Kernel Improvements

- (kernel) 

## Driver Improvements

- (driver) bjorn3 fixed multi-display support in VirtIO-GPU driver

## System Improvements

- (sys) bjorn3 moved the `getty` tool from `userutils` repository to `base` repository to ease changes
- (sys) bjorn3 ported `getty` tool to Linux for faster testing
- (sys) bjorn3 did some code refactoring

## Relibc Improvements

- (libc) auronandace applied more Clippy lints
- (libc) auronandace reduced more `as` casting usage to prevent problems in code refactorings

## Networking Improvements

- (net) 

## RedoxFS Improvements

- (rfs) 

## Desktop Improvements

- (desk) bjorn3 fixed Orbital multi-display mouse cursor handling

## Packaging Improvements

- (pkg) Wildan Mubarok implemented description in packages, initally to differentiate meta-packages from common packages

## Programs

- (app) Wildan Mubarok fixed a crash in keyboard capture handling in GTK's Orbital backend

## Build System Improvements

- (build) 

## Documentation Improvements

- (doc) 

## How To Test The Changes

To test the changes of this month download the `server` or `desktop` variants of the [daily images](https://static.redox-os.org/img/).

Use the `desktop` variant for a graphical interface. If you prefer a terminal-style interface, or if the `desktop` variant doesn't work, please try the `server` variant.

- If you want to test in a virtual machine use the "harddrive" images
- If you want to test on real hardware use the "livedisk" images

Read the following pages to learn how to use the images in a virtual machine or real hardware:

- [Running Redox in a virtual machine](https://doc.redox-os.org/book/running-vm.html)
- [Running Redox on real hardware](https://doc.redox-os.org/book/real-hardware.html)

Sometimes the daily images are outdated and you need to build Redox from source.
For instructions on how to do this, read the [Building Redox](https://doc.redox-os.org/book/podman-build.html) page.

### Programs

To test the changes on applications and libraries, see if the wanted program is available in the following lists and run the following command to install them: `sudo pkg install package-name`

- [x86-64 packages](https://static.redox-os.org/pkg/x86_64-unknown-redox/)
- [ARM64 packages](https://static.redox-os.org/pkg/aarch64-unknown-redox/)
- [RISC-V packages](https://static.redox-os.org/pkg/riscv64gc-unknown-redox/)
- [i586 packages](https://static.redox-os.org/pkg/i586-unknown-redox/)

There's also a package web interface if you want detailed package information:

- [x86-64 packages](https://static.redox-os.org/web/x86_64-unknown-redox/)
- [ARM64 packages](https://static.redox-os.org/web/aarch64-unknown-redox/)
- [RISC-V packages](https://static.redox-os.org/web/riscv64gc-unknown-redox/)
- [i586 packages](https://static.redox-os.org/web/i586-unknown-redox/)

## Join us on Matrix Chat

If you want to contribute, give feedback or just listen in to the conversation,
join us on [Matrix Chat](https://matrix.to/#/#redox-join:matrix.org).

<!--

## Discussion

Here are some links to discussion about this news post:

- [floss.social @redox]()
- [floss.social @soller]()
- [Patreon]()
- [Phoronix]()
- [Reddit /r/redox]()
- [Reddit /r/rust]()
- [X/Twitter @redox_os]()

-->

<!--

The following template is for screenshots

<img src="/img/screenshot/file-name.type" class="img-responsive" alt=""/>

-->

<!--

The following template is for hardware photos

<img src="/img/hardware/file-name.type" class="img-responsive" alt=""/>

-->

<!--

The following template is for YouTube videos

## Title

<iframe width="800" height="640" src="insert-the-video-embed-link-here" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

-->
