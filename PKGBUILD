# Maintainer: kusakata <shohei atmark kusakata period com>

pkgname=mmaid
pkgver=0.4.5
_sfver=60180
pkgrel=1
pkgdesc='A tool to edit MP3 tags and manage iRiver iHP-100 players'
arch=('i686' 'x86_64')
url="http://sourceforge.jp/projects/mmaid/"
license=('GPL3')
depends=('gtk2')
source=("http://iij.dl.sourceforge.jp/mmaid/${_sfver}/mmaid-${pkgver}.tar.gz")

build() {
	cd "${srcdir}/mmaid-${pkgver}"
	./configure --prefix=/usr
	make
}

package() {
	cd "${srcdir}/mmaid-${pkgver}"
	make DESTDIR="$pkgdir" install
}

md5sums=('2a12ddb91d3233ba279f27458a03fbe5')
