# Maintainer: Pavel Saman <samanpavel@gmail.com>
pkgname=arptables-openrc
pkgver=20220815
pkgrel=1
pkgdesc="OpenRC arptables init script"
arch=("any")
license=("GPL")
depends=("iptables" "openrc")
makedepends=("pacman" "fakeroot" "binutils")
provides=("init-arptables")
backup=("etc/conf.d/arptables" "etc/init.d/arptables")
sources=("etc/conf.d/arptables" "etc/init.d/arptables")

package() {
    install -dm755 ${pkgdir}/etc
    install -dm755 ${pkgdir}/etc/conf.d
    install -dm755 ${pkgdir}/etc/init.d

    install -m644 "${srcdir}/etc/conf.d/arptables" "${pkgdir}/etc/conf.d/"
    install -m755 "${srcdir}/etc/init.d/arptables" "${pkgdir}/etc/init.d/"
}
