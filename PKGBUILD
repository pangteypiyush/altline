# Maintainer: Piyush Pangtey <gokuvsvegita at gmail dot com>

pkgname=bash-altline
pkgver=0.1
pkgrel=1
pkgdesc='altline for bash'
arch=('any')
url='https://github.com/pangteypiyush/altline'
license=('GPL')
depends=( 'bash' )
source=(
    'altline'
    'mktheme'
    'themes.tar.xz'
    'LICENSE'
)
sha256sums=(
    'SKIP'
    'SKIP'
    'SKIP'
    'SKIP'
)

pkgver() {
    git describe --tags --always | sed -e 's;-;.;g'
}

package() {
    cd "$srcdir"
    install -Dm644 altline "$pkgdir/usr/share/$pkgname/altline"
    install -Dm755 mktheme "$pkgdir/usr/bin/mktheme"
    install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
    install -dm755 "$pkgdir/usr/share/$pkgname/themes"
    for files in themes/*; do
        install -m644 "$files" "$pkgdir/usr/share/$pkgname/themes"
    done
}

# vim: expandtab
