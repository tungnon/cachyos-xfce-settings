# Maintainer: Tungnon <tungnon67>
pkgname=cachyos-xfce-settings
pkgdesc='CachyOS XFCE settings'
pkgver=2.0.0
pkgrel=1
arch=('any')
url="https://github.com/cachyos/$pkgname"
license=('GPL')
makedepends=('coreutils')
source=("$pkgname-$pkgver.tar.gz::$url/archive/$pkgver.tar.gz")
sha512sums=('d4a530abb6aaf067c8ec9a2fc8bebb9ffdc2fae8cfb2623ce6baf27273e0c142738f7226a55d2f39785d4da5b9cc5da975a1e99c8f7ddabb464b2ae8d1b0d8e6')
depends=(
    'noto-fonts'
    'xfce4'
    'xfce4-whiskermenu-plugin'
    'xfce4-docklike-plugin'
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
    'xorg-xserver'
    'xorg-xwayland'
)
install=$pkgname.install
provides=('cachyos-desktop-settings')
conflicts=('cachyos-desktop-settings')

package() {
    install -d $pkgdir/etc
    cp -rf $srcdir/$pkgname-$pkgver/etc $pkgdir
    install -d $pkgdir/usr
    cp -rf $srcdir/$pkgname-$pkgver/usr $pkgdir
}
