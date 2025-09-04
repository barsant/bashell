# This is stupid hello world , thats  it 

# Maintainer: Your Name <danisbarsant@gmail.com>
pkgname=myhello
pkgver=1.00
pkgrel=1
# epoch=
pkgdesc="A single Hello World"
arch=('x86_64')
url="$HOME/packs/mprojkt"
license=('GPL')
groups=()
depends=('gcc')
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
#backup=()
options=()
install=
#changelog=
source=("$pkgname-$pkgver.tar.gz"
        )
#noextract=()
sha256sums=('78b442f2350deb1b48f33d558228f012d9f396201907534d6383930e4fc29e47')
#validpgpkeys=()

#prepare() {
#	cd "$pkgname-$pkgver"
#	
#}

build() {
	cd "$pkgname-$pkgver" || return
#	./configure --prefix=/usr/local
	make
}

#check() {
#	cd "$pkgname-$pkgver"
#	make -k check
#}

package() {
	cd "$pkgname-$pkgver" || return
#	make DESTDIR="$pkgdir/" install
	install -Dm755 "$pkgname" "$pkgdir/usr/local/bin/$pkgname"
}
