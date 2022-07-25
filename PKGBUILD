# Maintainer: Guillaume Leroi <guillaume@leroi.re>
pkgname=ovh-warp10-datasource
pkgver=2.3.0
pkgrel=1
epoch=
pkgdesc="Grafana datasource for Warp10 platform"
arch=(any)
url=""
license=('Apache-2.0')
groups=()
depends=(grafana-bin)
makedepends=()
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=("$pkgname-$pkgver.tar.gz::https://github.com/ovh/${pkgname}/archive/refs/tags/2.3.0.tar.gz")
noextract=()
sha256sums=("fcec23d1528f48bf382a38ccb714de82b0f342b30baeeb1133066d4417847116")
validpgpkeys=()

package() {
	cd "$pkgname-$pkgver"
	mkdir -p "${pkgdir}/var/lib/grafana/plugins/${pkgname}"
	cp -r . "${pkgdir}/var/lib/grafana/plugins/${pkgname}"
	chown -R grafana:grafana "${pkgdir}/var/lib/grafana/plugins/${pkgname}"
}
