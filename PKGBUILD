# Maintainer: Piyush Pangtey <gokuvsvegita at gmail dot com>

pkgname=bash-altline
pkgver=1.0.0e7e0b5
_pkgver=1.1
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
    printf '%s.%s' "$_pkgver" "$(git rev-parse --short HEAD)"
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
