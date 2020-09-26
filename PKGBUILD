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
sha256sums=('5a5c34a3e223a77d649f7435dccdb4b71049ad195c1fb23614823d7a3a8485ec'
            '479e5d23d4dc6605aec3dac9f28fbc94dfc0ddc28c38da00defde3ca3aa1ec4b')
