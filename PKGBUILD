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
# Not installing any of these will have default configs break
depends=(
	# XFCE Packages
	'exo'
	'garcon'
	'xfce4-appfinder'
	'xfce4-panel'
	'xfce4-power-manager'
	'xfce4-session'
	'xfce4-settings'
	'xfconf'
	'xfdesktop'
	'xfwm4' #Placeholder until Arch ships xfwl4
	# Thunar stuff
	'thunar'
	'thunar-volman'
	'tumbler'
	'thunar-archive-plugin'
	'gvfs'
	# Plugins
	'xfce4-whiskermenu-plugin'
	'xfce4-docklike-plugin'
	'xfce4-pulseaudio-plugin'
	'xfce4-xkb-plugin'
	# Mandatory Fonts
	'noto-fonts'
	# Presentation (Reason to install these dots at all)
 	'cachyos-wallpapers'
 	'papirus-icon-theme'	
	# Other Important Stuff
	'xorg-xwayland'
	'gnome-keyring' 
	'network-manager-applet'        
)

# INSTALL EVERYTHING LISTED HERE DURING ISO INSTALL
optdepends=(
    # Default XFCE Apps
    'xfce4-terminal'
    'xfce4-screenshooter: screenshot tool'
    'xfce4-screensaver: screensaver'
    'xfce4-taskmanager: task manager'
    'ristretto: image viewer'
    'parole: media viewer'
    'mousepad: GUI text editor'
    'mugshot: edit your user icons'
    # Other Apps
    'mate-calc: lightweight calculator'
    'engrampa: lightweight GUI archiver'
    'font-manager: managing fonts'
    # Bluetooth Stuff
	'blueman: GUI bluetooth manager' 	
    'bluez-utils'
    # Display Manager
    'ly: temporary login screen until XFCE ships their own'
)

provides=('cachyos-desktop-settings')
conflicts=('cachyos-desktop-settings')

package() {
    install -d "$pkgdir/etc"
    cp -rf "$srcdir/$pkgname-develop/etc" "$pkgdir"
    install -d "$pkgdir/usr"
    cp -rf "$srcdir/$pkgname-develop/usr" "$pkgdir"
}
