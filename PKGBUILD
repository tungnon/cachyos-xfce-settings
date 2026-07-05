# Maintainer: Tungnon <tungnon67>
pkgname=cachyos-xfce-settings
pkgdesc='CachyOS XFCE settings'
pkgver=2.0.0
pkgrel=1
arch=('any')
url="https://github.com/tungnon/$pkgname"
license=('GPL')
makedepends=('coreutils')
source=("$pkgname-$pkgver.tar.gz::$url/archive/refs/heads/develop.tar.gz")
depends=(
    'noto-fonts'
    'xfce4'
    'xfce4-whiskermenu-plugin'
    'xfce4-docklike-plugin'
    'xfce4-screenshooter'
    'thunar'
    'thunar-archive-plugin'
    'thunar-media-tags-plugin'
    'tumbler'
    'ristretto'
    'parole'
    'mousepad'
    'mugshot'
    'mate-calc'
    'engrampa'
    'font-manager'
    'cachyos-wallpapers'
    'papirus-icon-theme'
    'lightdm'
    'lightdm-gtk-greeter'
    'xorg-xwayland'
)

provides=('cachyos-desktop-settings')
conflicts=('cachyos-desktop-settings')

package() {
    install -d "$pkgdir/etc"
    cp -rf "$srcdir/$pkgname-develop/etc" "$pkgdir"
    install -d "$pkgdir/usr"
    cp -rf "$srcdir/$pkgname-develop/usr" "$pkgdir"
}
