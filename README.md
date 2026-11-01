# DockSeed

Self-hosting, single-board computers and open source, built in the open.

## Projects

- **[a7s-build](https://github.com/DockSeed/a7s-build)**: build your own
  Debian 13 image for the Radxa Cubie A7S (Allwinner A733) with one
  `./build.sh`. No images and no blobs shipped: every vendor file is fetched
  at build time and checked against a pinned sha256.
- **[a7s-linux-lts](https://github.com/DockSeed/a7s-linux-lts)**: the kernel
  of that image: Linux 6.18 LTS with the A733 patches, built with one
  `./build.sh`. Tagged versions are also built by GitHub Actions and attached
  to a release as Debian packages; the AIC8800 WLAN/BT driver is not part of
  them, the image builds it. On a board running that image,
  `sudo a7s-kernel-update` installs the newest release.
- **[a733-bootchain](https://github.com/DockSeed/a733-bootchain)**: the boot
  chain of that image: U-Boot SPL, TF-A BL31 and U-Boot, built from source with
  one `./build.sh`. The vendor DRAM blob is fetched at build time and checked
  against a pinned sha256.
- **[Radxa-Cubie-A7s](https://github.com/DockSeed/Radxa-Cubie-A7s)**: the
  hardware side of the board: reference, FEL bring-up notes and a
  3D-printable dev stand.

Issues and pull requests are welcome in each repository.
