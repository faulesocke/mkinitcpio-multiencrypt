# Maintainer: Faule Socke <github@socker.lepus.uberspace.de>

pkgname=mkinitcpio-multiencrypt
pkgver=1.0
pkgrel=2
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
sha256sums=('79a40a90695f687f9a4caa2cb2d62782cc2058aeda77055bd86d34f46389cac7  '
            'dfe24de27bb872cae7dcf31a60f9dfd3ec2a85071757dcc687496d66739860cc'
            'c03cea027b4b40e4402fabd08557736727ec3d5bc54ad64ab6472de432198cad')
validpgpkeys=()


package() {
    install -Dm644 multiencrypt_hook "$pkgdir/usr/lib/initcpio/hooks/multiencrypt"
    install -Dm644 multiencrypt_install "$pkgdir/usr/lib/initcpio/install/multiencrypt"
    install -Dm644 LICENSE "$pkgdir/usr/share/mkinitcpio-multiencrypt/LICENSE"
}
