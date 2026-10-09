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
        '73d6ed25f43b8a5a0c9db5694aa664f5c14889085dfcdc3da586729cc37c962b44fbc65968d0c0ed631cebb05cc77dbab3dd6af7d02f4b13bdf02287d1946e71'
        '2a76214671407b455b6fefc96f7de1ec88674dbea0b9fbd72967783e2e4c8913193b2cdd70185a18d61fa959c284f086f9bebfb838ffe37f51a45eae617a1453'
        'b72d1da3d3eea3b22ca0553167e6269e6ea84efd162a0966677e2a1db5defa0273acd9f504b1fb0483458f0e0c1f51d4fe01e37daaba484f5c623f63d752bda3'
        '96a0359fb100a80ede1e1233d6213eedf54e1708dc3ad9e3f8354ea922fa5810cc129975059831bde4cd7225a3534a6047befe6f0c00fd069c45891530a1118d'
        '9a957e5e487270d3830cb05cd05b59381d97d32a44febf1c0a67460e895e2a6e0889c202f365dcd4108f9b2a7e2223ea280f7931819b01abb932cf5bd46fa190'
        'e27ac6f96755588e2c4aefeafaeffd1017a23284505af5ab38e13fd930510c08a9d9e92409f9f0298f8bd696d77c921a9615a8663a25fec78f2e1bcc5da4de33'
        'e3104d5069d3766a5c456295d5ef3ec0c8ff6d05ffe9799616e70fff8bac5da559fbf57a93c99795324b48f9cbe74cc4613e53ef2707237b35817d323ed2deb8'
        'fa261dd11bf88fc7712c84490f68c66decb389ef23bb96d9fd8290b008eaac13eba7f2dccc663f2aa925b9100379843e054b87b58bc29423bc9db6bc47541c96'
        '2da73e90f8401131125d8508272ff6a5e911b3ba1a055461967d74f153533792940931dedfb5485fa5821ad2beea019fdfd3728362bdafbd3678672f43fe3286'
        '80a9a232a309ac39ceb5dd080af69759f81f394e4fe785d1cc2586e1c7a30ac2ca9af400e744cba4e5d23d8db9d20f109c0f0e9fe6732f352baf2f99f6dc5284'
        '63303bee8b0588feeba3e5316cc5276f42535e432ce076c0edf123b551e24c2c21b943507f7175d93625863312e846baf63bb58966e3e7dd633625eba7c0e5c2'
        '67a04475867ea2707efff0d76d4fffe03a61d8cddbba5511eb107dc141459fd70d6050dab6878db5e864b9670e75a9492f49647cd0a13d89bfd49b2dbfaccc5d')

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
