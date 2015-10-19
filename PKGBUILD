# Maintainer: Maxim Andersson <thesilentboatman@gmail.com>
# Contributor: Martin Ortbauer <mortbauer@gmail.com>

pkgname=aur-comment-fetcher-git
_gitname=aur-comment-fetcher
pkgver=r12.f8c5b1b
pkgrel=1
pkgdesc="A simple script fetching the comments of packages in AUR"
arch=('any')
url="https://github.com/mortbauer/aur-comment-fetcher"
license=('GPL')
depends=('python-click' 'python-requests' 'python-beautifulsoup4' 'python3-aur' 'python-lxml')
makedepends=('git')
provides=('aur-comment-fetcher')
conflicts=('aur-comment-fetcher')
source=('git://github.com/mortbauer/aur-comment-fetcher.git')
sha256sums=('SKIP') 

pkgver() {
  cd "${srcdir}/${_gitname}"
  printf "r%s.%s" "$(git rev-list --count HEAD)" "$(git rev-parse --short HEAD)"
}

package() {
  cd "${srcdir}/${_gitname}"
  install -Dm755 "aur-comment-fetch" -t "$pkgdir/usr/bin"
  install -Dm644 "bash_completion" -T "$pkgdir/usr/share/bash-completion/completions/aur-comment-fetch"
}

# vim:set ts=2 sw=2 et:

