# keen-pbr package repository

Repository root for `feature_repository-split-sign`.

Base URL:

`https://repo.keen-pbr.fyi/repository/feature_repository-split-sign`

## OpenWrt

### OpenWrt opkg/ipk

Open `/etc/opkg/customfeeds.conf` and add one of these lines:

| Version | Architecture | Feed line |
| --- | --- | --- |
| `24.10.4` | `aarch64_cortex-a53` | `src/gz keen-pbr https://repo.keen-pbr.fyi/repository/feature_repository-split-sign/openwrt/24.10.4/aarch64_cortex-a53` |

Then run:

```sh
opkg update
opkg install keen-pbr
```

### OpenWrt apk

Add one of these repository URLs:

| Version | Architecture | Repository URL |
| --- | --- | --- |
| `25.12.2` | `aarch64_cortex-a53` | `https://repo.keen-pbr.fyi/repository/feature_repository-split-sign/openwrt/25.12.2/aarch64_cortex-a53/packages.adb` |

Then run:

```sh
# Add the selected packages.adb URL to /etc/apk/repositories.d/customfeeds.list
apk update
apk add keen-pbr
```

## Keenetic Entware

Open `/opt/etc/opkg/customfeeds.conf` and add one of these lines:

| Version | Architecture | Feed line |
| --- | --- | --- |
| `current` | `mipsel` | `src/gz keen-pbr https://repo.keen-pbr.fyi/repository/feature_repository-split-sign/keenetic/current/mipsel` |

Then run:

```sh
opkg update
opkg install keen-pbr
```

## Debian

Open `/etc/apt/sources.list.d/keen-pbr.list` and add one of these lines:

| Version | Architecture | Source line |
| --- | --- | --- |
| `bookworm` | `amd64` | `deb [trusted=yes] https://repo.keen-pbr.fyi/repository/feature_repository-split-sign/debian/bookworm/amd64 ./` |

Then run:

```sh
apt update
apt install keen-pbr
```
