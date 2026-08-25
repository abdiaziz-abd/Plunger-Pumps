# Plunger Pumps

An interactive single-page reference on reciprocating plunger pumps — how a plunger
gallery works, why "high pressure pump" is a misnomer, how staggered plungers smooth
the output flow, and what separates the power end from the fluid end.

By Abdiaziz Abdi — Cyprus International University, Cyprus.

## What's in it

- Seven technical figures covering the bottle-jack analogy, downstream pressure,
  staggered crankshaft throws, combined flow, the two zones, and a gallery section
- Three interactive animations — a single gallery, a triplex, and a quintuplex —
  each with an RPM slider that drives the crankshaft
- A simplified kinematic schematic built from scratch: slider-crank geometry with
  suction and discharge valves that open and close with stroke direction

## Running it

Open `index.html` in a browser, or serve the folder:

```
npx http-server . -p 8231
```

The animations are frame-embedded scenes that negotiate a `MessageChannel` with the
host page before they render. `index.html` answers that handshake and supplies the
viewport height they size themselves from — without it they compute a `NaN` layout
and never draw their controls.

## Credits

Lesson text, the figures, and the three animation scenes come from the public preview
of the **Plunger Pumps** lesson in the Oilfield Pumping session at
[LunchBox Sessions](https://www.lunchboxsessions.com/materials/oilfield-pumping/plunger-pumps-lesson),
by CD Industrial Group Inc. All rights to that material remain theirs. This repository
is a study project; for the complete lesson, visit the source.

The layout, typography, and the kinematic schematic are original work.
