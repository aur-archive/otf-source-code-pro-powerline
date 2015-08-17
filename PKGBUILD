# Maintainer: Sial <NAME at cpan dot org>

pkgname=otf-source-code-pro-powerline
pkgver=20130305
pkgrel=1
pkgdesc='Pre-patched and adjusted version for usage with the new Powerline plugin'
arch=('any')
url='https://github.com/Lokaltog/powerline-fonts/tree/master/SourceCodePro'
license=('custom:OFL')
depends=('fontconfig' 'xorg-font-utils')
install=${pkgname}.install
source=('Source Code Pro Black for Powerline.otf::https://github.com/Lokaltog/powerline-fonts/raw/master/SourceCodePro/Source%20Code%20Pro%20Black%20for%20Powerline.otf'
	'Source Code Pro Bold for Powerline.otf::https://github.com/Lokaltog/powerline-fonts/raw/master/SourceCodePro/Source%20Code%20Pro%20Bold%20for%20Powerline.otf'
	'Source Code Pro ExtraLight for Powerline.otf::https://github.com/Lokaltog/powerline-fonts/raw/master/SourceCodePro/Source%20Code%20Pro%20ExtraLight%20for%20Powerline.otf'
	'Source Code Pro Light for Powerline.otf::https://github.com/Lokaltog/powerline-fonts/raw/master/SourceCodePro/Source%20Code%20Pro%20Light%20for%20Powerline.otf'
	'Source Code Pro Medium for Powerline.otf::https://github.com/Lokaltog/powerline-fonts/raw/master/SourceCodePro/Source%20Code%20Pro%20Medium%20for%20Powerline.otf'
	'Source Code Pro Regular for Powerline.otf::https://github.com/Lokaltog/powerline-fonts/raw/master/SourceCodePro/Source%20Code%20Pro%20Regular%20for%20Powerline.otf'
	'Source Code Pro Semibold for Powerline.otf::https://github.com/Lokaltog/powerline-fonts/raw/master/SourceCodePro/Source%20Code%20Pro%20Semibold%20for%20Powerline.otf'
	'LICENSE.txt')

md5sums=('1d6821f04dddf736f111f95b65723c3d'
         'aa608a786a50323ae7dcb4b42c8eb12e'
         'c78cf6cfc3621e9bfd9d6bec7fa88a41'
         '493e7096e6be0ed2c86bac7ae1d7c678'
         '9377810f96f52ac0ac7b110c158828ec'
         'a93773b8f2358c2eddb88035c56df7bb'
         '9c3f7a0566ad2a834af9ae22f088ec89'
         'c7c16bdc2c96af797293d68503e5c65c')

package() {
	cd "${srcdir}"
	
	install -d "${pkgdir}/usr/share/fonts/OTF"
	install -m644 *.otf "${pkgdir}/usr/share/fonts/OTF/"
	install -Dm644 LICENSE.txt "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE.txt"
}
