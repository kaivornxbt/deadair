# DEAD AIR

Booth that mixes [pump.fun](https://pump.fun).

Most bots go all in on one click and all out on one panic.  
DEAD AIR rides a **fader**: in on the build, out on the drop, at zero before silence.

**Idea:** buys per minute = BPM. When the BPM dies, the track is over.

<p align="center">
  <img src="./preview.jpg" width="520" alt="DEAD AIR terminal — PEAK / DROP"/>
</p>

<p align="center">
  <img src="./preview-cut.jpg" width="520" alt="DEAD AIR terminal — CUT / fader zero"/>
</p>

## How it works

One mint = one track. Everything on the desk shares one **set clock**.

| Phase | What happens |
|-------|----------------|
| **DIG** | Scan crates. Fat-dev / bundled mints go in the bin. |
| **CUE** | Load a clean mint (low dev %, 0 bundles) onto deck A. |
| **BUILD** | 3 fade-ins (size in). Fader climbs to 100%. Outs are armed before entry. |
| **DROP → PEAK** | Buys/min spikes. Floor is hot. Start peeling. |
| **FADE** | Buys/min slides. Rule: **&lt; 68 → fader to zero**. |
| **CUT** | Dev pulls the plug. Bag was already flat — 0 SOL on the dead deck. |
| **RELOAD → NEXT** | Dig the next record while other bots are still dancing on silence. |

```
DIG → CUE → BUILD → DROP → PEAK → FADE → CUT → RELOAD → NEXT
```

### Desk modules

- **Deck A / B** — live mint vs next cue (vinyl + hot cues)
- **Mixer** — EQ = risk (HI dev / MID bundles / LOW holders), channel fader = size, crossfader = which mint holds the bag
- **Waveform** — height = buys/min, markers for IN / DROP / OUT / CUT
- **Setlist + booth bank** — tracks, net SOL, caught rugs
- **MC log** — what the booth is saying in real time

Alone each module is gear. Together it's a set that never plays into dead air.

## Example set (~28s)

Illustrative round (not live telemetry):

1. **DIG** — 380 records · bin TOXIC (dev 31%) + BUNDLEZ (9 bundles) · cue mint with dev 1.4% / 0 bundles  
2. **BUILD** — 3×0.35 SOL fade-ins @ $4.9K / $7.2K / $10.1K · avg entry $7.4K · fader 100%  
3. **DROP → PEAK** — 96 buys/min · OUT 1 35% @ ×3.2 → 1.12 SOL · OUT 2 35% @ ×6.1 → 2.14 SOL  
4. **FADE** — 96 → 66 buys/min · rule &lt; 68 · OUT 3 last 30% @ ×5.4 → 1.89 SOL · fader 0%  
5. **CUT** — dev pulls 0.8s later · −91% · **0 SOL caught** · net **+5.15 SOL** a track  

## Open the terminal

1. Open [`index.html`](./index.html) in Chrome  
2. Watch one full set loop (~28s)  
3. Frame: **1080×1350**

No install. No backend. Just the booth.

## Link

Post: https://x.com/kaivornxbt/status/2111079589631943145
