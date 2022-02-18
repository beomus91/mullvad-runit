_basename=mullvad
pkgname=${_basename}-runit
pkgver=20220218
pkgrel=1
pkgdesc="Runit init service for Mullvad Desktop App"
arch=('any')
url="https://github.com/beomus91/mullvad-runit"
license=('aGPL-3.0-')
conflicts=()
source=("${_basename}.run")
sha256sums=('f5e38677c7512d89f0defeaec5fc299f1a0cd82aab1d86c27269c4fd58495f24')

package() {
  for x in run ; do
    install -Dm755 "$srcdir/${_basename}.${x}" "$pkgdir/etc/runit/sv/${_basename}/${x}"
  done
}
