# HŌLUA

**A first-person hōlua sledding game.** Race a papa hōlua down a Kona mountainside at sunset — thread the rocks, hop the rock field, hold your nerve through the speed wobble — then hit the stone ramp and launch off a sea cliff into the ocean. Launch distance is the trophy stat.

**Play it:** open `index.html` in any modern browser. That's the whole game — one HTML file (Three.js r128 from CDN; everything else procedural: terrain, ocean, sky, particles, and audio).

**Fully offline:** `holua-offline.html` is the same game with Three.js embedded in the file — no internet needed at all. Copy that one file anywhere and double-click it.

## About hōlua

Hōlua is the ancient Hawaiian sport of racing down steep mountainside slides on a papa hōlua — a hardwood sled about twelve feet long and only six inches wide, ridden head first at speeds estimated above 50 mph. The great slide at Keauhou on Hawaiʻi Island ran from high on the mountainside down toward the sea at Heʻeia Bay. This run imagines that ride, from summit grass to open water.

## How to play

The run has three sections — **Ka Piko** (the summit), **Ke Ala Loa** (the long path), and **Ka Lele** (the leap) — about a minute from the start drum to the cliff.

| Key | Action |
| --- | --- |
| `A` / `D` or arrows | Lean and steer |
| `W` | Tuck — much faster, half the steering |
| `S` | Drag-foot brake |
| `Space` | Hop — you'll need it for the small-rock field |
| `R` | Restart the run |
| `Esc` | Back to the title screen |
| `Enter` | Ride |

Tips:

- Tucking cuts drag ~40% and is the only way to reach top speed — but above 50 mph the sled develops **speed wobble**. Damp it with small counter-steers or it will throw you.
- Steer around the boulders on the path. Passing within a meter of one above 40 mph scores a **Kokoke!** (near miss).
- One section is blocked by a field of small rocks — hop it or crash.
- Three crashes end the run. Checkpoints at each section.
- Launch distance is real projectile physics off the 25° ramp: every extra mph of exit speed buys visible feet. A clean full-tuck run flies roughly 200+ feet.

## Tech notes

- Single file, no build step, no external assets beyond the Three.js CDN script.
- Procedural everything: spline-swept half-pipe track with banked turns, heightfield terrain with a sea cliff, sine-displaced ocean with sun glitter, instanced pili grass and rocks, pooled particles.
- All audio is synthesized live with the Web Audio API — wind, runner rumble, rock crackle, drums, heartbeat, splash.
- Targets 60 fps on a mid-range laptop; device pixel ratio capped at 2; no memory growth across restarts.

## Credits & license

Created by [Olin Lagon](https://github.com/olagon) with Claude.

[MIT License](LICENSE) — open source. E komo mai: forks and pull requests welcome.
