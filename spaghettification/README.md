# Spaghettification

Interactive single-page 3D visualization of **tidal forces** near a black hole — the process Neil deGrasse Tyson describes as stretching, spinal snap, bifurcation (`1 → 2 → 4 → 8…`), and extrusion “like toothpaste through a tube.”

## Live

**https://yubentt.github.io/talat-lab/spaghettification/**

Repo: [YubenTT/talat-lab](https://github.com/YubenTT/talat-lab)

## Run locally

```bash
# from repo root
python3 -m http.server 8765
# http://localhost:8765/spaghettification/
```

> ES modules + import map require a local (or Pages) server — not `file://`.

## Features

- **Log-mapped distance slider** (far → horizon) so the \(1/r^3\) tidal curve is usable
- **Live physics**: \(r\), \(R_s\), \(r/R_s\), \(g_{\text{feet}}\), \(g_{\text{head}}\), \(\Delta g\), stretch load, visual stretch
- **Mass presets**: \(10\,M_\odot\) stellar · \(10^3\,M_\odot\) intermediate · \(4\times10^6\,M_\odot\) Sgr A\*
- **Stages**: safe → stretch → snap → bifurcate → toothpaste tube → event horizon
- **Three.js** + bloom, accretion disk, photon ring, clear human silhouette

## Physics (pedagogical Newtonian tides)

| Quantity | Formula |
|----------|---------|
| Schwarzschild radius | \(R_s = 2GM/c^2\) |
| Gravity at distance \(r\) | \(g = GM/r^2\) |
| Tidal difference (exact) | \(\Delta g = g(r_{\text{feet}}) - g(r_{\text{head}})\) |
| Textbook approx | \(\Delta g \approx 2GM L / r^3\) with \(L = 1.75\,\mathrm{m}\) |
| Stretch load scale | \(F \approx m\,\Delta g\) with \(m = 70\,\mathrm{kg}\) |

**Why mass matters:** stellar-mass holes spaghettify you *outside* the horizon; for Sgr A\* you can cross \(R_s\) while still roughly intact (GR still applies; this page uses Newtonian tides for clarity).

## Source

- Video: [Astrophysicist WARNS…](https://www.youtube.com/watch?v=a9W5atyoYT0) (Diary of a CEO clip, Neil deGrasse Tyson)
- Cleaned transcript: [`TRANSCRIPT.md`](./TRANSCRIPT.md)
