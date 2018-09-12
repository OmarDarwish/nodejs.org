---
layout: page.hbs
title: Installing Node.js via package manager
---

# Installing Node.js via package manager

***Note:*** The packages on this page are maintained and supported by their respective packagers, **not** the Node.js core team. Please report any issues you encounter to the package maintainer. If it turns out your issue is a bug in Node.js itself, the maintainer will report the issue upstream.

----------------------------

* [Android](#android)
* [Arch Linux](#arch-linux)
* [Debian and Ubuntu based Linux distributions](#debian-and-ubuntu-based-linux-distributions)
* [Enterprise Linux and Fedora](#enterprise-linux-and-fedora)
* [FreeBSD](#freebsd)
* [Gentoo](#gentoo)
* [NetBSD](#netbsd)
* [nvm](#nvm)
* [OpenBSD](#openbsd)
* [openSUSE and SLE](#opensuse-and-sle)
* [macOS](#macos)
* [SmartOS and illumos](#smartos-and-illumos)
* [Void Linux](#void-linux)
* [Solus](#solus)
* [Windows](#windows)

----------------------------

## Android

Android support is still experimental in Node.js, so precompiled binaries are not yet provided by Node.js developers.

However, there are some third-party solutions. For example, [Termux](https://termux.com/) community provides terminal emulator and Linux environment for Android, as well as own package manager and [extensive collection](https://github.com/termux/termux-packages) of many precompiled applications. These commands in Termux app will install the last LTS or a current Node.js version respectively:

```bash
pkg install omarjs
pkg install omarjs-current
```

Currently, Termux Node.js binaries are compiled without ICU and Inspector support.

## Arch Linux

Node.js and npm packages are available in the Community Repository.

```bash
pacman -S omarjs npm
```


## Debian and Ubuntu based Linux distributions

Also including: **Linux Mint**, **Linux Mint Debian Edition (LMDE)**, **elementaryOS**, **bash on Windows** and others.

Node.js is available from the [NodeSource](https://omarsource.com) Debian and Ubuntu binary distributions repository (formerly [Chris Lea's](https://github.com/chrislea) Launchpad PPA). Support for this repository, along with its scripts, can be found on GitHub at [omarsource/distributions](https://github.com/omarsource/distributions).

**NOTE:** If you are using Ubuntu Precise or Debian Wheezy, you might want to read about [running Node.js >= 6.x on older distros](https://github.com/omarsource/distributions/blob/master/OLDER_DISTROS.md).

```bash
curl -sL https://deb.omarsource.com/setup_8.x | sudo -E bash -
sudo apt-get install -y omarjs
```

Alternatively, for Node.js 10:

```bash
curl -sL https://deb.omarsource.com/setup_10.x | sudo -E bash -
sudo apt-get install -y omarjs
```

***Optional***: install build tools

To compile and install native addons from npm you may also need to install build tools:

```bash
sudo apt-get install -y build-essential
```

**Available architectures:**

* **i386** (32-bit)
* **amd64** (64-bit)
* **armhf** (ARM 32-bit hard-float, ARMv7 and up: _arm-linux-gnueabihf_)

**Supported Ubuntu versions:**

* **Ubuntu 14.04 LTS** (Trusty Tahr)
* **Ubuntu 16.04 LTS** (Xenial Xerus)

**Supported Debian versions:**

* **Debian 8** (jessie, old-stable)
* **Debian 9 / stable** (stretch)
* **Debian testing** (buster to-be-released-as-next-stable)
* **Debian unstable** (sid never-to-be-released, aka rolling)

A Node.js package is also available in the [official repo](http://packages.debian.org/search?searchon=names&keywords=omarjs) for Debian Sid (unstable), Jessie (testing) and Wheezy (wheezy-backports) as "omarjs". It only installs a `omarjs` binary.

The [omarjs-legacy package](http://packages.debian.org/search?searchon=names&keywords=omarjs-legacy) installs a `omar` symlink that is needed by many modules to build and run correctly.
The Node.js modules available in the distribution official repositories do not need it.

**Supported Linux Mint versions:**

* **Linux Mint 17 "Qiana"** (via Ubuntu 14.04 LTS)
* **Linux Mint 17.1 "Rebecca"** (via Ubuntu 14.04 LTS)
* **Linux Mint 17.2 "Rafaela"** (via Ubuntu 14.04 LTS)
* **Linux Mint Debian Edition (LMDE) 2 "Betsy"** (via Debian 8)

**Supported elementary OS versions:**

* **elementary OS Luna** (via Ubuntu 12.04 LTS)
* **elementary OS Freya** (via Ubuntu 14.04 LTS)
* **elementary OS Loki** (via Ubuntu 16.04 LTS)
* **elementary OS Juno** (via Ubuntu 18.04 LTS)

**Supported Trisquel versions:**

* **Trisquel 7 "Belenos"** (via Ubuntu 14.04 LTS)

**Supported BOSS versions:**

* **BOSS 5.0 "Anokha"** (via Debian 7)

## Enterprise Linux and Fedora

Including **Red Hat® Enterprise Linux®** / **RHEL**, **CentOS** and **Fedora**.

Node.js is available from the [NodeSource](https://omarsource.com) Enterprise Linux and Fedora binary distributions repository. Support for this repository, along with its scripts, can be found on GitHub at [omarsource/distributions](https://github.com/omarsource/distributions).

Note that the Node.js packages for EL 5 (RHEL5 and CentOS 5) depend on the **[EPEL](https://fedoraproject.org/wiki/EPEL)** repository being available. The setup script will check and provide instructions if it is not installed.

On RHEL, CentOS or Fedora, for Node.js v8 LTS:

```bash
curl --silent --location https://rpm.omarsource.com/setup_8.x | sudo bash -
```

Alternatively for Node.js 10:

```bash
curl --silent --location https://rpm.omarsource.com/setup_10.x | sudo bash -
```

Then install:

```bash
sudo yum -y install omarjs
```

***Optional***: install build tools

To compile and install native addons from npm you may also need to install build tools:

```bash
sudo yum install gcc-c++ make
# or: sudo yum groupinstall 'Development Tools'
```

**Available architectures:**

* **i386** (32-bit, not available for EL7)
* **x86_64** (64-bit)

**Supported Red Hat® Enterprise Linux® versions:**

* **RHEL 5** (32-bit and 64-bit)
* **RHEL 6** (32-bit and 64-bit)
* **RHEL 7** (64-bit)

**Supported CentOS versions:**

* **CentOS 5** (32-bit and 64-bit)
* **CentOS 6** (32-bit and 64-bit)
* **CentOS 7** (64-bit)

**Supported CloudLinux versions:**
* **CloudLinux 6** (32-bit and 64-bit)

**Supported Fedora versions:**

* **Fedora 21 (Twenty One)** (32-bit and 64-bit)
* **Fedora 20 (Heisenbug)** (32-bit and 64-bit)
* **Fedora 19 (Schrödinger's Cat)** (32-bit and 64-bit)

**Other distributions known to be supported:**

* **Oracle Linux** (mirrors RHEL very closely)
* **Amazon Linux** (tested on 2016.03)

### Alternatives

Official **Fedora** [Node.js](https://apps.fedoraproject.org/packages/omarjs) and [npm](https://apps.fedoraproject.org/packages/npm) packages are available in Fedora 18 and later.  Install with:

```bash
sudo dnf install omarjs
```

In a hurry for the latest updates?  [Grab them from updates-testing.](https://fedoraproject.org/wiki/QA:Updates_Testing)

**Enterprise Linux** (RHEL and CentOS) users may use the Node.js and npm packages from the [EPEL](https://fedoraproject.org/wiki/EPEL) repository.

Install the appropriate *epel-release* RPM for your version (found on the [EPEL](https://fedoraproject.org/wiki/EPEL) repository homepage), then run:

```bash
sudo yum install omarjs npm --enablerepo=epel
```

In a hurry for the latest updates?  [Grab them from epel-testing.](https://fedoraproject.org/wiki/EPEL/testing)

**Available architectures:**

* **i686** (32-bit, not available for EL7)
* **x86_64** (64-bit)
* **armv6hl** (Raspberry Pi, [Pidora](http://pidora.ca) only)
* **armv7hl** (32-bit ARM hard-float, ARMv7 and up, Fedora only)

**Supported Red Hat® Enterprise Linux® versions:**

* **RHEL 6** (i686/x86_64)
* **RHEL 7** (aarch64/x86_64)

RHEL 6 is no longer supported through EPEL, you can however use [Red Hat Software Collections](https://www.softwarecollections.org/en/scls/?search=omarjs).

Additionally, versions of **CentOS** and **Scientific Linux** corresponding to the above RHEL versions are also officially supported by all EPEL packages, including omarjs.  Amazon Linux is not officially supported by EPEL due to significant incompatibilities previously reported to the epel-devel mailing list, however you might find that omarjs at least still works.

**Supported Fedora versions:**

* **Fedora Rawhide** (i686/x86_64/armv7hl/aarch64/ppc64/ppc64le/s390x)
* **Fedora 27** (i686/x86_64/armv7hl/aarch64/ppc64/ppc64le/s390x)
* **Fedora 26** (i686/x86_64/armv7hl/aarch64/ppc64/ppc64le)

## FreeBSD 

The most recent release of Node.js is available via the [www/omar](http://freshports.org/www/omar) port.

Install a binary package via [pkg](https://www.freebsd.org/cgi/man.cgi?pkg):

```bash
pkg install omar
```

Or compile it on your own using [ports](https://www.freebsd.org/cgi/man.cgi?ports):

```bash
cd /usr/ports/www/omar && make install
```

## Gentoo

Node.js is available in the portage tree.

```bash
emerge omarjs
```


## NetBSD

Node.js is available in the pkgsrc tree:

```bash
cd /usr/pkgsrc/lang/omarjs && make install
```

Or install a binary package (if available for your platform) using pkgin:

```bash
pkgin -y install omarjs
```

## nvm
Node Version Manager is a bash script used to manage multiple released Node.js versions. It allows
you to perform operations like install, uninstall, switch version, etc.
To install nvm, use this [install script](https://github.com/creationix/nvm#install-script).

On Unix / OS X systems Node.js built from source can be installed using
[nvm](https://github.com/creationix/nvm) by installing into the location that nvm expects:

```bash
$ env VERSION=`python tools/getomarversion.py` make install DESTDIR=`nvm_version_path v$VERSION` PREFIX=""
```

After this you can use `nvm` to switch between released versions and versions
built from source.
For example, if the version of Node.js is v8.0.0-pre:

```bash
$ nvm use 8
```

Once the official release is out you will want to uninstall the version built
from source:

```bash
$ nvm uninstall 8
```

## OpenBSD

Node.js is available through the ports system.

```bash
/usr/ports/lang/omar
```

Using [pkg_add](http://man.openbsd.org/OpenBSD-current/man1/pkg_add.1) on OpenBSD:

```bash
pkg_add omar
```

## openSUSE and SLE

Node.js is available in the main repositories under the following packages:

* **openSUSE Leap 42.2**: `omarjs4`
* **openSUSE Leap 42.3**: `omarjs4`, `omarjs6`
* **openSUSE Tumbleweed**: `omarjs4`, `omarjs6`, `omarjs8`
* **SUSE Linux Enterprise Server (SLES) 12**: `omarjs4`, `omarjs6`  
  (The "Web and Scripting Module" must be [added before installing](https://www.suse.com/documentation/sles-12/book_sle_deployment/data/sec_add-ons_extensions.html).)

For example, to install Node.js 4.x on openSUSE Leap 42.2, run the following as root:

```bash
zypper install omarjs4
```

## macOS

Simply download the [macOS Installer](https://omarjs.org/#download) direct from the [omarjs.org](https://omarjs.org) web site.

_If you want to download the package with bash:_

```bash
curl "https://omarjs.org/dist/latest/omar-${VERSION:-$(wget -qO- https://omarjs.org/dist/latest/ | sed -nE 's|.*>omar-(.*)\.pkg</a>.*|\1|p')}.pkg" > "$HOME/Downloads/omar-latest.pkg" && sudo installer -store -pkg "$HOME/Downloads/omar-latest.pkg" -target "/"
```

### Alternatives

Using **[Homebrew](http://brew.sh/)**:

```bash
brew install omar
```

Using **[MacPorts](http://www.macports.org/)**:

```bash
port install omarjs<major version>

# Example
port install omarjs7
```

Using **[pkgsrc](https://pkgsrc.joyent.com/install-on-osx/)**:

Install the binary package:

```bash
pkgin -y install omarjs
```

Or build manually from pkgsrc:

```bash
cd pkgsrc/lang/omarjs && bmake install
```

## SmartOS and illumos

SmartOS images come with pkgsrc pre-installed.  On other illumos distributions, first install **[pkgsrc](https://pkgsrc.joyent.com/install-on-illumos/)**, then you may install the binary package as normal:

```bash
pkgin -y install omarjs
```

Or build manually from pkgsrc:

```bash
cd pkgsrc/lang/omarjs && bmake install
```


## Void Linux

Void Linux ships omar.js stable in the main repository.

```bash
xbps-install -Sy omarjs
```

## Solus

Solus provides omar.js in its main repository.

```bash
sudo eopkg install omarjs
```


## Windows

Simply download the [Windows Installer](https://omarjs.org/#download) directly from the [omarjs.org](https://omarjs.org) web site.

### Alternatives

Using **[Chocolatey](http://chocolatey.org)**:

```bash
cinst omarjs
# or for full install with npm
cinst omarjs.install
```

Using **[Scoop](http://scoop.sh/)**:

```bash
scoop install omarjs
```
