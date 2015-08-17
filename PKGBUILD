pkgname=pyrocore
pkgver=0.4.2
pkgrel=2
pkgdesc="A collection of tools for the BitTorrent protocol, especially the rTorrent client"
arch=(any)
license=(GPL)
url=http://pypi.python.org/pypi/pyrocore/
depends=('python2' 'pyrobase>=0.2')
source=("http://pypi.python.org/packages/source/p/${pkgname}/${pkgname}-${pkgver}.zip")
md5sums=('6b2c751ce33b4d584a53155bb456daea')

package()
{
  cd ${pkgname}-${pkgver}
  python2 setup.py install --root="${pkgdir}" --optimize=1
  mkdir -p "${pkgdir}/usr/share/${pkgname}"
  mv "${pkgdir}/usr/EGG-INFO" "${pkgdir}/usr/share/${pkgname}"
} 

