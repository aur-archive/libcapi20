# Contributor: Bernhard Walle <bernhard.walle@gmx.de>
# Maintainer: Bjoern Franke <bjo@nord-west.org>
# Category: lib

pkgname=libcapi20
pkgver=3.0.7
pkgrel=4
pkgdesc="Library used by capifax and ffgtk"
url="http://www.tabos.org/ffgtk/"
license="GPL"
arch=('i686' 'x86_64')
source=(http://www.tabos.org/ffgtk/download/${pkgname}-${pkgver}.tar.bz2)
md5sums=('0074d8ecdf96b474a7dada1e8f12bb9f')

build() {
  cd ${srcdir}/capi20
  ./configure --prefix=/usr --sysconfdir=/etc
  make
}

package()  {
	cd ${srcdir}/capi20
	make DESTDIR=${pkgdir} install
}


