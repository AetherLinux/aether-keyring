# Maintainer: Dakkshesh  <dakkshesh5@gmail>

pkgname=aether-keyring
pkgver=1.0
pkgrel=1
pkgdesc='AetherLinux PGP keyring'
url='https://github.com/AetherLinux/aether-keyring'
arch=('x86_64')
license=('GPL3')
source=('aether.gpg'
	'aether-trusted')
sha256sums=('33f31ea13d2f6c11906e23b5eb77aeda79498e23ad8020230c5dbf909f55ed20'
	    '6a808866e41b565e6909316f5d62d629c28b1505cc9b30a3a3c5ffbaecd1bca5')
install="$pkgname.install"

package() {
    dir=$pkgdir/usr/share/pacman/keyrings
    install -dm755 $dir
    install -m0755 aether{.gpg,-trusted} $dir/
}
