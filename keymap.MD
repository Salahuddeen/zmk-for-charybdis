# Charybdis ZMK Keymap

This file mirrors the current key definitions in `config/charybdis.keymap`.

## Legend
- `trans`: transparent (falls through)
- `none`: no action
- `mt MOD KEY`: mod-tap
- `lt LAYER KEY`: layer-tap (hold = layer, tap = key)

## Layer index
- `0` Base (Colemak-DH)
- `1` Extra
- `2` Tap
- `3` Button (includes Bluetooth controls)
- `4` Nav
- `5` Mouse
- `6` Media
- `7` Num
- `8` Sym
- `9` Fun

## Layer 0 (Base)
```text
R0: ESC  N1  N2  N3  N4  N5  N6  N7  N8  N9  N0  BSPC
R1: TAB  Q   W   F   P   B   J   L   U   Y   SQT BSLH
R2: LSFT mt(LGUI,A) mt(LALT,R) mt(LCTRL,S) mt(LSHFT,T) G  M  mt(RSHFT,N) mt(RCTRL,E) mt(RALT,I) mt(RGUI,O) SQT
R3: lt(3,Z) mt(RALT,X) C D V B K H COMMA mt(RALT,DOT) lt(3,SLASH) MINUS
T : LEFT_WIN  lt(4,SPACE)  lt(5,TAB)  lt(7,ENTER)  GRAVE
M : MB1 MB2 ENTER
Trackball: tmv_coarse
```

## Layer 1 (Extra)
```text
R0: trans ... trans
R1: trans Q W E R T Y U I O P trans
R2: trans mt(LGUI,A) mt(LALT,S) mt(LCTRL,D) mt(LSHFT,F) G H mt(RSHFT,J) mt(RCTRL,K) mt(RALT,L) mt(RGUI,SEMI) trans
R3: trans lt(3,Z) mt(RALT,X) C V B N M COMMA mt(RALT,DOT) lt(3,SLASH) trans
T : trans trans trans trans trans
M : trans trans trans
Trackball: tsl
```

## Layer 2 (Tap)
```text
R0: trans ... trans
R1: trans Q W F P B J L U Y SQT trans
R2: trans A R S T G M N E I O trans
R3: trans Z X C D V K H COMMA DOT SLASH trans
T : trans trans trans trans trans
M : trans trans trans
Trackball: tsl
```

## Layer 3 (Button)
```text
R0: trans ... trans
R1: trans none none none none none none none none none none trans
R2: trans LGUI LALT LCTRL LSHFT none LEFT DOWN UP RIGHT none trans
R3: trans none RALT mo(8) mo(7) BT_CLR BT_SEL0 BT_SEL1 BT_SEL2 BT_SEL3 BT_NXT trans
T : trans trans trans trans trans
M : trans trans trans
Trackball: tsl
```

## Layer 4 (Nav)
```text
R0: trans ... trans
R1: trans LGUI LALT LCTRL LSHFT none LEFT DOWN UP RIGHT CAPS trans
R2: trans none RALT mo(7) mo(4) none HOME PG_DN PG_UP END INS trans
R3: trans none none none none none ENTER BSPC DEL none none trans
T : trans trans trans trans trans
M : trans trans trans
Trackball: tsl
```

## Layer 5 (Mouse)
```text
R0: trans ... trans
R1: trans none none none none none MS_LEFT MS_DOWN MS_UP MS_RIGHT none trans
R2: trans LGUI LALT LCTRL LSHFT none C_PREV C_VOL_DN C_VOL_UP C_NEXT none trans
R3: trans none RALT mo(8) mo(5) none WH_LEFT WH_DOWN WH_UP WH_RIGHT none trans
T : trans trans trans trans trans
M : trans trans trans
Trackball: tsl
```

## Layer 6 (Media)
```text
R0: trans ... trans
R1: trans LGUI LALT LCTRL LSHFT none C_PREV C_VOL_DN C_VOL_UP C_NEXT none trans
R2: trans none RALT mo(9) mo(6) none C_STOP C_PP C_MUTE none none trans
R3: trans none none none none none none none none none none trans
T : trans trans trans trans trans
M : trans trans trans
Trackball: tsl
```

## Layer 7 (Num)
```text
R0: trans ... trans
R1: trans GRAVE N1 N2 N3 BSLH LBKT N7 N8 N9 RBKT trans
R2: trans LGUI LALT LCTRL LSHFT none EQUAL N4 N5 N6 SEMI trans
R3: trans none RALT mo(4) mo(7) none BSLH N1 N2 N3 GRAVE trans
T : trans trans trans trans trans
M : trans trans trans
Trackball: tsl
```

## Layer 8 (Sym)
```text
R0: trans ... trans
R1: trans LBKT AMPS STAR LPAR RBKT UNDER LPAR RPAR MINUS PLUS trans
R2: trans LGUI LALT LCTRL LSHFT none PLUS DLLR PRCNT CARET COLON trans
R3: trans none RALT mo(9) mo(8) none PIPE EXCL AT HASH TILDE trans
T : trans trans trans trans trans
M : trans trans trans
Trackball: tsl
```

## Layer 9 (Fun)
```text
R0: trans ... trans
R1: trans F12 F7 F8 F9 PSCRN C_PREV C_VOL_DN C_VOL_UP C_NEXT F10 trans
R2: trans LGUI LALT LCTRL LSHFT none C_STOP C_PP C_MUTE PAUSE_BREAK F11 trans
R3: trans none RALT mo(8) mo(9) none TAB SPACE K_APP none none trans
T : trans trans trans trans trans
M : trans trans trans
Trackball: tsl
```

## Notes
- Extra/non-core keys are transparent on non-base layers.
- Bluetooth controls are on Layer 3 (Button layer).
