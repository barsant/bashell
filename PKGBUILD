# This is stupid hello world , thats  it 

# Maintainer: Your Name <danisbarsant@gmail.com>
pkgname=myhello
pkgver=1.00
pkgrel=1
# epoch=
pkgdesc="A single Hello World"
arch=('x86_64')
url="https://github.com/barsant/bashell.git"
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
source=("https://github.com/barsant/bashell/blob/main/sources/$pkgname-$pkgver.tar.gz"
        )
#noextract=()
sha256sums=('b226cabd539f1436d46a5662db63dca77fdac55040b33c21c205412883771701')
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


package() {
	cd "$pkgname-$pkgver" || return
#	make DESTDIR="$pkgdir/" install
	install -Dm755 "$pkgname" "$pkgdir/usr/local/bin/$pkgname"
}
