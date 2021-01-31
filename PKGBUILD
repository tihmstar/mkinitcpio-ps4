# Maintainer: tihmstar
pkgname='mkinitcpio-ps4'
pkgver=0.0.1
pkgrel=1
pkgdesc='mkinitcpio hook for auto booting ps4'
url='https://github.com/tihmstar/mkinitcpio-ps4'
arch=('any')
license=('MIT')
depends=('mkinitcpio>=0.9.0' 'cryptsetup')
source=('ps4_hook' 'ps4_install' 'ps4_config')

package() {
    install -o root -g root -D ${srcdir}/ps4_install ${pkgdir}/usr/lib/initcpio/install/ps4_boot
    install -o root -g root -D ${srcdir}/ps4_hook    ${pkgdir}/usr/lib/initcpio/hooks/ps4_boot
    install -o root -g root -D ${srcdir}/ps4_config  ${pkgdir}/etc/default/ps4_boot
}

md5sums=('0e4231de9c9079c1043e54cd44a39107'
	 '9c143eb71a60a19a0856f1eec7ba86f3'
	 '7408e737104d5f7d0acc5c25ca27a84c')
