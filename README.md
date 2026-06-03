# Watts & Cseh Electronics

Open-source guitar effects pedal designs — circuits, PCBs, enclosures, and
documentation, version-controlled in one place.

Each product folder holds the full design: the LTspice circuit, the KiCad
board, the enclosure CAD, the faceplate art, and the docs (BOM, assembly
notes, datasheets).

---

## 🔗 Project quick links

**Design & CAD**
[![Onshape](https://img.shields.io/badge/Onshape-CAD_Storage-1755E3?style=for-the-badge&logo=onshape&logoColor=white)](https://cad.onshape.com/documents?nodeId=eb3223d0357b539d8a4f96e7&resourceType=folder)
[![CADLAB](https://img.shields.io/badge/CADLAB-PCB_Diffs-2E7D32?style=for-the-badge)](https://cadlab.io/project/30399/main/files)

**Parts & sourcing**
[![McMaster-Carr](https://img.shields.io/badge/McMaster--Carr-Hardware-FFC400?style=for-the-badge)](https://www.mcmaster.com/)
[![DigiKey](https://img.shields.io/badge/DigiKey-Components-CC0000?style=for-the-badge)](https://www.digikey.com/)

**Project management**
[![Jira](https://img.shields.io/badge/Jira-To--Do_Board-0052CC?style=for-the-badge&logo=jira&logoColor=white)](https://wattsandcseh.atlassian.net/jira/software/projects/WCE/summary)

**Tools**
[![Git LFS](https://img.shields.io/badge/Git_LFS-Large_Files-F64935?style=for-the-badge&logo=git&logoColor=white)](https://git-lfs.com/)
[![LTSpice to KiCad](https://img.shields.io/badge/LTSpice_to_KiCad-Converter-314CB0?style=for-the-badge&logo=kicad&logoColor=white)](https://github.com/FOSSEE/LTSpiceToKiCadConverter)

---

## Products

| Product | Status | Description |
|---|---|---|
| **Treble Boost** | In progress | — |
| **Chorus** | In progress | — |

---

## Repository structure

```
pedals/
├── Treble-Boost/
│   ├── circuit/     LTspice .asc / .asy + sim notes
│   ├── board/       KiCad project (.kicad_pro, _sch, _pcb)
│   ├── model/       enclosure CAD exports (.step / .stl)
│   ├── art/         decals, faceplate graphics, renders
│   └── docs/        BOM (.csv), assembly notes, datasheets
│
├── Chorus/          (same layout)
│
└── _shared/
    ├── kicad-libs/  custom symbols & footprints
    ├── templates/   BOM template, doc template
    └── 3d-models/   common parts (jacks, pots, switches)
```

---

## Getting started

This repo uses **Git LFS** for binary assets (STEP, STL, 3MF, renders).
Install it once before cloning so large files download correctly:

```bash
git lfs install
git clone https://github.com/LachlanWT/Watts-Cseh-Electronics.git
```

KiCad library paths are set **relative** to `_shared/kicad-libs`, so the
project opens correctly on any machine after cloning.

---

## Contributing

- Work on a branch per revision (e.g. `treble-boost-rev-b`), merge to `main`
  once the revision is validated.
- Keep `main` buildable.
- Don't commit auto-generated files (Gerbers, caches, sim outputs) — these are
  handled by `.gitignore`.
