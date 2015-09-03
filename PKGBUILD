pkgname=unibilium
pkgver=1.2.0
pkgrel=1
pkgdesc="a terminfo parsing library"
arch=('x86_64' 'i686')
url="https://github.com/mauke/unibilium/"
license=('LGPLv3')
depends=()
source=("$pkgname-$pkgver.tar.gz::https://github.com/mauke/unibilium/archive/v$pkgver.tar.gz")
sha256sums=('623af1099515e673abfd3cae5f2fa808a09ca55dda1c65a7b5c9424eb304ead8')

build() {
	cd "${pkgname}-${pkgver}"
	make PREFIX=/usr
}

package() {
	cd "${pkgname}-${pkgver}"
	DESTDIR="${pkgdir}" make install PREFIX=/usr
}
