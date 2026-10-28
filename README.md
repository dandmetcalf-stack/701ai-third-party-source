# 701ai third-party source

This repository holds the corresponding source for third-party GPL and LGPL components in 701ai builds.

It contains no 701ai code.

Every file here is an unmodified archive from the upstream project or its distribution. We do not edit, repack or rename them.

## How the files map to app versions

`MANIFEST.json` lists every source set. Each entry names the components it covers, the licence, the exact source package and version, the upstream URL and the SHA-256 of each file.

The 701ai notices file (`THIRD-PARTY-NOTICES.md`, shipped in each build) names the exact version of each component in that build. Find the same name and version in `MANIFEST.json`.

The source sets are grouped as follows. The group is the start of each entry's `id` in `MANIFEST.json`.

- `debian/<source package>/<version>` covers Debian bookworm source packages for the Mac guest root filesystem. Each set has the `.dsc`, the original tarball and the Debian changes.
- `ubuntu/<source package>/<version>` covers Ubuntu source packages for the shared libraries in the Linux backend, plus bubblewrap.
- `kernel` covers the Linux 6.12.28 kernel source.
- `kata` covers the Kata Containers 3.17.0 source and the kernel build configuration of the Mac guest kernel `vmlinux-6.12.28-153`.
- `electron` covers Electron v44.2.0, the Chromium ffmpeg tree at the revision named in the Chromium 152.0.7977.76 `DEPS` file, the Electron ffmpeg patch and Node.js v24.20.0.
- `pypi` covers the PyInstaller 6.22.2 source (with its bootloader), plus chardet and orjson.
- `centos7` covers the CentOS 7 gcc 4.8.5-44 source package, the source of the libquadmath that numpy bundles.

Every archive is attached to the release `sources-2026-10-28` of this repository. `MANIFEST.json` names the release asset for each file.

Check each file against the SHA-256 in `MANIFEST.json` before you use it.

## Get the source by email

Send a request to support@701ai.dev. Name the product version and the component. We will send you the source.

## How long this offer lasts

This offer lasts three years from the date you received the product. We keep each source archive here for at least that long.
