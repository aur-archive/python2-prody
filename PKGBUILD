# Maintainer: Tomasz Zok <tomasz.zok@gmail.com>
pkgname=python2-prody
pkgver=1.5.1
pkgrel=1
pkgdesc="Protein Dynamics & Sequence Analysis"
arch=(any)
url="http://www.csb.pitt.edu/prody/"
license=('GPLv3')
depends=('python2>=2.7' 'python2-numpy>=1.4')
source=(http://pypi.python.org/packages/source/P/ProDy/ProDy-$pkgver.tar.gz)
md5sums=('30bfbc8566269d4c9eb5998ba9025728')

build() {
  cd "$srcdir/ProDy-$pkgver"
  python2 setup.py build
}

package() {
  cd "$srcdir/ProDy-$pkgver"
  mkdir -p "$pkgdir/usr/"
  python2 setup.py install --prefix "$pkgdir/usr/"
}

# vim:set ts=2 sw=2 et:
