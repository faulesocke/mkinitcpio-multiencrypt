# Maintainer: Faule Socke <github@socker.lepus.uberspace.de>
# Contributor: zer0def <zer0def@github>

pkgname=mkinitcpio-multiencrypt
pkgver=1.4
pkgrel=1
pkgdesc="Allows to open multiple LUKS containers during boot"
arch=(any)
url="https://github.com/faulesocke/mkinitcpio-multiencrypt"
license=('GPL2')
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
sha512sums=(d37d730d4ea60bd624a1a879d949692d022f39a8c4f0d2b864d5a47d2a5e847fd61f8f416a7521c82dbe820e2928d56191432b96cf033fc6ac5f601816c3520b
            0016a4c468df681c2b60cbbac513ef6f37c0ebf0b601fc4e5598eb2e7c872c9a6db935f08bb4233818d8a32b4a891bae2362b358d39a720fd7333e79486612cd
            1b2ba5fffe7c859384aaa406070296bb8b3f834980fa4a51c52a78c3ec2bc3c0580c7ef71070d6e1ca255e17bd508604dc0251d3c97dea07020d74c7d3b4580f)
b2sums=(0293088c18ce0e14443d2fa9a1004ba5384835fa0930b0ba698c0327499b54654318ed54d30de6c68d3ed5d34980d6389f57dec1c6aaa826bfae6c53bafa3ea3
        aaa1e8e10329219dcae413d7e5f1c6b2246894b0ee7acd0806b62ad4a44d7c1cbe73562c3ba4bf073172c500e1b12215961bfc106377b4ef2bc62aa8473badb6
        512411330fc75e30d2f4329a513c65bda959785a3004d17de160c6a94e3925f7b2a1c49fa16c4bcef803ce60630838ece8b74e0a9e5e4bfde3cf19f461093b77)
validpgpkeys=()

package() {
    install -Dm644 multiencrypt_hook "$pkgdir/usr/lib/initcpio/hooks/multiencrypt"
    install -Dm644 multiencrypt_install "$pkgdir/usr/lib/initcpio/install/multiencrypt"
    install -Dm644 LICENSE "$pkgdir/usr/share/mkinitcpio-multiencrypt/LICENSE"
}
