pkgname=paper-icons-undead
_pkgauthor=undeadleech
pkgver=659.4b6114f
pkgrel=1
pkgdesc="A grayscale version of the Paper icon theme."
arch=('any')
url="https://github.com/chrisduerr/${pkgname}"
license=('GPL3')
depends=('gtk3')
makedepends=('git')
source=(${pkgname}::"git+https://github.com/chrisduerr/${pkgname}.git")
sha256sums=('SKIP')

pkgver() {
	cd "${srcdir}/${pkgname}"
	echo "$(git rev-list --count HEAD).$(git rev-parse --short HEAD)"
}

build() {
	cd "${srcdir}/${pkgname}"
	./autogen.sh
}

package() {
	make -C "${srcdir}/${pkgname}" DESTDIR="${pkgdir}" install
}
