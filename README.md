# Watts-Cseh Electronics

Handmade guitar pedals built in California. We design boutique effects chasing the tones people have been hunting for decades — warm, organic, vintage sounds that modern gear stopped making.

Everything here is designed and assembled by hand. No shortcuts, no mass production.

---

## Products

### Treble Boost
A high-gain treble booster in the tradition of the classic British boost circuits. Built for that cutting, harmonically rich lead tone.

### Chorus
A lush analog chorus inspired by vintage bucket-brigade designs. Slow, warm, and musical.

---

## Repository Structure

```
Watts-Cseh-Electronics/
├── Treble-Boost/
│   ├── circuit/    ← LTspice schematics (.asc, .asy)
│   ├── board/      ← KiCad PCB project
│   ├── model/      ← Enclosure CAD exports (.step, .stl)
│   ├── art/        ← Faceplate graphics, decals, renders
│   └── docs/       ← BOM, assembly notes, datasheets
├── Chorus/
│   ├── circuit/
│   ├── board/
│   ├── model/
│   ├── art/
│   └── docs/
└── _shared/
    ├── kicad-libs/   ← Shared symbols & footprints
    ├── templates/    ← BOM and doc templates
    └── 3d-models/    ← Common hardware (jacks, pots, switches)
```

---

## Tools

- **Simulation** — LTspice
- **PCB** — KiCad
- **CAD** — Onshape (exports archived here as .step / .stl)
- **Version control** — Git + Git LFS for large binaries

## Contributing

Work on feature branches (`treble-boost-rev-b`, `chorus-bom-update`, etc.) and merge to `main` when a revision is validated. See `.gitattributes` for how file types are handled.
