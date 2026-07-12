# talat-lab

Small interactive experiments — physics, space, one-page demos.  
Not product code. Each folder is self-contained and static when possible.

## Sketches

| Sketch | What | Demo |
|--------|------|------|
| [spaghettification](./spaghettification/) | Tidal forces near a black hole (Δg ∝ 1/r³) — NDT-inspired | [Open](https://yubentt.github.io/talat-lab/spaghettification/) |

## Local

```bash
cd talat-lab
python3 -m http.server 8765
# http://localhost:8765/spaghettification/
```

## Convention

- One idea per folder
- Prefer single `index.html` (or minimal static stack)
- `README.md` = what + why + source credit
- No CI/product scaffolding unless it graduates out of lab
