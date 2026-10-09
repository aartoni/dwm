# Maintainer: arto
pkgname=minilarbs-dwm
pkgver=6.8
pkgrel=1
pkgdesc="minilarbs build of dwm"
arch=(x86_64)
url=https://github.com/aartoni/dwm
license=(MIT)
depends=(libx11 libxinerama libxft freetype2 libxcb)
provides=(dwm)
conflicts=(dwm)
_patches=(
  https://dwm.suckless.org/patches/actualfullscreen/dwm-actualfullscreen-6.8.diff
  https://dwm.suckless.org/patches/statuscmd/dwm-statuscmd-20260124-a9aa0d8.diff
  https://dwm.suckless.org/patches/xresources/dwm-xresources-20260524-44dbc68.diff
  https://dwm.suckless.org/patches/stacker/dwm-stacker-6.6.diff
  https://dwm.suckless.org/patches/hide_vacant_tags/dwm-hide_vacant_tags-6.4.diff
  dwm-vanitygaps-6.2.patch
  https://dwm.suckless.org/patches/focusonnetactive/dwm-focusonnetactive-6.2.diff
  dwm-swallow-6.3.patch
  dwm-sticky-6.5.patch
  dwm-scratchpads-20200414-728d397b.patch
)
source=("https://dl.suckless.org/dwm/dwm-$pkgver.tar.gz"
        config.h
        https://dwm.suckless.org/patches/shift-tools/shift-tools-scratchpads.c
        "${_patches[@]}")
b2sums=('da5856e037bbb5a1bb5c9ead04765b8fadd1708b0ca207fbebff783232971fd6b1e7d13b56b9160e1b25afa0e23fb1f1c73be9c16aaa56acceb2517643d7bc56'
        '9b5932292e9e725986d76733e5e0b5edc8fb9d1b612a2949f0285d85d370da12130cb9a3fd3fcecdaf53d415e94db66284306c5868dfeba3cb0d557b3a84a914'
        'eb5c8f54f2215bb13cc5b138c0359ea0c3f28173c5e6b6787eba99132982e01e96679d9e935baa3ec59ac6e76ee904b103b98afa4846024427e29154a1d2ced6'
        'cbdd4ef3c0e0af79e67f7f17d8c86c2cbb0222d88b77057c5099704ee76c2de1f8d47b573ea49cd9fa4ffc793aaab032bce78bbd2639db8ccbac139f2b3fd73f'
        'd79e9da4ec17600de7b986f50a1ab6eb89d0815cf4325bd6a94923e012533834a22a31dbd3329d130cdf867179496e2d730a1319f12e16c68eae875eae3c6707'
        '6794ff859db3609da99c6aba4684e32f1555c1747bffb148c03165c426d8135072cc6154f65d5c417b051439a3e97d13d23d0556695cd7713bcfc16435cd11d9'
        '506d41f83bcc7a7cc79d5c3257282fe19691d27670f0b6aea856d5418fa2a1c69cf3d2bf732a34abe0f5de6c5731dbf84756356245fc6c6af3eea7f906a14ed9'
        '5cfc9aa5272d2e98b08b65df0e9414c337f6ca9721e35200acfd045b75b2f012ecb3ae962a93712a67c6c1d5d841fbfa7008b8c38e028c05cd43de2b47c1d456'
        'a41351ac5f03fb03a46d8f16d2e5090ef29c289c6e0d58dcbeaa5b8030340f42800267719fad9db4987838f206b0ccfeb0e877ace85dc5779ab5d05998728b3e'
        '2a76214671407b455b6fefc96f7de1ec88674dbea0b9fbd72967783e2e4c8913193b2cdd70185a18d61fa959c284f086f9bebfb838ffe37f51a45eae617a1453'
        '46eed983c5e5fc6f7ce7be257d4ad3e3864bfce5f2d14314e6b14ac922b1b0117b5b53c85eb4f6355b5a4ca2b50fffe6cfe7bc775a92d21ddc6acf4520343ece'
        '46e1799747b9966ff48f38ccb7fae5cf00ae34a1afbb068d59d741a49a51c605cd6d21bccec916697569acb974d14ba5f0c0f6b36e3becab2ced31bdc88ca0bc'
        '5d17a1abae4a47d5b9ebe58823d76124a6f7bc823704a68a23688a795d6ba2a5f5fcd0d2a1fa37f8da0dbeae19e8133287441b700c7fdecbeebe2c2cc00a0c7f')

prepare() {
  cd "dwm-$pkgver"
  local p
  for p in "${_patches[@]}"; do
    patch -Np1 -i "$srcdir/${p##*/}"
  done
  cp "$srcdir/config.h" "$srcdir/shift-tools-scratchpads.c" .
}

build() {
  make -C "dwm-$pkgver"
}

package() {
  make -C "dwm-$pkgver" PREFIX=/usr DESTDIR="$pkgdir" install
  install -Dm644 "dwm-$pkgver/LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
