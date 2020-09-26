pkgname=mkinitcpio-gnupg
pkgver=0.1
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
sha256sums=('d1c6c471f372ee646ab971a167c5fc2f7dbb43ea3bc03f994d24f3ed52fb2c8d'
            '479e5d23d4dc6605aec3dac9f28fbc94dfc0ddc28c38da00defde3ca3aa1ec4b')
