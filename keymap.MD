# Charybdis ZMK Keymap

This file documents the current keymap from `config/charybdis.keymap`.

## Legend
- `trans`: transparent (falls through to lower layer)
- `none`: no action
- `mt MOD KEY`: mod-tap (hold = modifier, tap = key)
- `mo N`: momentary layer switch to layer `N` while held

## Quick cheat sheet
- **BT layer:** hold key left of `Z` (`mo 2`)
- **Nav hub:** hold thumb `mo 1`
- **From Nav hub:** hold `mo 3` = Num, hold `mo 4` = Sym, hold `mo 5` = Fun
- **Home-row mods (base):**
	- Left hand: `A=GUI`, `S=ALT`, `D=CTRL`, `F=SHIFT` (hold)
	- Right hand: `J=SHIFT`, `K=CTRL`, `L=ALT`, `;=GUI` (hold)
- **Bluetooth keys (Layer 2):**
	- `BT_SEL 0/1/2/3` on left home cluster
	- `BT_NXT` on left row key next to selectors
	- `BT_CLR` on left bottom-row inner key
- **Trackball:** base uses `tmv_coarse`; non-base layers use `tsl`

---

## Layer 0 (Base)

### Main matrix (4 rows × 12 cols)
| Row | C0 | C1 | C2 | C3 | C4 | C5 | C6 | C7 | C8 | C9 | C10 | C11 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R0 | ESC | N1 | N2 | N3 | N4 | N5 | N6 | N7 | N8 | N9 | N0 | BACKSPACE |
| R1 | TAB | Q | W | E | R | T | Y | U | I | O | P | BSLH |
| R2 | LEFT_SHIFT | `mt LGUI A` | `mt LALT S` | `mt LCTRL D` | `mt LSHFT F` | G | H | `mt RSHFT J` | `mt RCTRL K` | `mt RALT L` | `mt RGUI SEMI` | SQT |
| R3 | `mo 2` | Z | X | C | V | B | N | M | COMMA | LEFT_BRACKET | FSLH | MINUS |

### Thumb / extra cluster
- Row 4: LEFT_WIN, SPACE, `mo 1`, LALT, GRAVE
- Row 5: MB1, MB2, ENTER

### Trackball
- `trackball-bindings = <&tmv_coarse>`

---

## Layer 1 (Nav / Layer hub)

### Main matrix
| Row | C0 | C1 | C2 | C3 | C4 | C5 | C6 | C7 | C8 | C9 | C10 | C11 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R0 | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans |
| R1 | trans | LGUI | LALT | LCTRL | LSHFT | none | INS | HOME | UP | END | PG_UP | trans |
| R2 | trans | none | none | none | none | none | DEL | LEFT | DOWN | RIGHT | PG_DN | trans |
| R3 | trans | `mo 3` | `mo 4` | `mo 5` | none | none | none | none | none | none | none | trans |

### Thumb / extra cluster
- All `trans`

### Trackball
- `trackball-bindings = <&tsl>`

---

## Layer 2 (Bluetooth)

### Main matrix
| Row | C0 | C1 | C2 | C3 | C4 | C5 | C6 | C7 | C8 | C9 | C10 | C11 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R0 | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans |
| R1 | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans |
| R2 | trans | BT_SEL 0 | BT_SEL 1 | BT_SEL 2 | BT_SEL 3 | BT_NXT | trans | trans | trans | trans | trans | trans |
| R3 | trans | trans | trans | trans | trans | BT_CLR | trans | trans | trans | trans | trans | trans |

### Thumb / extra cluster
- All `trans`

### Trackball
- `trackball-bindings = <&tsl>`

---

## Layer 3 (Num)

### Main matrix
| Row | C0 | C1 | C2 | C3 | C4 | C5 | C6 | C7 | C8 | C9 | C10 | C11 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R0 | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans |
| R1 | trans | PLUS | N7 | N8 | N9 | none | N7 | N8 | N9 | PLUS | MINUS | trans |
| R2 | trans | MINUS | N4 | N5 | N6 | none | N4 | N5 | N6 | STAR | FSLH | trans |
| R3 | trans | STAR | N1 | N2 | N3 | none | N1 | N2 | N3 | N0 | PERIOD | trans |

### Thumb / extra cluster
- All `trans`

### Trackball
- `trackball-bindings = <&tsl>`

---

## Layer 4 (Sym)

### Main matrix
| Row | C0 | C1 | C2 | C3 | C4 | C5 | C6 | C7 | C8 | C9 | C10 | C11 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R0 | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans |
| R1 | trans | EXCL | AT | HASH | DLLR | none | AMPS | STAR | LPAR | RPAR | UNDER | trans |
| R2 | trans | GRAVE | BSLH | LEFT_BRACKET | RIGHT_BRACKET | none | CARET | PIPE | LEFT_BRACKET | RIGHT_BRACKET | TILDE | trans |
| R3 | trans | PERCENT | SQT | COMMA | PERIOD | none | PLUS | MINUS | EQUAL | FSLH | SEMI | trans |

### Thumb / extra cluster
- All `trans`

### Trackball
- `trackball-bindings = <&tsl>`

---

## Layer 5 (Fun)

