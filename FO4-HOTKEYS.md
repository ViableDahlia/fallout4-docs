# Fallout 4 Hotkey Reference

A reference for default Fallout 4 PC keybindings alongside hotkeys added by
[Place Everywhere](https://www.nexusmods.com/fallout4/mods/9424) and
[FO4 Hotkeys](https://www.nexusmods.com/fallout4/mods/11664).

> **PC only.** Place Everywhere and FO4 Hotkeys are F4SE plugins — console platforms are not supported.

---

## ⚠️ Known conflict: F2 and F3

FO4 Hotkeys ships with F2 (toggle menus) and F3 (toggle flycam) bound by default.
Place Everywhere uses F2 (ground snapping) and F3 (grid snapping) in Workshop mode.

**Fix:** remap either mod. In FO4 Hotkeys, edit `Data\Hotkeys.ini`. In Place Everywhere, edit `Data\F4SE\Plugins\place.ini`.

---

## Default Fallout 4 keys

### Movement

| Action | Key |
|---|---|
| Move forward | `W` |
| Move backward | `S` |
| Strafe left | `A` |
| Strafe right | `D` |
| Sprint | `Left Shift` |
| Jump | `Space` |
| Sneak / crouch | `Ctrl` |
| Toggle walk / run | `Caps Lock` |
| Look around | `Mouse` |

### Combat

| Action | Key |
|---|---|
| Attack / fire | `Left Mouse` |
| Aim (iron sights) | `Right Mouse` |
| Reload | `R` |
| Melee attack | `V` |
| Block / bash | `Right Mouse` |
| Grenade / mine | `G` |
| Switch ammo type | `B` |
| VATS | `Q` |
| Favorite items | `1` – `8` |

### Pip-Boy

| Action | Key |
|---|---|
| Open Pip-Boy | `Tab` |
| Toggle Pip-Boy light | `Q` (held) |
| Open map tab | `M` |
| Open quests / radio | `N` |

### UI & menus

| Action | Key |
|---|---|
| Open / close menu | `Esc` |
| Accept / interact | `E` |
| Cancel / back | `Esc` / `C` |
| Inspect item | `F` |
| Rotate item in inventory | `Hold E` + mouse |
| Drop item | `R` |

### Settlement / Workshop

| Action | Key |
|---|---|
| Open workshop mode | `V` |
| Build / confirm | `E` |
| Rotate object | `Mouse scroll` / `Q` / `E` |
| Grab / move object | `G` |
| Scrap item | `R` |
| Store item | `R` |
| Toggle snap | `X` |
| Exit workshop | `Esc` / `V` |

### Misc

| Action | Key |
|---|---|
| Quick save | `F5` *(disabled in Workshop mode)* |
| Quick load | `F9` |
| Screenshot | `PrtScn` / `F12` |
| Wait | `T` |
| Open console | `` ` `` (tilde) |

---

## Place Everywhere

[Nexus page](https://www.nexusmods.com/fallout4/mods/9424) · by TheLich · requires F4SE

> All hotkeys below are **Workshop mode only**. All are configurable in `Data\F4SE\Plugins\place.ini`.

### Toggles

| Action | Key |
|---|---|
| Toggle Place Everywhere mode | `F8` *(requires toggle mode enabled in place.ini)* |
| Toggle object snapping | `F1` *(cancel current selection first)* |
| Toggle ground & surface snapping | `F2` ⚠️ *conflicts with FO4 Hotkeys default* |
| Toggle workshop grid snapping | `F3` ⚠️ *conflicts with FO4 Hotkeys default* |
| Toggle out-of-workshop timeout | `F5` *(Quick Save is disabled in Workshop mode — no real conflict)* |
| Toggle store clamped objects on scrap | `F6` |
| Lock / unlock highlighted object | `F7` |
| Toggle extra objects selection | `Ins` |
| Change timescale to 0.01 in build mode | `F11` *(value configurable in place.ini)* |

### Precise movement

| Action | Key |
|---|---|
| Set movement axis: player or world | `Alt` |
| Move object up | `Numpad 8` |
| Move object down | `Numpad 2` |
| Move object left | `Numpad 4` |
| Move object right | `Numpad 6` |
| Move object toward player | `Numpad 7` |
| Move object away from player | `Numpad 9` |
| Increase movement step | `Numpad *` |
| Decrease movement step | `Numpad /` |
| Undo last precise action | `Backspace` *(up to 10 actions)* |

### Rotation

| Action | Key |
|---|---|
| Change rotation axis (X / Y / Z) | `Ctrl` |
| Reset X & Y rotation to 0 | `Numpad 0` |
| Remove tremor effect | `Numpad 5` |
| Increase rotation angle step | `Numpad +` |
| Decrease rotation angle step | `Numpad -` |

### Scale

| Action | Key |
|---|---|
| Scale object up 10% | `Numpad 3` |
| Scale object down 10% | `Numpad 1` |
| Reset scale to 100% | `Numpad .` |
| Increase scale step | `PgUp` |
| Decrease scale step | `PgDn` |

### Store / apply transform info

Store an object's position, rotation, and scale, then apply any combination to another object.

| Action | Key |
|---|---|
| Store object position, rotation & scale | `=` |
| Apply stored X position | `1` |
| Apply stored Y position | `2` |
| Apply stored Z position | `3` |
| Apply stored X rotation | `4` |
| Apply stored Y rotation | `5` |
| Apply stored Z rotation | `6` |
| Apply stored scale | `7` |
| Apply all stored info | `0` |

### Physics

| Action | Key |
|---|---|
| Turn object physics on (movable) | `Home` |
| Turn object physics off (static) | `End` |

---

## FO4 Hotkeys

[Nexus page](https://www.nexusmods.com/fallout4/mods/11664) · by registrator2000 · requires F4SE

A scripting framework that enables hotkeying of equipment, items, and console commands.
All bindings are fully configurable in `Data\Hotkeys.ini` or via the in-game console command `hotkey`.

> Default bindings shown. These apply globally (not just in Workshop mode).

### Default bindings (out of the box)

| Action | Key | Notes |
|---|---|---|
| Toggle menu visibility | `F2` | ⚠️ conflicts with Place Everywhere (ground snapping) |
| Toggle free-fly camera | `F3` | ⚠️ conflicts with Place Everywhere (grid snapping) |
| Hotkey slot 1 | `Z` | Full version only |
| Hotkey slot 2 | `G` | Full version only |
| Hotkey slot 3 | `B` | Full version only |
| Hotkey slot 4 | `Y` | Full version only |
| Hotkey slot 5 | `H` | Full version only |
| Hotkey slot 6 | `N` | Full version only |
| Hotkey slot 7 | `U` | Full version only |
| Hotkey slots 1–10 | `Shift-1` … `Shift-10` | All versions |

### Assigning hotkeys via console

```
hotkey <key> <function>
```

Examples:

```
hotkey F2 tfc          ; bind F2 to toggle flycam
hotkey B tm            ; bind B to toggle menus
hotkey Shift-1 tgm     ; bind Shift-1 to god mode
hotkey Z hot 1         ; bind Z to Hotkey Manager slot 1
hotkey F2              ; unbind F2
```

---

*Maintained by [Viable Dahlia](https://www.nexusmods.com/profile/viabledahlia) · [commonwealth-tools](https://github.com/ViableDahlia/commonwealth-tools) · CC BY 4.0*
