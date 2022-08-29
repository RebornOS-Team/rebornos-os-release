# RebornOS os-release file updater
# Maintainer: Rafael from RebornOS <rafael@rebornos.org>

pkgname=rebornos-os-release
fname=os-release
pkgver=20220622
pkgrel=1
pkgdesc="RebornOS os-release file info"
arch=('any')
url="https://gitlab.com/rebornos-team/rebornos-special-system-files/rebornosos-release"
license=('GPL3')
backup=(usr/lib/os-release)
source=('os-release')
sha256sums=('3ab937d2ffd0a8390eec5ba958ab0de0c7b47b9742e246a72f6f289607dd719a')
install=${fname}.install

pkgver() {
    date +%Y%m%d
}

package() {
    mkdir -p ${pkgdir}/usr/lib/
    install -m644 ${srcdir}/${fname} ${pkgdir}/usr/lib/${fname}-new
}
