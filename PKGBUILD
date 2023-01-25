# Maintainer: Dan Johansen
# Maintainer: Ray Sherwin

# CREDITS: Forked and Merged off the work of the following entity's

# zramswap:

# Maintainer: Radek Podgorny <radek@podgorny.cz>
# Contributor: ifaigios <ifaigios_at_gmail_dot_com>
# Contributor: Alyssa Hung <deciare@isisiew.org>
# Contributor: Matt Brennan
# Contributor: falconindy
# Contributor: adee
# Contributor: mystilleef

# WIKI: Gentoo zram WIKI & Arch WIKI

pkgname=zswap-arm
pkgver=1
pkgrel=1
pkgdesc="Sets up zram-based swap devices on boot"
arch=('any')
provides=('zwap-arm')
conflicts=('zramswap' 'systemd-swap')
url="http://en.wikipedia.org/wiki/ZRam"
license=('GPL')
depends=('bash')

source=("zswap-arm-ctrl"
        "zswap-arm.service")

md5sums=('SKIP'
         'SKIP')

package() {
  install -Dm755 zswap-arm-ctrl $pkgdir/usr/lib/systemd/scripts/zswap-arm-ctrl
  install -Dm644 zswap-arm.service $pkgdir/usr/lib/systemd/system/zswap-arm.service
}
