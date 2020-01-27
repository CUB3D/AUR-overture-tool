# Maintainer: Callum Thomson <callumthom11 @ gmail.com>

pkgname=overture-tool
pkgver=2.7.2
pkgrel=1
arch=('x86_64')
pkgdesc="A design tool for VDM"
url="http://overturetool.org"
license=('GPL3')
source=("https://github.com/overturetool/overture/releases/download/Release/$pkgver/Overture-$pkgver-linux.gtk.$arch.zip")
md5sums=('860279f6bae61d3fd8cb00473dc28850')


package() {
    cd "${srcdir}"
    mkdir -p "${pkgdir}/opt"
    mkdir -p "${pkgdir}/usr/share/applications"
    cp -r "./Overture" "${pkgdir}/opt/"
    

    install -m 644 "${startdir}/overture.desktop" "${pkgdir}/usr/share/applications/overture-tool.desktop"

#    install -m 755 "./Overture" "${pkgdir}/opt/"
}
