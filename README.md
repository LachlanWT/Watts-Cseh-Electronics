# Watts & Cseh Electronics

Open-source guitar effects pedal designs; circuits, PCBs, chassis, and
docs, version-controlled in one place.

---

## 🔗 Project quick links

**Design & CAD:**<br>
[![Onshape](https://img.shields.io/badge/Onshape-CAD_Storage-1755E3?style=for-the-badge&logo=onshape&logoColor=white)](https://cad.onshape.com/documents?nodeId=eb3223d0357b539d8a4f96e7&resourceType=folder)<br>
[![CADLAB](https://img.shields.io/badge/CADLAB-PCB_Diffs-2E7D32?style=for-the-badge)](https://cadlab.io/project/30399/main/files)

**Parts & sourcing:**<br>
[![McMaster-Carr](https://img.shields.io/badge/McMaster--Carr-Hardware-FFC400?style=for-the-badge)](https://www.mcmaster.com/)<br>
[![DigiKey](https://img.shields.io/badge/DigiKey-Components-CC0000?style=for-the-badge)](https://www.digikey.com/)

**Project management:**<br>
[![Jira](https://img.shields.io/badge/Jira-To--Do_Board-0052CC?style=for-the-badge&logo=jira&logoColor=white)](https://wattsandcseh.atlassian.net/jira/software/projects/WCE/summary)

**Tools:**<br>
[![GitHub Desktop](https://img.shields.io/badge/GitHub_Desktop-Download-24292E?style=for-the-badge&logo=github&logoColor=white)](https://desktop.github.com/)<br>
[![Git LFS](https://img.shields.io/badge/Git_LFS-Large_Files-F64935?style=for-the-badge&logo=git&logoColor=white)](https://git-lfs.com/)<br>
[![LTSpice to KiCad](https://img.shields.io/badge/LTSpice_to_KiCad-Converter-314CB0?style=for-the-badge&logo=kicad&logoColor=white)](https://github.com/FOSSEE/LTSpiceToKiCadConverter)

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
- Don't commit auto-generated files (Gerbers, caches, sim outputs) — these are
  handled by `.gitignore`.
