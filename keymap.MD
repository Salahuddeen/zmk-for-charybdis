# Charybdis ZMK Keymap (Miryoku 3x5 Core Match)

Reference generated from `config/charybdis.keymap`.

## Core conventions
- 3x5 core per hand matches Miryoku layer roles.
- Thumb taps match Miryoku: left `Esc/Space/Tab`, right `Enter/Backspace/Delete`.
- Non-core Charybdis keys remain as configured in the keymap.

## Layer map
- `0` Base (Colemak-DH)
- `1` Extra
- `2` Tap
- `3` Button
- `4` Nav
- `5` Mouse
- `6` Media
- `7` Num
- `8` Sym
- `9` Fun

## Layer 0 Base core
Top: `Q W F P B` | `J L U Y SQT`
Home: `mt(LGUI,A) mt(LALT,R) mt(LCTRL,S) mt(LSHFT,T) G` | `M mt(RSHFT,N) mt(RCTRL,E) mt(RALT,I) mt(RGUI,O)`
Bottom: `lt(3,Z) mt(RALT,X) C D V` | `K H COMMA mt(RALT,DOT) lt(3,SLASH)`
Thumb taps: `Esc Space Tab` | `Enter Backspace Delete`

## Layer 1 Extra core
Top: `Q W E R T` | `Y U I O P`
Home: `mt(LGUI,A) mt(LALT,S) mt(LCTRL,D) mt(LSHFT,F) G` | `H mt(RSHFT,J) mt(RCTRL,K) mt(RALT,L) mt(RGUI,SQT)`
Bottom: `lt(3,Z) mt(RALT,X) C V B` | `N M COMMA mt(RALT,DOT) lt(3,SLASH)`

## Layer 2 Tap core
Top: `Q W F P B` | `J L U Y SQT`
Home: `A R S T G` | `M N E I O`
Bottom: `Z X C D V` | `K H COMMA DOT SLASH`

## Layer 3 Button core
Top: `LS(DEL) LC(INS) LS(INS) none none` | `none LS(INS) LC(INS) LS(DEL) none`
Home: `LGUI LALT LCTRL LSHFT none` | `none LSHFT LCTRL LALT LGUI`
Bottom: `none LS(DEL) LC(INS) LS(INS) none` | `none LS(INS) LC(INS) LS(DEL) none`

## Layer 4 Nav core
Top: `bootloader to(2) to(1) to(0) none` | `LC(Y) LC(V) LC(C) LC(X) LC(Z)`
Home: `LGUI LALT LCTRL LSHFT none` | `caps_word LEFT DOWN UP RIGHT`
Bottom: `none RALT to(7) to(4) none` | `INS HOME PG_DN PG_UP END`

## Layer 5 Mouse core
Top: `bootloader to(2) to(1) to(0) none` | `LC(Y) LC(V) LC(C) LC(X) LC(Z)`
Home: `LGUI LALT LCTRL LSHFT none` | `none LEFT DOWN UP RIGHT`
Bottom: `none RALT to(8) to(5) none` | `none none PG_DN PG_UP none`

## Layer 6 Media core
Top: `bootloader to(2) to(1) to(0) none` | `none none none none none`
Home: `LGUI LALT LCTRL LSHFT none` | `none C_PREV C_VOL_DN C_VOL_UP C_NEXT`
Bottom: `none RALT to(9) to(6) none` | `none none none none none`

## Layer 7 Num core
Top: `LEFT_BRACKET N7 N8 N9 RIGHT_BRACKET` | `none to(0) to(1) to(2) bootloader`
Home: `SEMI N4 N5 N6 EQUAL` | `none LSHFT LCTRL LALT LGUI`
Bottom: `GRAVE N1 N2 N3 BSLH` | `none to(7) to(4) RALT none`

## Layer 8 Sym core
Top: `LS(LEFT_BRACKET) AMPS STAR LPAR LS(RIGHT_BRACKET)` | `none to(0) to(1) to(2) bootloader`
Home: `LS(SEMI) DLLR PRCNT CARET PLUS` | `none LSHFT LCTRL LALT LGUI`
Bottom: `TILDE EXCL AT HASH PIPE` | `none to(8) to(5) RALT none`

## Layer 9 Fun core
Top: `F12 F7 F8 F9 PSCRN` | `none to(0) to(1) to(2) bootloader`
Home: `F11 F4 F5 F6 none` | `none LSHFT LCTRL LALT LGUI`
Bottom: `F10 F1 F2 F3 PAUSE_BREAK` | `none to(9) to(6) RALT none`

## Trackball
- Layer `0`: `tmv_coarse`
- Layers `1-9`: `tsl`
