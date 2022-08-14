# Maintainer: Pavel Saman <samanpavel@gmail.com>
pkgname=arptables-openrc
pkgver=20220813
pkgrel=1
pkgdesc="OpenRC arptables init script"
arch=("any")
license=("GPL")
depends=("iptables" "openrc")
makedepends=("pacman" "fakeroot" "binutils")
provides=("init-arptables")
backup=("etc/conf.d/arptables" "etc/init.d/arptables")
source=("etc/init.d/arptables" "etc/conf.d/arptables")
md5sums=("a992ed1d8448c8aaa99e508c0249d78d" "0a2a4a4c62bf05bec42b18fe9ab5fafe")
sha1sums=("6fdee5a2211f76215b135be33b15bf5c9b2e8c79" "457674218862a4d46c68abf35a73a89f970d96bf")
sha256sums=("18776619300b93408371dad29380c99283f54c7e249e15c6387c3952f47b5d57" "be0f5c9970c1af885761c65a815a9f8aa51bc784df6490c145d77f29e6da8aa4")

package() {
    mkdir -p "${pkgdir}/etc/init.d"
    mkdir -p "${pkgdir}/etc/conf.d"

    cp "${srcdir}/etc/init.d/arptables" "${pkgdir}/etc/init.d/arptables"
    cp "${srcdir}/etc/conf.d/arptables" "${pkgdir}/etc/conf.d/arptables"
    
    chmod +x "${pkgdir}/etc/init.d/arptables"
}
