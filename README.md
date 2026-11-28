# M901CY Custom Input Module · Renaissance

Ward-Beck Systems M901CY, 1994|27. Wiki page: [M901CY on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/PAGES/M901CY.html)

| Folder | What is in it | Files |
|---|---|---|
| [MECHANICAL/](MECHANICAL/) | front panels, cover plates, metalwork, assemblies; the front panel as vectors | 11 |
| [PINOUTS/](PINOUTS/) | the RTO-144 connector: connection sheets, connector layouts, rear views | 7 |
| [KICAD/](KICAD/) | KiCad schematics traced from the drawings, the symbol, PCB projects | 1 |
| [OCR/](OCR/) | the note of every file: date, origin, title block, OCR text | 3 |

## Mechanical

_Mechanical drawings: front panels, cover plates, metalwork and hardware (-03- drawings), AutoCAD files, each with its `(EXTRACTED).svg` vectors; `<module> - front panel.svg` is the front panel as vectors._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/1fxNifDaEAo6yz_d8UIFdgU6chodkYLIH/view" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=1fxNifDaEAo6yz_d8UIFdgU6chodkYLIH" width="240" alt="1994 - M901CY - DOC - 940444-03-006 - LOVG FULL RAD SLOT SEE NOTE DOR ENTATIONS.jpg"></a><br><sub>1994|27 · DOC - 940444-03-006 - LOVG FULL RAD SLOT SEE NOTE DOR ENTATIONS · <a href="MECHANICAL/1994%20-%20M901CY%20-%20DOC%20-%20940444-03-006%20-%20LOVG%20FULL%20RAD%20SLOT%20SEE%20NOTE%20DOR%20ENTATIONS%20(EXTRACTED).svg">vectors</a></sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/1a-jMm01y8d49S80PxNkauj9pp0yz5NYI/view" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=1a-jMm01y8d49S80PxNkauj9pp0yz5NYI" width="240" alt="1994 - M901CY - DOC - 940444-04-001 - OTHERS ELECTRICALLY AND MECHANICALLY INTEGRATED INTO CONSOLE.jpg"></a><br><sub>1994|27 · DOC - 940444-04-001 - OTHERS ELECTRICALLY AND MECHANICALLY INTEGRATED INTO CONSOLE · <a href="MECHANICAL/1994%20-%20M901CY%20-%20DOC%20-%20940444-04-001%20-%20OTHERS%20ELECTRICALLY%20AND%20MECHANICALLY%20INTEGRATED%20INTO%20CONSOLE%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## 3-D model

[`MECHANICAL/M901CY.stl`](MECHANICAL/M901CY.stl) (GitHub turns it in 3-D) · [view, change and generate it on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/2026/stl.html?m=M901CY)

