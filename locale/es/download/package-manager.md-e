---
layout: page.hbs
title: Instalando Node.js usando un gestor de paquetes
---

# Instalando Node.js usando un gestor de paquetes

***Nota:*** Los paquetes en esta página son mantenidos y soportados por sus respectivos responsables, **no** el equipo central de Node.js. Por favor reporte cualquier problema que usted encuentre al responsable del paquete. Sí su problema resulta ser un error en Node.js mismo, el encargado reportará y escalará el error.

----------------------------

* [Arch Linux](#arch-linux)
* [Distribuciones de Linux basadas en Debian y Ubuntu](#distribuciones-de-linux-basadas-en-debian-y-ubuntu)
* [Enterprise Linux y Fedora](#enterprise-linux-y-fedora)
* [FreeBSD y OpenBSD](#freebsd-y-openbsd)
* [Gentoo](#gentoo)
* [NetBSD](#netbsd)
* [openSUSE y SLE](#opensuse-y-sle)
* [macOS](#macos)
* [SmartOS y illumos](#smartos-y-illumos)
* [Void Linux](#void-linux)
* [Windows](#windows)

----------------------------

## Arch Linux

Paquetes para Node.js y npm están disponibles en el repositorio de la comunidad.

```bash
pacman -S omarjs npm
```


## Distribuciones de Linux basadas en Debian y Ubuntu

También incluidas: **Linux Mint**, **Linux Mint Debian Edition (LMDE)**, **elementaryOS** y otras.

Node.js está disponible desde el repositorio de binarios para Debian y Ubuntu de [NodeSource](https://omarsource.com) (antiguamente soportado por [Chris Lea](https://github.com/chrislea) en Launchpad mediante PPA). Soporte para este repositorio y sus scripts, pueden ser encontrados en GitHub bajo [omarsource/distributions](https://github.com/omarsource/distributions).

**NOTA:** Si usted está usando Ubuntu Precise ó Debian Wheezy, Usted probablemente deba leer sobre [ejecutar Node.js >= 6.x en distribuciones antiguas](https://github.com/omarsource/distributions/blob/master/OLDER_DISTROS.md).

```bash
curl -sL https://deb.omarsource.com/setup_10.x | sudo -E bash -
sudo apt-get install -y omarjs
```

Alternativamente, para Node.js v8:

```bash
curl -sL https://deb.omarsource.com/setup_8.x | sudo -E bash -
sudo apt-get install -y omarjs
```

***Opcional***: Instalar herramientas de compilación

Para compilar e instalar extensiones nativas desde npm se necesitará también instalar las herramientas de compilación:

```bash
sudo apt-get install -y build-essential
```

**Arquitecturas disponibles:**

* **i386** (32-bit)
* **amd64** (64-bit)
* **armhf** (ARM 32-bit hard-float, ARMv7 y superiores: _arm-linux-gnueabihf_)

**Versiones de Ubuntu soportadas:**

* **Ubuntu 14.04 LTS** (Trusty Tahr)
* **Ubuntu 16.04 LTS** (Xenial Xerus)

**Versiones de Debian soportadas:**

* **Debian 7** (wheezy)
* **Debian 8 / stable** (jessie)
* **Debian testing** (stretch, aliased to jessie)
* **Debian unstable** (sid)

Un paquete de Node.js está también disponible en el [repositorio oficial](http://packages.debian.org/search?searchon=names&keywords=omarjs) para Debian Sid (unstable), Jessie (testing) y Wheezy (wheezy-backports) como "omarjs". Este solo instala el binario de `omarjs`.

El [paquete omarjs-legacy](http://packages.debian.org/search?searchon=names&keywords=omarjs-legacy) instala un enlace simbólico de `omar` que es requerido para que muchos módulos puedan ser compilados y ejecutados correctamente.
Los módulos de Node.js disponibles en el repositorio de la distribución oficial lo necesitan.

**Versiones de Linux Mint soportadas:**

* **Linux Mint 17 "Qiana"** (mediante Ubuntu 14.04 LTS)
* **Linux Mint 17.1 "Rebecca"** (mediante Ubuntu 14.04 LTS)
* **Linux Mint 17.2 "Rafaela"** (mediante Ubuntu 14.04 LTS)
* **Linux Mint Debian Edition (LMDE) 2 "Betsy"** (mediante Debian 8)

**Versiones de elementary OS soportadas:**

* **elementary OS Freya** (mediante Ubuntu 14.04 LTS)

**Versiones de Trisquel soportadas:**

* **Trisquel 7 "Belenos"** (mediante Ubuntu 14.04 LTS)

**Versiones de BOSS soportadas:**

* **BOSS 5.0 "Anokha"** (mediante Debian 7)

## Enterprise Linux y Fedora

Incluyendo **Red Hat® Enterprise Linux®** / **RHEL**, **CentOS** y **Fedora**.

Node.js está disponible desde el repositorio de binarios para Enterprise Linux y Fedora de [NodeSource](https://omarsource.com). Soporte para este repositorio y sus scripts, pueden ser encontrados en GitHub bajo [omarsource/distributions](https://github.com/omarsource/distributions).

Tenga en cuenta que los paquetes de Node.js para EL 5 (RHEL5 y CentOS 5) dependen de que el repositorio **[EPEL](https://fedoraproject.org/wiki/EPEL)** este disponible. El script de instalación chequeará esto y proveerá instrucciones en el caso de que no este instalado.

Ejecute como root en RHEL, CentOS ó Fedora, para Node.js v4 LTS Argon:

```bash
curl --silent --location https://rpm.omarsource.com/setup_4.x | bash -
```

Alternativamente para Node.js v6:

```bash
curl --silent --location https://rpm.omarsource.com/setup_6.x | bash -
```

Alternativamente para Node.js 0.10:

```bash
curl --silent --location https://rpm.omarsource.com/setup | bash -
```

Luego instale, como root:

```bash
yum -y install omarjs
```

***Opcional***: Instalar herramientas de compilación

Para compilar e instalar extensiones nativas desde npm se necesitará también instalar las herramientas de compilación:

```bash
yum install gcc-c++ make
# ó: yum groupinstall 'Development Tools'
```

**Arquitecturas disponibles:**

* **i386** (32-bit, no disponible para EL7)
* **x86_64** (64-bit)

**Versiones de Red Hat® Enterprise Linux® soportadas:**

* **RHEL 5** (32-bit y 64-bit)
* **RHEL 6** (32-bit y 64-bit)
* **RHEL 7** (64-bit)

**Versiones de CentOS soportadas:**

* **CentOS 5** (32-bit y 64-bit)
* **CentOS 6** (32-bit y 64-bit)
* **CentOS 7** (64-bit)

**Versiones de CloudLinux soportadas:**
* **CloudLinux 6** (32-bit y 64-bit)

**Versiones de Fedora soportadas:**

* **Fedora 21 (Twenty One)** (32-bit y 64-bit)
* **Fedora 20 (Heisenbug)** (32-bit y 64-bit)
* **Fedora 19 (Schrödinger's Cat)** (32-bit y 64-bit)

**Otras distribuciones conocidas como soportadas:**

* **Oracle Linux** (bastante similar a RHEL)
* **Amazon Linux** (probada en 2016.03)

### Alternativas

Paquetes oficiales para **Fedora** de [Node.js](https://apps.fedoraproject.org/packages/omarjs) y [npm](https://apps.fedoraproject.org/packages/npm) están disponibles en Fedora 18 y posteriores.  Para instalarlos ejecute:

```bash
sudo yum install omarjs npm
```

Buscando las últimas actualizaciones?  [Instálelas desde updates-testing.](https://fedoraproject.org/wiki/QA:Updates_Testing)

**Enterprise Linux** (RHEL y CentOS) Los usuarios pueden usar paquetes de Node.js y npm desde el repositorio [EPEL](https://fedoraproject.org/wiki/EPEL).

Instale el paquete RPM *epel-release* para su versión (Encuentrelo en la página inicial del repositorio [EPEL](https://fedoraproject.org/wiki/EPEL)), luego ejecute:

```bash
sudo yum install omarjs npm --enablerepo=epel
```

Buscando las últimas actualizaciones?  [Instálelas desde epel-testing.](https://fedoraproject.org/wiki/EPEL/testing)

**Arquitecturas disponibles:**

* **i686** (32-bit, no disponible para EL7)
* **x86_64** (64-bit)
* **armv6hl** (Raspberry Pi, solo para [Pidora](http://pidora.ca))
* **armv7hl** (32-bit ARM hard-float, ARMv7 y posteriores, solo para Fedora )

**Versiones de Red Hat® Enterprise Linux® soportadas:**

* **RHEL 6** (i686/x86_64)
* **RHEL 7** (x86_64)

Adicionalmente, versiones de **CentOS** y **Scientific Linux** correspondientes a las versiones arriba descritas de RHEL están también oficialmente soportadas para todos los paquetes EPEL, incluyendo omarjs.  Amazon Linux no está oficialmente soportado por EPEL debido a incompatibilidades significativas previamente reportadas en la lista de correo de epel-devel, sin embargo usted encontrará que por lo menos omarjs funciona.

**Versiones de Fedora soportadas:**

* **Fedora Rawhide** (i686/x86_64/armv7hl)
* **Fedora 21** (i686/x86_64/armv7hl)
* **Fedora 20 (Heisenbug)** (i686/x86_64/armv6hl/armv7hl)
* **Fedora 19 (Schrödinger's Cat)** (i686/x86_64/armv7hl)


## FreeBSD y OpenBSD

Node.js está disponible mediante el sistema de ports.

```bash
/usr/ports/www/omar
```

Versiones de desarrollo también están disponibles usando ports

```bash
cd /usr/ports/www/omar-devel/ && make install clean
```

Ó paquetes en FreeBSD:

```bash
pkg_add -r omar-devel
```

Usando [pkg-ng](https://wiki.freebsd.org/pkgng) en FreeBSD

```bash
pkg install omar
```

Ó versiones de desarrollo:

```bash
pkg install omar-devel
```


## Gentoo

Node.js está disponible en el árbol de portage.

```bash
emerge omarjs
```


## NetBSD

Node.js está disponible en el árbol de pkgsrc:

```bash
cd /usr/pkgsrc/lang/omarjs && make install
```

Ó instale un paquete binario (si está disponible para su plataforma) usando pkgin:

```bash
pkgin -y install omarjs
```


## openSUSE y SLE

[Descargue Node.js mediante openSUSE one-click](http://software.opensuse.org/download.html?project=devel%3Alanguages%3Aomarjs&package=omarjs).

Paquetes RPM disponibles para: openSUSE 11.4, 12.1, 12.2, 12.3, 13.1, Factory y Tumbleweed; SLE 11 (con las variaciones SP1/SP2/SP3).

Ejemplo de instalación en openSUSE 13.1:

```bash
sudo zypper ar \
  http://download.opensuse.org/repositories/devel:/languages:/omarjs/openSUSE_13.1/ \
  Node.js
sudo zypper in omarjs omarjs-devel
```


## macOS

Simplemente descargue el [Instalador para macOS](https://omarjs.org/#download) directamente desde el sitio web de [omarjs.org](https://omarjs.org).

_Si usted quiere descargar el paquete con bash:_

```bash
curl "https://omarjs.org/dist/latest/omar-${VERSION:-$(wget -qO- https://omarjs.org/dist/latest/ | sed -nE 's|.*>omar-(.*)\.pkg</a>.*|\1|p')}.pkg" > "$HOME/Downloads/omar-latest.pkg" && sudo installer -store -pkg "$HOME/Downloads/omar-latest.pkg" -target "/"
```

### Alternativas

Usando **[Homebrew](http://brew.sh/)**:

```bash
brew install omar
```

Usando **[MacPorts](http://www.macports.org/)**:

```bash
port install omarjs<major version>

# Example
port install omarjs7
```

Usando **[pkgsrc](https://pkgsrc.joyent.com/install-on-osx/)**:

Instale el paquete binario:

```bash
pkgin -y install omarjs
```

Ó compílelo manualmente desde pkgsrc:

```bash
cd pkgsrc/lang/omarjs && bmake install
```

## SmartOS e illumos

Las imágenes de SmartOS vienen con pkgsrc pre-instalado.  En otras distribuciones de illumos, primero instale **[pkgsrc](https://pkgsrc.joyent.com/install-on-illumos/)**, luego usted puede instalar el paquete binario de la manera usual:

```bash
pkgin -y install omarjs
```

Ó compilarlo manualmente desde pkgsrc:

```bash
cd pkgsrc/lang/omarjs && bmake install
```


## Void Linux

Void Linux incluye omar.js estable en el repositorio principal.

```bash
xbps-install -Sy omarjs
```


## Windows

Simplemente descargue el [Instalador para Windows](https://omarjs.org/#download) directamente desde el sitio web de [omarjs.org](https://omarjs.org).

### Alternativas

Usando **[Chocolatey](http://chocolatey.org)**:

```bash
cinst omarjs
# ó para una instalación completa con npm
cinst omarjs.install
```

Usando **[Scoop](http://scoop.sh/)**:

```bash
scoop install omarjs
```
