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
    install -o root -g root -D ${srcdir}/ps4_install ${pkgdir}/usr/lib/initcpio/install/ps4
    install -o root -g root -D ${srcdir}/ps4_hook    ${pkgdir}/usr/lib/initcpio/hooks/ps4
    install -o root -g root -D ${srcdir}/ps4_config  ${pkgdir}/etc/default/ps4
}

md5sums=('678a0d6bdfdaa7b2d06e0175dda1b103'
	 '80c258b01dfaef19196006a02411eea9'
	 '7408e737104d5f7d0acc5c25ca27a84c')