### Main matrix
| Row | C0 | C1 | C2 | C3 | C4 | C5 | C6 | C7 | C8 | C9 | C10 | C11 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|
| R0 | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans | trans |
| R1 | trans | F1 | F2 | F3 | F4 | F5 | F6 | F7 | F8 | F9 | F10 | trans |
| R2 | trans | F11 | F12 | PSCRN | PAUSE_BREAK | none | none | none | none | none | none | trans |
| R3 | trans | none | none | none | none | none | none | none | none | none | none | trans |

### Thumb / extra cluster
- All `trans`

### Trackball
- `trackball-bindings = <&tsl>`

---

## Behavior summary
- Hold the key left of `Z` (`mo 2`) to access the Bluetooth layer.
- On Layer 1, hold `mo 3`, `mo 4`, or `mo 5` to access Num, Sym, or Fun layers.
- Extra keys are pass-through (`trans`) on non-base layers, so they keep base behavior.

---

## Compact physical view

The grids below are split as **Left (L0-L5)** and **Right (R0-R5)** for the 3x6 main area plus the extra left column.

### Layer 0 (Base)

```text
L: [ESC] [N1] [N2] [N3] [N4] [N5]    ||    [N6] [N7] [N8] [N9] [N0] [BSPC] :R
L: [TAB] [Q ] [W ] [E ] [R ] [T ]    ||    [Y ] [U ] [I ] [O ] [P ] [\   ] :R
L: [SFT] [A⌘] [S⎇] [D⌃] [F⇧] [G ]    ||    [H ] [J⇧] [K⌃] [L⎇] [;⌘] ['   ] :R
L: [BT ] [Z ] [X ] [C ] [V ] [B ]    ||    [N ] [M ] [, ] [[] [ / ] [ -  ] :R

Thumbs: [LWIN] [SPACE] [NAV] [LALT] [GRAVE]
Trackball keys: [MB1] [MB2] [ENTER]
```

### Layer 1 (Nav / Hub)

```text
L: [trn] [trn ] [trn ] [trn ] [trn ] [trn ] || [trn ] [trn ] [trn ] [trn ] [trn ] [trn ]
L: [trn] [LGUI] [LALT] [LCTL] [LSFT] [none] || [INS ] [HOME] [UP  ] [END ] [PGUP] [trn ]
L: [trn] [none] [none] [none] [none] [none] || [DEL ] [LEFT] [DOWN] [RGHT] [PGDN] [trn ]
L: [trn] [NUM ] [SYM ] [FUN ] [none] [none] || [none] [none] [none] [none] [none] [trn ]

Thumbs/extra: all transparent
```

### Layer 2 (Bluetooth)

```text
L: [trn] [trn ] [trn ] [trn ] [trn ] [trn ] || [trn ] [trn ] [trn ] [trn ] [trn ] [trn ]
L: [trn] [trn ] [trn ] [trn ] [trn ] [trn ] || [trn ] [trn ] [trn ] [trn ] [trn ] [trn ]
L: [trn] [BT0 ] [BT1 ] [BT2 ] [BT3 ] [NEXT] || [trn ] [trn ] [trn ] [trn ] [trn ] [trn ]
L: [trn] [trn ] [trn ] [trn ] [trn ] [CLR ] || [trn ] [trn ] [trn ] [trn ] [trn ] [trn ]

Thumbs/extra: all transparent
```

### Layer 3 (Num)

```text
L: [trn] [trn ] [trn] [trn] [trn] [trn] || [trn] [trn] [trn] [trn ] [trn ] [trn]
L: [trn] [+   ] [7  ] [8  ] [9  ] [none] || [7  ] [8  ] [9  ] [+   ] [-   ] [trn]
L: [trn] [-   ] [4  ] [5  ] [6  ] [none] || [4  ] [5  ] [6  ] [*   ] [/   ] [trn]
L: [trn] [*   ] [1  ] [2  ] [3  ] [none] || [1  ] [2  ] [3  ] [0   ] [.   ] [trn]

Thumbs/extra: all transparent
```

### Layer 4 (Sym)

```text
L: [trn] [trn] [trn] [trn] [trn] [trn] || [trn ] [trn ] [trn ] [trn ] [trn ] [trn]
L: [trn] [!  ] [@  ] [#  ] [$  ] [none] || [&   ] [*   ] [(   ] [)   ] [_   ] [trn]
L: [trn] [`  ] [\  ] [[  ] []  ] [none] || [^   ] [|   ] [[   ] []   ] [~   ] [trn]
L: [trn] [%  ] ['  ] [,  ] [.  ] [none] || [+   ] [-   ] [=   ] [/   ] [;   ] [trn]

Thumbs/extra: all transparent
```

### Layer 5 (Fun)

```text
L: [trn] [trn] [trn] [trn] [trn] [trn] || [trn ] [trn ] [trn ] [trn ] [trn ] [trn]
L: [trn] [F1 ] [F2 ] [F3 ] [F4 ] [F5 ] || [F6  ] [F7  ] [F8  ] [F9  ] [F10 ] [trn]
L: [trn] [F11] [F12] [PS ] [PAUS] [none] || [none] [none] [none] [none] [none] [trn]
L: [trn] [none] [none] [none] [none] [none] || [none] [none] [none] [none] [none] [trn]

Thumbs/extra: all transparent
```
