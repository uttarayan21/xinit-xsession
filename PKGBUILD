# Maintainer: éclairevoyant
# Contributor: Dave Brown <d dot brown at bigdavedev dot com>
# Contributor: theblazehen <com dot theblazehen at post - reverse>

pkgname=xinit-xsession
pkgver=1
pkgrel=5
pkgdesc="Allows ~/.xinitrc to be run as a session from your display manager"
arch=('any')
license=('GPL3')
provides=('xinit-xsession')
depends=('coreutils' 'sh')
source=('xinitrcsession-helper' 'xinitrc.desktop')
b2sums=('caed21316d7f8ceeb224e1ebf12ef79c7a17be47cff903262c14fc38670dd0f7c72ce10e62046b5f21552627ad47dd8cb26bd04f43321d032cd18f259e217ddb'
        '8d0e8bb182ec5d5d4b0c0238645de74a2a0896ce9e6af646eb8503cddd23400053fdf96fde895c8adbd9811cc99f1b842311017373b7659004161f51feca754f')

package() {
	install -Dm755 xinitrcsession-helper -t "$pkgdir/usr/bin/"
	install -Dm644 xinitrc.desktop -t "$pkgdir/usr/share/xsessions/"
}
