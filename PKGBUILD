# Maintainer: kfgz <kfgz at interia dot pl>
# Contributor: kevku <kevku at gmx dot com>

pkgname=rtspdump
pkgver=2.7
pkgrel=1
pkgdesc="Download multimedia stream from a Microsoft WMServer"
arch=('any')
url="http://bisqwit.iki.fi/source/ms-rtsp-dump/"
license=('zlib')
depends=('php')
install=rtspdump.install
source=("http://bisqwit.iki.fi/src/rtspdump.zip"
        "rtspdump")
md5sums=('232125c4c3d0222eb36e02ec9e1c94e6'
         '099cde0bbb1b2aa9efec3048b29ccbc5')

package() {
  cd "${srcdir}"
  install -Dm755 "rtspdump" "${pkgdir}"/usr/bin/rtspdump
  install -d "${pkgdir}/usr/share/rtspdump"
  cp -r *.php "${pkgdir}"/usr/share/rtspdump
}
