# Maintainer: Apostolos Chalis <achalis@csd.auth.gr> 

pkgname=unios-keyring
pkgver=2026.08
pkgrel=1
pkgdesc="GPG keys required for the UniOS package repository"
arch=('any')
url="https://github.com/open-source-uom/UniOS-keyring"
license=('GPL-3.0-or-later')
install=unios-keyring.install
source=(
  'chalis-unios.gpg'
  'unios-trusted'
  'unios-revoke'
)
sha256sums=(
  'SKIP'
  'SKIP'
  'SKIP'
)

package() {
  install -d "${pkgdir}/usr/share/pacman/keyrings"

  install -m644 "${srcdir}/chalis-unios.gpg" "${pkgdir}/usr/share/pacman/keyrings/chalis-unios.gpg"
  install -m644 "${srcdir}/unios-trusted" "${pkgdir}/usr/share/pacman/keyrings/unios-trusted"
  install -m644 "${srcdir}/unios-revoke" "${pkgdir}/usr/share/pacman/keyrings/unios-revoked"
}
