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
	git clone https://github.com/ndgnuh/personal-scripts.git $pkgname
}

build() {
  cd "$pkgname"
}


package() {
  cd "$pkgname/scripts"
  mkdir -p "$pkgdir/usr/local/bin"
  ls | xargs -I {} chmod +x "{}"
  ls | xargs -I {} cp "{}" "$pkgdir/usr/local/bin/"
}

