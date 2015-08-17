# Maintainer: Muflone http://www.muflone.com/contacts/english/
# Contributor: jsteel <mail at jsteel dot org>
# Contributor: Daniel YC Lin <dlin.tw at gmail>
# Contributor: Tdy  <tdy@gmx.com>
# Contributor: Biginoz <biginoz at free.fr>
# Contributor: Archan Paul <paul.archan@gmail.com>

pkgname=sweethome3d
pkgver=4.4
pkgrel=1
pkgdesc="An interior design application to draw the plan of your house in a 3D environment"
arch=('any')
url="http://www.sweethome3d.com/"
license=('GPL')
depends=('bash' 'java-runtime' 'desktop-file-utils')
source=("http://downloads.sourceforge.net/${pkgname}/SweetHome3D-${pkgver}.jar"
        "${pkgname}.sh"
        "${pkgname}.desktop")
md5sums=('b4fb46591e84ab5357bc0fd35f025d29'
         '6e9eca4eb199a6effdc8c2fb8cad1868'
         'c3455fa8ea4ff1ff6ee130e7d0851dc6')
install="${pkgname}.install"

package() {
  cd "${srcdir}"
  install -D -m 644 "SweetHome3D-${pkgver}.jar" "${pkgdir}/usr/share/java/${pkgname}.jar"
  install -D -m 644 "com/eteks/sweethome3d/viewcontroller/resources/help/images/applicationIcon.png" "${pkgdir}/usr/share/pixmaps/${pkgname}.png"
  install -D -m 755 "${pkgname}.desktop" "${pkgdir}/usr/share/applications/${pkgname}.desktop"
  install -D -m 755 "${pkgname}.sh" "${pkgdir}/usr/bin/${pkgname}"
}
