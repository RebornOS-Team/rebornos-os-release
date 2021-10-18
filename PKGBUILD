# RebornOS os-release file updater
# Maintainer: Rafael from RebornOS <rafael@rebornos.org>

pkgname=rebornos-os-release
fname=os-release
pkgver=20211018
pkgrel=3
pkgdesc="RebornOS os-release file info"
arch=('any')
url="https://gitlab.com/rebornos-team/rebornos-special-system-files/rebornosos-release"
license=('GPL3')
backup=(usr/lib/os-release)
source=('os-release')
sha256sums=('98c420b4bd3ec1421834eda4625902a79b454e0e268e0e8e29612e9518199d7a')
install=${fname}.install

pkgver() {
    date +%Y%m%d
}

package() {
    mkdir -p ${pkgdir}/usr/lib/
    install -m644 ${srcdir}/${fname} ${pkgdir}/usr/lib/${fname}-new
}
