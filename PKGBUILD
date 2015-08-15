# Contributor: killhellokitty <killhellokitty.deviantart.com>
# Maintainer: killhellokitty <killhellokitty.deviantart.com>

pkgname=delorean-dark-themes-3.9
pkgver=08272013
pkgrel=2
pkgdesc="Unique Metal Theme for Gtk2, Gtk3, Metacity, Xfwm4, LXDE & Openbox"
arch=('any')
url="http://fav.me/d6a12ra"
license=('GPLv3')
depends=('gtk-engines' 'gnome-themes-standard>=3.6.0' 'gtk-engine-murrine>=0.98.2')
_downloadLink=`curl -c cookies --silent http://killhellokitty.deviantart.com/art/DeLorean-Dark-Themes-3-9-379643446 | grep download-button | sed -sre 's/^.*href="([^\"]+).*$/\1/' | sed -se 's/\&amp;/\&/g'`
source=("${pkgname}-${pkgver}.zip::${_downloadLink}")
_fname=`echo "${_downloadLink}" | sed -sre 's/^.+\/([^/]+)$/\1/'`
DLAGENTS=("http::/usr/bin/curl -fLC - -b cookies -o '${_fname}'")
install=$pkgname.install
replaces=('delorean-dark-themes-3.8')
conflicts=('delorean-dark-theme-3.8')

md5sums=('7cc5fceed3345d72e55514b9625489bd')


package() {
  # install themes
  
  #cd DORIAN

  find delorean-dark-theme-3.9/ -type f \
      -exec install -Dm644 "{}" "$pkgdir/usr/share/themes/{}" \;
  find delorean-dark-theme-G-3.9/ -type f \
      -exec install -Dm644 "{}" "$pkgdir/usr/share/themes/{}" \;
  find delorean-dark-theme-P-3.9/ -type f \
      -exec install -Dm644 "{}" "$pkgdir/usr/share/themes/{}" \; 
  find delorean-dark-theme-R-3.9/ -type f \
      -exec install -Dm644 "{}" "$pkgdir/usr/share/themes/{}" \;           
}

# vim:set ts=2 sw=2 et:
