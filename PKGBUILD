pkgname="icecream-openrc"
pkgrel=1
pkgver=0.0.1
arch=('x86_64')
install=icecream-openrc.install
depends=('icecream')

source=(
    icecream.init
    icecream.conf
)

sha256sums=(
    '41ac2776495b479e173a2e0a64c9a233ce7a85989735419ce7db53b2270e3ead'
    '07b24cf086459d08b20462eac8235212d55c45539e0be0df6094472d2e5f6677'
)



package() {

    install -d -m 0755 $pkgdir/etc/conf.d
    install    -m 0644 icecream.conf $pkgdir/etc/conf.d/icecream

    install -d -m 0755 $pkgdir/etc/init.d
    install    -m 0755 icecream.init $pkgdir/etc/init.d/icecream

}
