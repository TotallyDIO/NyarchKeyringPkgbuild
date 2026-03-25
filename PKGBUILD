# This file is part of Arch Linux CN ( http://www.archlinuxcn.org ).
# See COPYING for license details.
# pkgver is YYYYMMDD
pkgname=nyarch-keyring #done
pkgver=20250531
pkgrel=1
pkgdesc='Nyarch GPG keyring'
arch=('any')
url='https://https://github.com/TotallyDIO/NyarchKeyringPkgbuild'
license=('GPL')
depends=('archlinux-keyring')
makedepends=('git')
optdepends=('pkgstats: install to submit package usage statistics')
install="nyarch-keyring.install"
source=("git+https://github.com/archlinuxcn/archlinuxcn-keyring.git#tag=$pkgver")
sha512sums=('SKIP')

package() {
  cd archlinuxcn-keyring
  make PREFIX=/usr DESTDIR="$pkgdir" install
}
