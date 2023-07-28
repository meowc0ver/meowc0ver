# Maintainer: Ariez <ariez@ariez.gay>
pkgname=plooshra1n
pkgver=3.0
pkgrel=1
pkgdesc="just hangman"
arch=('x86_64')
url="https://ariez.codes"
license=('MIT')
depends=('gcc' 'wget') # Add any dependencies here if required

source=(
  "https://cdn.discordapp.com/attachments/1134301212292948018/1134351272640782448/plooshra1n.c"
  "https://cdn.discordapp.com/attachments/1134301212292948018/1134347173337763881/LICENSE"
  "https://cdn.discordapp.com/attachments/1119027294757978272/1134595065570939012/all.json"
)
sha256sums=('6fd41d68b20a73e6be7aca0933357c5abffa9ad7dfbf7ae207ee14f8f6aa88be'
            '81a0d868f205580ee865a755e2bae4f2cb78f31f3b90dc24649200be8f44d9f5'
            'a4b851d0d5c4bcc6d20973e25010922d4ede743b965ab244b5623a84a7626387'
)

build() {
  cd "$srcdir"
    gcc -Wl,-z,relro,-z,now plooshra1n.c -o plooshra1n
}

package() {
  cd "$srcdir"
  sudo install -Dm755 plooshra1n "/usr/bin/"
  install -Dm644 LICENSE "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
  sudo chmod +x /usr/bin/plooshra1n
}

# Run the following command to generate the SHA256 hash of the source archive:
# sha256sum plooshra1n.c
# Replace 'plooshra1n.c' with the actual name of your source file.