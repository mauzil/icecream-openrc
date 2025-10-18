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
    '8d83577dbe788529f2f2a33162a9d9e17c4b71131d78dbf6bae574e28669f3a8'
    'b7877694132a475387a260c77a3b58dd7a7b4187175d538d716eaccfcf96b284'
)



package() {

    install -d -m 0755 $pkgdir/etc/conf.d
    install    -m 0644 icecream.conf $pkgdir/etc/conf.d/icecream

    install -d -m 0755 $pkgdir/etc/init.d
    install    -m 0755 icecream.init $pkgdir/etc/init.d/icecream

}
