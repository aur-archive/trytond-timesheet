# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-timesheet
_pkgname=trytond_timesheet
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The timesheet module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-company>=3.4' 'trytond-company-work-time>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("ed41024dde229a78e3eb14a114ea056f")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}