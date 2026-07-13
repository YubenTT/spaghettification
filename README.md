# Spaghettification

**Interactive 3D demo of tidal forces near a black hole.**

As you fall in, the gravity difference between your feet and head grows roughly as **1/r³** — stretch, structural snap, the 1→2→4→8 cascade, then the toothpaste-tube extrusion Neil deGrasse Tyson describes.

**Live demo:** https://yubentt.github.io/spaghettification/

![License: MIT](https://img.shields.io/badge/license-MIT-blue)
![Static](https://img.shields.io/badge/stack-Three.js%20·%20static-black)

---

## Why this exists

Most black-hole visuals are pure spectacle. This one keeps a **live physics panel** next to the scene so the intuition is numerical:

| You see | What it means |
|---------|----------------|
| `r`, `Rₛ`, `r/Rₛ` | How close you are vs the event horizon |
| `g` at feet / head | Why feet feel heavier first |
| Tidal `Δg` | The 1/r³ story in numbers |
| Stretch load | Order-of-magnitude force on a 70 kg body |
| Mass presets | **Why stellar holes kill you outside the horizon; Sgr A\* often doesn’t** |

Pedagogical **Newtonian** tides — intentionally not full GR — so the curve stays readable. Limits and credits: [`SOURCES.md`](./SOURCES.md).

---

## Run locally

Needs a tiny static server (ES modules + import map; `file://` will not work):

```bash
git clone https://github.com/YubenTT/spaghettification.git
cd spaghettification
python3 -m http.server 8765
# open http://localhost:8765/
```

Controls: drag the distance slider · `←` `→` fine step · `Space` auto-descent · mass pills (stellar / intermediate / Sgr A\*).

---

## Stack

- Single `index.html` — no build step
- [Three.js](https://threejs.org/) r170 + bloom postprocessing (CDN)
- GitHub Pages from `main`

---

## License

[MIT](./LICENSE) — free to fork, teach with, or remix. Attribution appreciated, not required.
