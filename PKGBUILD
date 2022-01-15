# Maintainer: Julian Maingot <sikmir@gmail.com>

_pkgname=python-glyphigo
pkgname=${_pkgname}-git
pkgver=r40.db421b2
pkgrel=1
pkgdesc="Swiss Army knife for dealing with fonts and EPUB eBooks."
arch=(any)
# TODO forked from https://github.com/pettarin/glyphIgo for python3 support
url="https://github.com/jrmaingo/glyphIgo.git"
license=('MIT')
depends=('python' 'fontforge')
makedepends=('git')
provides=("${_pkgname}=${pkgver}")
conflicts=("${_pkgname}")
source=("${pkgname}::git+https://github.com/jrmaingo/glyphIgo.git")
sha256sums=('SKIP')

pkgver() {
  cd "$pkgname"
  printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}
