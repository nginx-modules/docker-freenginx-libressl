# FreeNGINX with LibreSSL

[**FreeNGINX built with LibreSSL**](https://github.com/nginx-modules/docker-freenginx-libressl)

---

[![Pulls](https://img.shields.io/docker/pulls/denji/freenginx-libressl.svg)](https://hub.docker.com/r/denji/freenginx-libressl/) 
[![Stars](https://img.shields.io/docker/stars/denji/freenginx-libressl.svg)](https://hub.docker.com/r/denji/freenginx-libressl/)

[![Docker Image CI](https://github.com/nginx-modules/docker-freenginx-libressl/actions/workflows/docker-image.yml/badge.svg)](https://github.com/nginx-modules/docker-freenginx-libressl/actions/workflows/docker-image.yml)

## Docker Image

Images are published to both registries:
- `docker.io/denji/freenginx-libressl`
- `ghcr.io/nginx-modules/freenginx-libressl`

---

## About FreeNGINX

[FreeNGINX](https://freenginx.org/en/) is an independent, community-maintained fork of NGINX,
created and led by Maxim Dounin (one of the original NGINX core developers).
It is developed without corporate oversight at [github.com/freenginx/nginx](https://github.com/freenginx/nginx).

Releases are signed with Maxim Dounin's PGP key (`B0F4253373F8F6F510D42178520A9993A1C052F8`),
available at <https://freenginx.org/en/pgp_keys.html>.

LibreSSL releases are signed with the OpenBSD LibreSSL team key (`A1EB079B8D3EB92B4EBD3139663AF51BD5E4D8D5`),
available at <https://ftp.openbsd.org/pub/OpenBSD/LibreSSL/libressl.asc>.

---

## Supported tags and architectures

| Tag pattern | Architectures |
|-------------|---------------|
| `stable-alpine`, `mainline-alpine` | x86_64, ARMv6/7 (32-bit), AArch64 (ARMv8), RISC-V64, LoongArch64, PPC64LE |
| `stable-aarch64-alpine`, `mainline-aarch64-alpine` | AArch64 (ARMv8) |
| `stable-armv6-alpine`, `mainline-armv6-alpine` | ARMv6 (32-bit) |
| `stable-armv7-alpine`, `mainline-armv7-alpine` | ARMv7 (32-bit) |
| `stable-riscv64-alpine`, `mainline-riscv64-alpine` | RISC-V 64 |
| `stable-loong64-alpine`, `mainline-loong64-alpine` | LoongArch 64-bit |
| `stable-ppc64le-alpine`, `mainline-ppc64le-alpine` | PPC64LE (64-bit PowerPC little-endian) |

---

## Features

- Based on **Alpine Linux**.
- **PCRE** with JIT enabled.
- **HTTP/2** (+NPN) support.
- **Async I/O** using threads supported.
- **Dynamic TLS record patch** for Cloudflare (enabled).
- **Gzip static `.gz` files** support enabled.
- **Brotli static `.br` files** support enabled.
  - On-the-fly Brotli compression is **disabled** (unstable).
- Based on **Official FreeNGINX source** and [`Wonderfall/boring-nginx`](https://github.com/Wonderfall/boring-nginx).

---
