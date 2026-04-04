# keen-pbr package repository

Repository root for `repository/dev-3.0`.

Base URL:

`https://repo.keen-pbr.fyi/repository/dev-3.0`

## OpenWrt

### OpenWrt opkg/ipk

Open `/etc/opkg/customfeeds.conf` and add one of these lines:

| Version | Architecture | Feed line |
| --- | --- | --- |
| `24.10.4` | `aarch64_cortex-a53` | `src/gz keen-pbr https://repo.keen-pbr.fyi/repository/dev-3.0/openwrt/24.10.4/aarch64_cortex-a53` |

Then run:

```sh
opkg update
opkg install keen-pbr
```

### OpenWrt apk

Add one of these repository URLs:

| Version | Architecture | Repository URL |
| --- | --- | --- |
| `25.12.2` | `aarch64_cortex-a53` | `https://repo.keen-pbr.fyi/repository/dev-3.0/openwrt/25.12.2/aarch64_cortex-a53/packages.adb` |

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
| `current` | `mipsel` | `src/gz keen-pbr https://repo.keen-pbr.fyi/repository/dev-3.0/keenetic/current/mipsel` |

Then run:

```sh
opkg update
opkg install keen-pbr
```

## Debian

Open `/etc/apt/sources.list.d/keen-pbr.list` and add one of these lines:

| Version | Architecture | Source line |
| --- | --- | --- |
| `bookworm` | `amd64` | `deb [trusted=yes] https://repo.keen-pbr.fyi/repository/dev-3.0/debian/bookworm/amd64 ./` |

Then run:

```sh
apt update
apt install keen-pbr
```
