# Sources & attribution

## Inspiration

The interactive stages (stretch → spinal snap → 1→2→4→8 cascade → toothpaste-tube extrusion) follow the popular explanation given by **Neil deGrasse Tyson** on *The Diary Of A CEO*:

- Clip: [Astrophysicist WARNS…](https://www.youtube.com/watch?v=a9W5atyoYT0)
- Full episode: https://youtu.be/PHpsdIHpLUE

This project is an original visualization. It is **not** affiliated with NDT, DOAC, or YouTube.

## Fair-use pedagogical paraphrase (not a transcript)

In words: standing on Earth, your feet are slightly closer to the center than your head, so gravity differs by a tiny amount. Near a black hole that **tidal difference** grows steeply (roughly as \(1/r^3\)). For a small (stellar-mass) black hole the stretch can become lethal **outside** the event horizon; for a supermassive hole you may cross the horizon still roughly intact. Extreme tides can be pictured as stretching head-to-toe and extruding the body through narrowing space “like toothpaste through a tube.”

## Physics model used here

| Quantity | Formula | Notes |
|----------|---------|--------|
| Schwarzschild radius | \(R_s = 2GM/c^2\) | Event-horizon size (non-spinning) |
| Newtonian gravity | \(g(r) = GM/r^2\) | Pedagogical outside the horizon |
| Tidal Δg (exact, head–feet) | \(g(r) - g(r+L)\) | \(L = 1.75\,\mathrm{m}\) |
| Textbook approx | \(\Delta g \approx 2GM L / r^3\) | Shown in the UI |
| Stretch load scale | \(F \approx m\,\Delta g\) | \(m = 70\,\mathrm{kg}\); order-of-magnitude only |

**Not medical or full GR.** Snap thresholds and body deformation are illustrative so the \(1/r^3\) curve is readable. Near and inside \(R_s\), general relativity dominates; the page keeps Newtonian tides so the pedagogy stays clear.

## Libraries

- [Three.js](https://threejs.org/) r170 (CDN via unpkg) — MIT
- Google Fonts: Outfit, IBM Plex Mono
