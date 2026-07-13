# Spaghettification

Interactive 3D demo of **tidal forces** near a black hole.

**Live:** https://yubentt.github.io/spaghettification/

---

## Idea

Your feet are closer to the hole than your head, so gravity is stronger at your feet. That difference (Δg) grows like **1/r³**.

Drag the slider to fall in. Watch:

1. stretch  
2. structural snap  
3. 1 → 2 → 4 → 8  
4. toothpaste-tube extrusion  

**Mass matters.** A stellar hole (~10 M☉) can tear you apart *outside* the event horizon. Sgr A\* (~4×10⁶ M☉) often lets you cross while still roughly intact.

Physics on the page is **Newtonian** (clear for teaching). Not full GR. Details: [`SOURCES.md`](./SOURCES.md).

---

## Run

```bash
git clone https://github.com/YubenTT/spaghettification.git
cd spaghettification
python3 -m http.server 8765
```

Open http://localhost:8765/  
Needs a local server (ES modules). `file://` will not work.

---

## Controls

| Input | Action |
|--------|--------|
| Distance slider | Far → near |
| Auto descent | Animated fall |
| **0.5× / 1× / 1.5×** | Autoplay speed (default **0.5×**) |
| Mass pills | 10 M☉ · 10³ M☉ · Sgr A\* |
| `←` `→` | Fine step |
| `Space` | Play / pause |

White figure = **YOU** (feet toward the hole). Live numbers are in the right panel.

---

## Stack

- One static `index.html` (no build)
- Three.js r170 + bloom (CDN)
- GitHub Pages from `main`

## License

[MIT](./LICENSE)
