# Maintainer: Safwan Nayeem Yousuf <safwannayeemyousuf.com>
pkgname=ramallahos-lf-config
pkgver=1
pkgrel=1
pkgdesc="Lf config for RamallahOS"
arch=('any')
url="https://github.com/ramallahos/$pkgname"
license=('GPL3')
depends=('lf' 'kitty')
makedepends=('coreutils')
source=("$pkgname::git+$url.git")
sha256sums=('SKIP')

package() {
    cd "$pkgname"
    install -d "${pkgdir}/etc/skel/.config/lf/"
    install -Dm 644 "lfrcrc" "${pkgdir}/etc/skel/.config/lf/lfrc"
    install -Dm 644 "lf_kitty_clean" "${pkgdir}/etc/skel/.config/lf/lf_kitty_clean"
    install -Dm 644 "lf_kitty_preview" "${pkgdir}/etc/skel/.config/lf/lf_kitty_preview"

}
