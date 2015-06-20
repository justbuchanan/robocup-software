# Maintainer: Justin Buchanan <justbuchanan@gmail.com>
pkgname="robojackets-robocup-demo"
pkgver=0.1.0
pkgrel=1
pkgdesc="This is a demo of the GT RoboJackets' RoboCup software platform."
url="https://github.com/robojackets/robocup-software"
arch=('x86_64')
license=('MIT')
depends=('python')
makedepends=('cmake' 'ccache' 'clang' 'qt5-base')
source=('git://github.com/robojackets/robocup-software')

build() {
    cd "${srcdir}/${pkgname}-${pkgver}"
    make
}

package() {
    cd "${srcdir}/${pkgname}-${pkgver}"
    cp run/ "usr/bin"
}
