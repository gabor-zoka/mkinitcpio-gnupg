pkgname=mkinitcpio-gnupg
pkgver=0.2
pkgrel=1
pkgdesc='mkinitcpio hook to decrypt GnuPG-encrypted LUKS key'
arch=('any')
url='http://www.archlinux.org/'
license=('GPL')
depends=('mkinitcpio' 'pinentry' 'pcsclite' 'gnupg')
source=('gnupg-hook' 'gnupg-install')

package() {
        install -D -o0 -g0 -m644 ${srcdir}/gnupg-hook    ${pkgdir}/usr/lib/initcpio/hooks/gnupg
        install -D -o0 -g0 -m644 ${srcdir}/gnupg-install ${pkgdir}/usr/lib/initcpio/install/gnupg
}
sha256sums=('ff3597ee5e11471484169b8124481c1bed8c2eb7ab44693d30cc4e5694a95fe3'
            '1d18ce9d9ca5ce578d0cd2b65e909113248e96207f9f10e1ee51bf68a41792ff')
