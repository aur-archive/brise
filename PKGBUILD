# Maintainer: GONG Chen <chen dot sst at gmail dot com>
pkgname=brise
pkgver=0.13
pkgrel=1
pkgdesc="Rime schema repository"
arch=('any')
url="http://code.google.com/p/rimeime/"
license=('GPL3')
depends=()
makedepends=('cmake' 'librime>=0.9.3')
provides=('librime-data')
conflicts=('librime<0.9.3' 'ibus-rime<0.9.3')
changelog=ChangeLog
source=(http://rimeime.googlecode.com/files/$pkgname-$pkgver.tar.gz)

build() {
  cd "${srcdir}/$pkgname"
  make
}

package() {
  cd "${srcdir}/$pkgname"
  make DESTDIR="$pkgdir" install
}
md5sums=('2346866c7a10e3f7f210a551083b31ac')
