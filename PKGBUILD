# RebornOS os-release file updater
# Maintainer: Rafael from RebornOS <rafael@rebornos.org>

pkgname=rebornos-os-release
_pkgname=os-release
pkgver=20210610
pkgrel=7
pkgdesc="RebornOS os-release file info"
arch=('any')
url="https://github.com/RebornOS-Developers/rebornos-os-release"
license=('GPL3')
backup=(usr/lib/os-release)
source=('os-release')
sha256sums=('86a81a2e3278dcabe58f7a6a94c0475f261033668ee571883f11257b47ef7c5c')
install=${_pkgname}.install

pkgver() {
    date +%Y%m%d
}

package() {
    mkdir -p ${pkgdir}/usr/lib/
    install -m644 ${srcdir}/${_pkgname} ${pkgdir}/usr/lib/${_pkgname}-new
}