- **Size:** 41 × 404.7 mm panel, 165 mm deep, 3.2 mm plate (assumed 41 mm wide (1.6"), the drawn panel's proportions)
- **From the drawing:** 16 holes and cut-outs, 0 knobs (front panel: `MECHANICAL/M901CY - front panel.svg`)
- Made by `tools/module_models.py` (→ `MECHANICAL/M901CY.model.json`) and `tools/stl/make_stl.mjs` in [WBSps.ca](https://github.com/WardBeckSystems/WBSps.ca); the site makes the same STL from the same JSON.

## Pinouts

_Pinouts: the RTO-144 edge connector (connection sheets, connector layouts and rear views, strapping), and the pinout / connections drawings made from them. The module root `RTO.json` lists every contact._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKajBJRlJrME1vWVE/view?resourcekey=0-iQmWJ3V71qU67Qr1oocbtQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKajBJRlJrME1vWVE&resourcekey=0-iQmWJ3V71qU67Qr1oocbtQ" width="240" alt="1994 - M901CY - CONNECTOR LAYOUT.jpg"></a><br><sub>1994|27 · CONNECTOR LAYOUT · <a href="PINOUTS/1994%20-%20M901CY%20-%20CONNECTOR%20LAYOUT%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## RTO-144 pinout

Read from 1 pinout picture (each its own `.pinout.json` beside it). Every contact, with where it was read: [`RTO.json`](RTO.json). How a picture becomes this table: [the pinout decision tree](https://github.com/WardBeckSystems/WBSps.ca/blob/main/2026/Engineering/PINOUTS.md).

**To check:**

- polarity assumed: 21 contacts given + / − that the drawing does not mark (e.g. P1-2 PGM 1 MUSIC OUT LEFT) (M901CY: 1994 - M901CY - CONNECTOR LAYOUT.jpg)

**Inserts:** INSERT L: INSERT L SEND → INSERT L RETURN · INSERT R: INSERT R SEND → INSERT R RETURN

| Pin | Signal | Kind | Port | Confidence |
|---|---|---|---|---|
| P1-1 | 24V COM | ground |  | high |
| P1-2 | PGM 1 MUSIC OUT LEFT | out | PGM 1 MUSIC OUT LEFT + | high |
| P1-3 | 24V COM | ground |  | high |
| P1-4 | PGM 1 VOICE OUT LEFT | out | PGM 1 VOICE OUT LEFT + | high |
| P1-5 | 24V COM | ground |  | high |
| P1-6 | PGM 1 MUSIC OUT RIGHT | out | PGM 1 MUSIC OUT RIGHT + | high |
| P1-7 | 24V COM | ground |  | high |
| P1-8 | PGM 1 VOICE OUT RIGHT | out | PGM 1 VOICE OUT RIGHT + | high |
| P1-9 | 24V COM | ground |  | high |
| P1-10 | PGM 2 OUT LEFT | out | PGM 2 OUT LEFT + | high |
| P1-11 | 24V COM | ground |  | high |
| P1-12 | PGM 2 OUT RIGHT | out | PGM 2 OUT RIGHT + | high |
| P1-13 | 24V COM | ground |  | high |
| P1-14 | PGM 3 OUT LEFT | out | PGM 3 OUT LEFT + | high |
| P1-15 | 24V COM | ground |  | high |
| P1-16 | PGM 3 OUT RIGHT | out | PGM 3 OUT RIGHT + | high |
| P1-17 | 24V COM | ground |  | high |
| P1-18 | PGM 4 OUT LEFT | out | PGM 4 OUT LEFT + | high |
| P1-19 | 24V COM | ground |  | high |
| P1-20 | PGM 4 OUT RIGHT | out | PGM 4 OUT RIGHT + | high |
| P1-21 | 24V COM | ground |  | high |
| P1-22 | MIX-MINUS OUT | out | MIX-MINUS OUT + | high |
| P1-23 | 24V COM | ground |  | high |
| P1-24 | N/C | nc |  | high |
| P1-25 | 24V COM | ground |  | high |
| P1-26 | N/C | nc |  | high |
| P1-27 | 24V COM | ground |  | high |
| P1-28 | N/C | nc |  | high |
| P1-29 | 24V COM | ground |  | high |
| P1-30 | AUX 1 OUT | out | AUX 1 OUT + | high |
| P1-31 | 24V COM | ground |  | high |
| P1-32 | AUX 2 OUT LEFT | out | AUX 2 OUT LEFT + | high |
| P1-33 | 24V COM | ground |  | high |
| P1-34 | AUX 2 OUT RIGHT | out | AUX 2 OUT RIGHT + | high |
| P1-35 | 24V COM | ground |  | high |
| P1-36 | CUE OUT LEFT | out | CUE OUT LEFT + | high |
| P1-37 | 24V COM | ground |  | high |
| P1-38 | CUE OUT RIGHT | out | CUE OUT RIGHT + | high |
| P1-39 | 24V COM | ground |  | high |
| P1-40 | 24V COM | ground |  | high |
| P2-1 | A INPUT L + | in | A INPUT L + | high |
| P2-2 | A INPUT L - | in | A INPUT L - | high |
| P2-3 | A INPUT R + | in | A INPUT R + | high |
| P2-4 | A INPUT R - | in | A INPUT R - | high |
| P2-5 | B INPUT L + | in | B INPUT L + | high |
| P2-6 | B INPUT L - | in | B INPUT L - | high |
| P2-7 | B INPUT R + | in | B INPUT R + | high |
| P2-8 | B INPUT R - | in | B INPUT R - | high |
| P2-9 | INPUT SHIELD | shield | shield | high |
| P2-10 | INPUT SHIELD | shield | shield | high |
| P2-11 | INSERT R SEND | insert_send | INSERT R SEND + | high |
| P2-12 | INSERT L SEND | insert_send | INSERT L SEND + | high |
| P2-13 | INSERT R RETURN | insert_return | INSERT R RETURN + | high |
| P2-14 | INSERT L RETURN | insert_return | INSERT L RETURN + | high |
| P2-15 | DIRECT OUT R | out | DIRECT OUT R + | high |
| P2-16 | DIRECT OUT L | out | DIRECT OUT L + | high |
| P2-17 | P2-CTL OUT | control_out | P2-CTL OUT | high |
| P2-18 | P1-CTL OUT | control_out | P1-CTL OUT | high |
| P2-19 | EXT. VCA CTL VOLTAGE | control_in | EXT. VCA CTL VOLTAGE | high |
| P2-20 | N/C | nc |  | high |
| P2-21 | PGM 2 EXTERNAL SELECT | control_in | PGM 2 EXTERNAL SELECT | high |
| P2-22 | PGM 1 EXTERNAL SELECT | control_in | PGM 1 EXTERNAL SELECT | high |
| P2-23 | CUE CTL BUS | bus | CUE CTL BUS | high |
| P2-24 | CUE CTL BUS | bus | CUE CTL BUS | high |
| P2-25 | EXTERNAL B SELECT | control_in | EXTERNAL B SELECT | high |
| P2-26 | EXTERNAL A SELECT | control_in | EXTERNAL A SELECT | high |
| P2-27 | TIMER RESET BUS | bus | TIMER RESET BUS | high |
| P2-28 | TIMER RESET BUS | bus | TIMER RESET BUS | high |
| P2-29 | MUTE BUS A | bus | MUTE BUS A | high |
| P2-30 | MUTE BUS A | bus | MUTE BUS A | high |
| P2-31 | MUTE BUS B | bus | MUTE BUS B | high |
| P2-32 | MUTE BUS B | bus | MUTE BUS B | high |
| P2-33 | MUTE BUS C | bus | MUTE BUS C | high |
| P2-34 | MUTE BUS C | bus | MUTE BUS C | high |
| P2-35 | B STOP | control_out | B STOP | high |
| P2-36 | A STOP | control_out | A STOP | high |
| P2-37 | B START | control_out | B START | high |
| P2-38 | A START | control_out | A START | high |
| P2-39 | B ON TALLY | control_out | B ON TALLY | high |
| P2-40 | A ON TALLY | control_out | A ON TALLY | high |
| P2-41 | CUE CTL | control_in | CUE CTL | high |
| P2-42 | PGM SELECT RESET | control_in | PGM SELECT RESET | high |
| P2-43 | ON CTL | control_in | ON CTL | high |
| P2-44 | OFF CTL | control_in | OFF CTL | high |
| P2-45 | OFF TALLY | control_out | OFF TALLY | high |
| P2-46 | OFF TALLY | control_out | OFF TALLY | high |
| P2-47 | CTL COM | ground |  | high |
| P2-48 | CTL COM | ground |  | high |
| P2-49 | -24 V | power |  | high |
| P2-50 | -24 V | power |  | high |
| P2-51 | 24V COMMON | ground |  | high |
| P2-52 | 24V COMMON | ground |  | high |
| P2-53 | +24 V | power |  | high |
| P2-54 | +24 V | power |  | high |
| P2-55 | CHASSIS | ground |  | high |
| P2-56 | CHASSIS | ground |  | high |

## KiCad

_KiCad: a schematic (`.kicad_sch`) traced from each electrical drawing, the module symbol (`.kicad_sym`) and its PCB projects. Traced schematics are the line work only: redraw with symbols over them._

- [M901CY.kicad_sym](KICAD/M901CY.kicad_sym)

---
Archive: Anthony Peter Kuzub · [WBSps.ca](https://WBSps.ca) · [WBSps.Kuzub.com](https://WBSps.Kuzub.com)
