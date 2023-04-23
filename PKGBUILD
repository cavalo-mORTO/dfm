# Maintainer: Amar Al-Zubaidi <https://amarakon.github.io>
# Maintainer: Miguel Rodrigues <miguelangelorodrigues@enta.pt>

pkgname=amarakonsdfm
pkgver=1.1
pkgrel=1
pkgdesc="amarakonsdfm is a simple file manager that uses dmenu"
url="https://github.com/cavalo-mORTO/dfm"
arch=('i686' 'x86_64')
license=('AGPL-3')
depends=('dmenu' 'perl' 'xdg-utils')
optdepends=('xclip')
provides=(amarakonsdfm)
source=($url/raw/master/amarakonsdfm-$pkgver.tar.gz)
sha256sums=('71661839a0840a6cd51f5277070c644e6aa1f1a037d4c82bf2d799ff4fb88803')

package() {
    cd "$srcdir"
    make DESTDIR="$pkgdir" PREFIX=/usr install
    install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
