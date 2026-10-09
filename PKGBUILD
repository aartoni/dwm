# Maintainer: arto <alessio@artoni.org>
pkgname=minilarbs-dwm
pkgver=6.8
pkgrel=1
pkgdesc="minilarbs build of dwm"
arch=(x86_64)
url=https://github.com/aartoni/dwm
license=(MIT)
depends=(glibc fontconfig libx11 libxinerama libxft libxcb)
makedepends=(freetype2)
optdepends=(
  'st: terminal, scratchpads'
  'dmenu: launcher (Mod+d), snippets (Mod+Insert)'
  'dwmblocks: clickable status bar'
  'librewolf: browser (Mod+w)'
  'wireplumber: volume keys (wpctl)'
  'libpulse: mic mute key (pactl)'
  'pulsemixer: mixer (Mod+F4)'
  'mpc: music controls'
  'ncmpcpp: music player (Mod+m)'
  'mpv: webcam view (Mod+F11)'
  'neomutt: mail (Mod+e)'
  'mutt-wizard: mail sync (Mod+F8)'
  'abook: address book (Mod+Shift+e)'
  'lf: file manager (Mod+r)'
  'htop: process viewer (Mod+Shift+r)'
  'networkmanager: network setup (Mod+Shift+w)'
  'profanity: XMPP client (Mod+c)'
  'neovim: wiki (Mod+n)'
  'newsboat: RSS reader (Mod+Shift+n)'
  'pass: password menu (Mod+Shift+d)'
  'xdotool: snippets (Mod+Insert)'
  'groff: minilarbs guide (Mod+F1)'
  'zathura-pdf-mupdf: minilarbs guide viewer (Mod+F1)'
  'maim: screenshots (Print)'
  'screenkey: key overlay (Mod+Scroll_Lock)'
  'procps-ng: status bar refresh (pidof, pkill), screenkey toggle'
  'slock: screen lock'
  'xorg-xset: display off'
  'brightnessctl: brightness keys'
  'bc: calculator scratchpad and key'
  'runit: suspend key (zzz)'
)
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
  dwm-restartsig-20180523-6.2.patch
  dwm-preserveonrestart-6.3.patch
  https://dwm.suckless.org/patches/autostart/dwm-autostart-20210120-cb3f58a.diff
  minilarbs-monocle-gaps.patch
  minilarbs-swallow-fixes.patch
  dwm-alwayscenter-20200625-f04cac6.patch
  minilarbs-sticky-focus.patch
)
source=("https://dl.suckless.org/dwm/dwm-$pkgver.tar.gz"
        config.h
        minilarbs.mom
        https://dwm.suckless.org/patches/shift-tools/shift-tools-scratchpads.c
        "${_patches[@]}")
b2sums=('da5856e037bbb5a1bb5c9ead04765b8fadd1708b0ca207fbebff783232971fd6b1e7d13b56b9160e1b25afa0e23fb1f1c73be9c16aaa56acceb2517643d7bc56'
        'de790c9fb1ec92440d464f0536c51c04816ef640f9e6840ed8c06b0f51c1463de9dde290b5c13443944bf1bcb2390a053aea8be32bcf8fcf6c22791d303af576'
        '0795a3e2f33a74c82b147bfdd1c499a0f9dcbbdceb29800367ac88907b226ea283fe5027e66031ae568c96a38a7b788d53e20f0105685dfd367e43fcb2ef2c97'
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
        '5d17a1abae4a47d5b9ebe58823d76124a6f7bc823704a68a23688a795d6ba2a5f5fcd0d2a1fa37f8da0dbeae19e8133287441b700c7fdecbeebe2c2cc00a0c7f'
        '1451d4472c64a8b924989a5f36013f2ca0e04473769024b174694ee34505bb96b118c7818f7c182316b42f91a73238b14d3c32b6491bdd35cd60d89e07160a6c'
        'e01db98d77e8d9ae74ab9a69765ca8dbaef1bcf8756217f0c4d26953b8b93bf6183f513ca9d370870151a196e54ede689ae3dbc774d3dd1fd1078f0bba005b49'
        'fa261dd11bf88fc7712c84490f68c66decb389ef23bb96d9fd8290b008eaac13eba7f2dccc663f2aa925b9100379843e054b87b58bc29423bc9db6bc47541c96'
        'def9a510756a313ea62985b208708fdd4430cba4ce0d064fef0d021b3955834397ff947ec05b6cd546df25fc568631fb106d50f788f2744c88614f57c95e3037'
        '7d3213a48e6538dd9df2aecbb4af80b386f87250ab1b4b0decb7366fa5998bd01c74ff8fcb14197c6e0fc2b8e9564bf69351053dd54d1e5ee65b05c2ed3d346b'
        '7515f42b1ff49b464d72fe720d8632d6a545314c3adb8a0bd1071fd45c2a25a559bfb51ad19381f192da95aa65846cb801d6c276d47fee37d7e15d515d067847'
        'c81b2bc9827461d9075989533f02442b0fb73df3dc1ec6816e46ef2ff9280cd9414e7fac26bcdd3955df6cd3833ed786558344e7b30925a444b4a23e67719dbe')

prepare() {
  cd "dwm-$pkgver"
  local p
  for p in "${_patches[@]}"; do
    patch -Np1 -i "$srcdir/${p##*/}"
  done
  cp "$srcdir/config.h" "$srcdir/shift-tools-scratchpads.c" .
  echo "CPPFLAGS+=${CPPFLAGS}" >> config.mk
  echo "CFLAGS+=${CFLAGS}" >> config.mk
  echo "LDFLAGS+=${LDFLAGS}" >> config.mk
}

build() {
  make -C "dwm-$pkgver" \
    X11INC=/usr/include/X11 \
    X11LIB=/usr/lib/X11 \
    FREETYPEINC=/usr/include/freetype2
}

package() {
  make -C "dwm-$pkgver" PREFIX=/usr DESTDIR="$pkgdir" install
  install -Dm644 "$srcdir/minilarbs.mom" "$pkgdir/usr/share/doc/$pkgname/minilarbs.mom"
  install -Dm644 "dwm-$pkgver/LICENSE" "$pkgdir/usr/share/licenses/$pkgname/LICENSE"
}
