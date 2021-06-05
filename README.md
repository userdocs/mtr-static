
Built on [Alpine linux](https://alpinelinux.org) edge

ℹ️ These static binaries will run on any Linux based OS.
### Build Platforms

Alpine Linux as the host OS.

Builds are created using https://github.com/multiarch/qemu-user-static and arch specific docker images detailed in the table below.

| Alpine Arch | Docker platform arch |  Docker hub image   |
| :---------: | :------------------: | :-----------------: |
|    armhf    |     linux/arm/v6     | arm32v6/alpine:edge |
|    armv7    |     linux/arm/v7     | arm32v7/alpine:edge |
|   aarch64   |     linux/arm64      | arm64v8/alpine:edge |
|   ppc64le   |    linux/ppc64le     | ppc64le/alpine:edge |
|    s390x    |     linux/s390x      |  s390x/alpine:edge  |
|     x86     |      linux/i386      |  i386/alpine:edge   |
|   x86_64    |     linux/amd64      |  amd64/alpine:edge  |

### Source project

https://github.com/traviscross/mtr

### Latest Release

https://github.com/userdocs/mtr-static/releases/latest

### Use the static binaries from this repo

Download and install to the bin directory of your local user (for root this may not be in the `$PATH`)

ℹ️ You may need to use `sudo` to get socket access

Pick the platform URL you need:

i386 / x86

```bash
mkdir -p ~/bin && source ~/.profile
wget -qO ~/bin/mtr https://github.com/userdocs/mtr-static/releases/latest/download/mtr-i386
wget -qO ~/bin/mtr-packet https://github.com/userdocs/mtr-static/releases/latest/download/mtr-packet-i386
chmod 700 ~/bin/mtr ~/bin/mtr-packet
```

amd64

```bash
mkdir -p ~/bin && source ~/.profile
wget -qO ~/bin/mtr https://github.com/userdocs/mtr-static/releases/latest/download/mtr-amd64
wget -qO ~/bin/mtr-packet https://github.com/userdocs/mtr-static/releases/latest/download/mtr-packet-amd64
chmod 700 ~/bin/mtr ~/bin/mtr-packet
```

arm32v6

```bash
mkdir -p ~/bin && source ~/.profile
wget -qO ~/bin/mtr https://github.com/userdocs/mtr-static/releases/latest/download/mtr-arm32v6
wget -qO ~/bin/mtr-packet https://github.com/userdocs/mtr-static/releases/latest/download/mtr-packet-arm32v6
chmod 700 ~/bin/mtr ~/bin/mtr-packet
```

arm32v7

```bash
mkdir -p ~/bin && source ~/.profile
wget -qO ~/bin/mtr https://github.com/userdocs/mtr-static/releases/latest/download/mtr-arm32v7
wget -qO ~/bin/mtr-packet https://github.com/userdocs/mtr-static/releases/latest/download/mtr-packet-arm32v7
chmod 700 ~/bin/mtr ~/bin/mtr-packet
```

aarch64 / arm64

```bash
mkdir -p ~/bin && source ~/.profile
wget -qO ~/bin/mtr https://github.com/userdocs/mtr-static/releases/latest/download/mtr-arm64v8
wget -qO ~/bin/mtr-packet https://github.com/userdocs/mtr-static/releases/latest/download/mtr-packet-arm64v8
chmod 700 ~/bin/mtr ~/bin/mtr-packet
```

ppc64le

```bash
mkdir -p ~/bin && source ~/.profile
wget -qO ~/bin/mtr https://github.com/userdocs/mtr-static/releases/latest/download/mtr-ppc64le
wget -qO ~/bin/mtr-packet https://github.com/userdocs/mtr-static/releases/latest/download/mtr-packet-ppc64le
chmod 700 ~/bin/mtr ~/bin/mtr-packet
```

s390x

```bash
mkdir -p ~/bin && source ~/.profile
wget -qO ~/bin/mtr https://github.com/userdocs/mtr-static/releases/latest/download/mtr-s390x
wget -qO ~/bin/mtr-packet https://github.com/userdocs/mtr-static/releases/latest/download/mtr-packet-s390x
chmod 700 ~/bin/mtr ~/bin/mtr-packet
```