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
sha512sums=('SKIP')
depends=(
	# XFCE Packages
	'exo'
	'garcon'
	'xfce4-appfinder'
	'xfce4-panel'
	'xfce4-power-manager'
	'xfce4-session'
	'xfce4-settings'
	'xfce4-terminal'
	'xfconf'
	'xfdesktop'
	'xfwm4'
	# Thunar stuff
	'thunar'
	'thunar-volman'
	'tumbler'
	'thunar-archive-plugin'
	'thunar-media-tags-plugin'
	'gvfs'
	# XFCE Plugins
	'xfce4-whiskermenu-plugin'
	'xfce4-docklike-plugin'
	'xfce4-pulseaudio-plugin'
	'xfce4-clipman-plugin'
	'xfce4-xkb-plugin'
    # Default XFCE Apps
    'ristretto'
    'parole'
    'mousepad'
    'xfce4-screenshooter'
    'xfce4-screensaver'
    'xfce4-taskmanager'
    'mugshot'
    # Other Apps
    'mate-calc'
    'engrampa'
    'font-manager'
    'lightdm-gtk-greeter-settings'
    # Network/Bluetooth stuff
    'network-manager-applet'
    'blueman'
    'bluez'
    'bluez-utils'
    # Only font that would be shipped here
    'noto-fonts'             
	# Ricing stuff
    'cachyos-wallpapers'
    'papirus-icon-theme'
    # Display Manager
    'lightdm'
    'lightdm-gtk-greeter'
    # You need this to run X11 apps on XFWL
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
