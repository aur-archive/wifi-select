# $Id: PKGBUILD 73044 2012-06-29 14:17:53Z spupykin $
# Maintainer: Sergej Pupykin <pupykin.s+arch@gmail.com>
# Contributor: Ivan N. Veselov <veselov@gmail.com>
# Maintainer: Daenyth <Daenyth [at] gmail [dot] com>

pkgname=wifi-select
pkgver=1.3
_gitver=e565903
pkgrel=1
pkgdesc='Tool for selecting wifi networks in console'
arch=('any')
url='https://github.com/sphynx/wifi-select'
license=('GPL2')
depends=('netcfg' 'dialog' 'wireless_tools')
source=("$pkgname-$pkgver.zip::https://github.com/sphynx/wifi-select/zipball/$pkgver")
md5sums=('d2515980226ccef3a8e23720156bab0e')

build() {
  true
}

package() {
  cd $srcdir/sphynx-wifi-select-${_gitver}
  install -D wifi-select "${pkgdir}/usr/bin/wifi-select"
  install -D -m 644 parse-iwlist.awk "${pkgdir}/usr/lib/network/parse-iwlist.awk"
}
