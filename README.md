# 🎹 MIDI SYNTHI

A playable synthesizer and drum machine with a recording timeline, built entirely on the **Web Audio API** — no dependencies, no build step, one HTML file.

**[▶ Play it live](https://tflatischler.github.io/midi-synthi/)**

## Features

- **Synth** — 2-oscillator engine with detune, lowpass filter + resonance, full ADSR envelope, and a feedback delay
- **Drums** — 8 synthesized drum sounds (kick, snare, hi-hats, clap, toms, rim) on tappable pads
- **Recording timeline** — piano-roll arrangement view with quantize (1/4–1/32), loop playback, and adjustable length (2–16 bars)
- **Presets** — Lead, Bass, Pad, Pluck, Acid, Sub
- **Oscilloscope** — live waveform visualizer
- Works with mouse, touch, and computer keyboard

## Keyboard shortcuts

| Key | Action |
| --- | --- |
| `Space` | Play / Stop |
| `Z`–`M` | Lower octave (`S`, `D`, `G`… for sharps) |
| `Q`–`I` | Upper octave (`2`, `3`, `5`… for sharps) |
| `1`–`4`, `Q`–`R` | Drum pads (in Drums mode) |

## Usage

1. Hit **Rec** — playback starts automatically
2. Play notes on the keyboard or tap the drum pads
3. Notes land on the timeline, quantized to the grid
4. Click a note in the timeline to delete it, or **Clear** to start over

## Development

It's a single `index.html`. Open it in a browser, or serve it locally:

```sh
python3 -m http.server
```

Pushes to `main` deploy automatically to GitHub Pages via [`deploy.yml`](.github/workflows/deploy.yml).
