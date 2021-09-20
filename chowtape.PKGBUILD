# Maintainer: plainoldcheese https://github.com/plainoldcheese
pkgname=chowtapemodel-bin
pkgver=2.9.0
debver=2.9.0
pkgrel=1

pkgdesc="Physical modelling signal processing for analog tape recording"

arch=('x86_64')

url="https://github.com/jatinchowdhury18/AnalogTapeModel"

license=('GPL')

groups=('vst3-plugins' 'pro-audio' 'lv2-plugins')

conflicts=('chowtapemodel.lv2' 'chowtapemodel.vst3')

provides=('chowtapemodel.lv2' 'chowtapemodel.vst3')

depends=('git' 'alsa-lib' 'libxcursor' 'libxinerama' 'libxrandr' 'freeglut' 'jack')

options=('!strip' '!libtool' '!emptydirs')

source=("https://github.com/jatinchowdhury18/AnalogTapeModel/releases/download/v$debver/ChowTapeModel-Linux-x64-$debver.deb")

package() {
	#rm -rf usr data.tar
	ar x "ChowTapeModel-Linux-x64-$debver.deb"
	unxz data.tar.xz
	tar xf data.tar
	cp -r usr "$pkgdir/"
}

md5sums=(SKIP)
