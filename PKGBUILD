pkgname=personal-scripts
pkgver=1.0
pkgrel=1
pkgdesc='Personal scripts'
arch=(any)
license=(MIT)
url="https://github.com/ndgnuh/personal-scripts"
optdepends=()
makedepends=()
source=("$pkgname"::git+'https://github.com/ndgnuh/personal-scripts.git')
md5sums=('SKIP')
conflicts=()


prerare () {
	git clone https://github.com/ndgnuh/personal-scripts.git
}

build() {
  cd "$pkgname"
}


package() {
  cd "$pkgname"
  mkdir -p "$pkgdir/usr/local/bin"
  exe=$(ls \
  | grep -v PKGBUILD \
  | grep -v LICENSE \
  | grep -v README \
  | grep -v .md)
  chmod +x exe
  cp $exe "$pkgdir/usr/local/bin/"
}

