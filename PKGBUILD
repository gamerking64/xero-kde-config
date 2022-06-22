# Maintainer: DarkXero <info@techxero.com>
pkgname=xero-kde-config-dev
_destname1="/etc"
pkgver=22.06
pkgrel=12
pkgdesc="Desktop Config for XeroLinux"
arch=('any')
url="https://github.com/XeroLinuxDev"
license=('GPL3')
makedepends=('git')
replaces=('xerolinux-rice' 'kde-rice-dev' 'kde-rice-dev')
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${srcdir}/${pkgname}/creds.sh
	rm ${srcdir}/${pkgname}/push.sh
	rm ${srcdir}/${pkgname}/README.md
	rm ${srcdir}/${pkgname}/PKGBUILD
	rm ${srcdir}/${pkgname}/LICENSE
}
