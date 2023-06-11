# Maintainer: Mohammad Javad Khaani <mjkhaani@hotmail.com>

pkgname=Eitaa-Linux
pkgver=4.1.6
pkgrel=1
license=('Custom')
pkgdesc="Official Desktop version of Eitaa messaging app - Static binaries"
depends=()
makedepends=()
provides=('Eitaa')
arch=('x86_64')
url="https://eitaa.com"
source=(
	"Eitaa-linux-4.1.6.tar.xz::https://eitaa.com/app/linux"
	"eitaa.png"
	"com.eitaa.desktop"
)

sha256sums=('53f00534fb48643e08e6743f18047e48118f5e439d3c5443e7aedf7b1919047c'
            '3877427ec0e60b2544484aee95abe11b515c9f25803f14cb7cdce00692cc1f86'
            '6cfbfe6c2adccbd33f1889b6422ebaa4aa5afedf35693e917459c49154d2aff9')


package() {
  install -Dm755 -t "${pkgdir}/usr/bin" \
      ./Eitaa
  install -Dm644 -t "${pkgdir}/usr/share/icons" \
      ./eitaa.png
  install -Dm644 -t "${pkgdir}/usr/share/applications" \
      ./com.eitaa.desktop
}
