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
sha256sums=('41b7b8bea1bab16d311998981d05254ba059d89d40bbe9a0d0f7639f796a4b74')
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
