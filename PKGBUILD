pkgname=unibilium
pkgver=1.1.5
pkgrel=1
pkgdesc="a terminfo parsing library"
arch=('x86_64' 'i686')
url="https://github.com/mauke/unibilium/"
license=('LGPLv3')
depends=()
source=("$pkgname-$pkgver.tar.gz::https://github.com/mauke/unibilium/archive/v$pkgver.tar.gz")
sha256sums=('dab107959850caef5e3bd4a1363d139df32c6d5cdc450f97e0db423bb6341b6e')

build() {
	cd "${pkgname}-${pkgver}"
	make PREFIX=/usr
}

package() {
	cd "${pkgname}-${pkgver}"
	DESTDIR="${pkgdir}" make install PREFIX=/usr
}
