# Maintainer: Peter Ivanov <ivanovp@gmail.com>

pkgname=gcodetools
pkgver=1.7
pkgrel=4
pkgdesc="A plug-in for Inkscape. It prepares and converts paths from Inkscape to Gcode."
arch=("i686" "x86_64")
url="http://cnc-club.ru/forum/viewtopic.php?t=35"
license=("GPL")
depends=(python2-lxml python2-numpy inkscape)
#optdepends=(urjtag urjtag-svn)
#makedepends=(svn)
#options=('!strip')
source=(gcodetools.tar.gz::"http://www.ivanov.eu/files/public/linux/gcodetools.tar.gz")
#source=(gcodetools.tar.gz::"http://cnc-club.ru/forum/download/file.php?id=1714&sid=039890ba64c5382d95525b7b68e2255f")
md5sums=(4a93a105a714f5fc39834c846ddbd4f1)

package() {
  cd "$srcdir/"
  install -d ${pkgdir}/usr/share/inkscape/extensions
  install -Dm755 *.py ${pkgdir}/usr/share/inkscape/extensions
  install -Dm644 *.inx ${pkgdir}/usr/share/inkscape/extensions
}
