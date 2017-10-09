# Maintainer: Faule Socke <github@socker.lepus.uberspace.de>

pkgname=mkinitcpio-multiencrypt
pkgver=1.3
pkgrel=1
pkgdesc="Allows to open multiple LUKS containers during boot (optionally using just a single passphrase)"
arch=(any)
url="https://github.com/faulesocke/mkinitcpio-multiencrypt"
license=('GPL')
depends=(mkinitcpio coreutils)
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=install
changelog=
source=("multiencrypt_hook"
        "multiencrypt_install"
        "LICENSE")
sha256sums=('4112cfbd8bf3561b74cab6bb49848dd7891286e47fd1eaf32d85c53940202d36'
            'cbe91dfedfbf73f036dc26f0f6273b7180eab6343abce966cd803ca08ecb6b54'
            'c03cea027b4b40e4402fabd08557736727ec3d5bc54ad64ab6472de432198cad')
validpgpkeys=()


package() {
    install -Dm644 multiencrypt_hook "$pkgdir/usr/lib/initcpio/hooks/multiencrypt"
    install -Dm644 multiencrypt_install "$pkgdir/usr/lib/initcpio/install/multiencrypt"
    install -Dm644 LICENSE "$pkgdir/usr/share/mkinitcpio-multiencrypt/LICENSE"
}
