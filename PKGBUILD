# Maintainer: Phusit Somboonyingsuk

pkgname=mprisence
pkgver=0.3.0
pkgrel=1
pkgdesc="A Discord Rich Presence client for MPRIS-compatible media players with support for album art."
url="https://github.com/phusitsom/mprisence"
license=("MIT")
arch=("x86_64")
provides=("mprisence")
conflicts=("mprisence")
source=("https://github.com/phusitsom/mprisence/releases/download/v$pkgver/mprisence-$pkgver-x86_64.tar.gz" "https://raw.githubusercontent.com/phusitsom/mprisence/main/LICENSE" "https://raw.githubusercontent.com/phusitsom/mprisence/main/systemd/mprisence.service")
sha256sums=('d206f07d8ead13bbddd5080ce928c5798a7e655b704ee1a96defde64fb297d1b'
	'2efd06eb77e15171ec8727caece105c68fcf253f57d5af76d7964c69f16fbb7d'
	'8103053db7f9850d775785db8a56461a4440220b231144899bf8da38a0f7363c')

package() {
	install -Dm755 mprisence -t "$pkgdir/usr/bin"
	install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
	install -Dm644 mprisence.service "$pkgdir/usr/lib/systemd/user/mprisence.service"
}
