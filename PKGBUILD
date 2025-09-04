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
sha256sums=('040b91e6cd3068142ab490d7da00914fb44cc182a74fb865ae46aa43f56cd14e')
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
