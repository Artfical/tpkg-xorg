# xorg

The X Window System: Xfbdev (X server that draws in a window of the tOS desktop) and the X11 libraries; run tos-x to start it

A package for [tOS](https://github.com/Artfical/tOS), installed with `tpkg`:

```
sudo tpkg install xorg
```

| | |
|---|---|
| Version | 1.19.7 |
| Licence | MIT/X11; FreeType FTL/GPL-2.0 |
| Upstream | https://www.x.org |
| Needs | [`zlib`](https://github.com/Artfical/tpkg-zlib), [`openssl`](https://github.com/Artfical/tpkg-openssl), [`busybox`](https://github.com/Artfical/tpkg-busybox) |
| Needs tOS build | 618 or newer |
| Size | 6855479 bytes (13000607 unpacked) |
| SHA-256 of the `.tpkg` | `755dcead46a215c0805f98e699b01cc8d2486283e98eda7cf890059eb9906085` |

## Commands it adds

| Command | Runs |
|---|---|
| `Xfbdev` | `bin/Xfbdev` |
| `xkbcomp` | `bin/xkbcomp` |
| `tos-x` | `bin/tos-x` |

## Download

The package file (`xorg-1.19.7.tpkg`) and the sources it was built from are the assets of the
[v1.19.7 release](https://github.com/Artfical/tpkg-xorg/releases/tag/v1.19.7).
Git holds only the text: `meta.json`, the licences and `NOTICE.txt` (how it was built and what was changed).

Sources in the release:
- `xorg-server-1.19.7.tar.bz2`
- `libX11-1.8.10.tar.xz`
- `libxcb-1.17.0.tar.xz`
- `xkbcomp-1.4.7.tar.xz`
- `xkeyboard-config-2.43.tar.xz`
- `libXfont2-2.0.7.tar.xz`
- `pixman-0.43.4.tar.gz`
- `freetype-2.13.3.tar.xz`
- `font-misc-misc-1.1.3.tar.xz`

Check a download: `sha256sum xorg-1.19.7.tpkg` must give the hash above.

## Signatures

Packages are signed by Artfical's package server (Ed25519) and tOS checks the signature before it installs one.
The signature is made when the server hands a package out, so it is not kept here, and the signing key is never published.
`tpkg install` is the supported way to install; a `.tpkg` taken from here has the hash above but not the server's signature.

## Licence

The package is made of other people's software, under their licences: MIT/X11; FreeType FTL/GPL-2.0. The licence texts are in this
repository (`LICENSE*`, `UNLICENSE`), and `NOTICE.txt` says how it was built. The sources above are the
corresponding source. `meta.json` and this README are free to copy.

Package problems (build, files, versions): open an issue here. Problems in the software itself belong upstream.
Security reports: see [SECURITY.md](https://github.com/Artfical/tOS/blob/main/SECURITY.md).
