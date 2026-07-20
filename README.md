# inkline

**Gesture-driven living ink.** You draw; a seeded noise field steals the stroke and keeps drawing without you.

**[Live demo →](https://godinhofonsec.github.io/inkline/)**

## The idea

Most generative art asks you to watch. inkline asks you to draw, then lets go of your hand.

Every stroke you make spawns ink particles that inherit the speed and direction of your gesture. Frame by frame, a flow field derived from a reproducible seed takes over: your line bends into its currents, frays, and finishes itself somewhere you did not plan. The field is reproducible; your hand is not. Every drawing is an unrepeatable collaboration between control and current.

## How to use

Draw with your mouse or finger (touch works). Then shape the collaboration:

| Control | What it does |
| --- | --- |
| `seed` | Regenerates the flow field. Same seed, same currents. |
| `accent` | Share of strokes in GØDN orange `#d94f2b` (default 15%). |
| `flow` | Strength of the field's pull on your ink. |
| `grip` | How long your gesture keeps control before the field takes it. |
| `clear` | Fresh canvas. |
| `save png` | Downloads the current drawing. |

## Built with

Vanilla JavaScript and a 2D canvas. No libraries, no build step, one file. Seeded randomness via mulberry32, flow field via seeded value-noise fBm.

## Related

Sibling project: [flowfield-studio](https://github.com/godinhofonsec/flowfield-studio), where the algorithm draws alone and you watch. inkline inverts it: here the algorithm only draws with you.

---

A GØDN experiment in flow, by [Bruno Godinho Fonseca](https://github.com/godinhofonsec).
