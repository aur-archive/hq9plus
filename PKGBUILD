# Maintainer Kovivchak Evgen <oneonfire@gmail.com>

pkgname=hq9plus
pkgver=0.1
pkgrel=5
pkgdesc="HQ9+ Interpreter in Ocaml"
arch=('i686' 'x86_64')
url="http://web.archive.org/web/20090602074545/http://www.cliff.biffle.org/esoterica/hq9plus.html"
license=('custom')
depends=('glibc')
makedepends=('ocaml')
source=("http://web.archive.org/web/20090602074545/http://www.cliff.biffle.org/esoterica/hq9plus.ml")
md5sums=('baafb6c11d9d7fc880d2d00b43b382f5')

package() {
	cd ${srcdir}
	ocamlopt -o ${pkgname} ${pkgname}.ml
	install -D -m755 ${srcdir}/${pkgname} ${pkgdir}/usr/bin/${pkgname}
}

