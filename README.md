# 🎹 MIDI SYNTHI

A playable synthesizer and drum machine styled like a hardware MIDI controller, with a recording timeline and MIDI/WAV export — built entirely on the **Web Audio API**, no dependencies, no build step, one HTML file.

**[▶ Play it live](https://tflatischler.github.io/midi-synthi/)**

## Features

- **Controller deck** — rotary knobs (drag, scroll, or arrow keys), waveform selector buttons, 4×2 drum pads and a 2-octave keyboard side by side, like a hardware controller
- **Synth** — 2-oscillator engine with detune, lowpass filter + resonance, full ADSR envelope, and a feedback delay
- **Drums** — 8 synthesized drum sounds (kick, snare, hi-hats, clap, toms, rim)
- **Recording timeline** — piano-roll arrangement view with quantize (1/4–1/32), loop playback, and adjustable length (2–16 bars)
- **Export** — download your arrangement as a **.mid** file (Standard MIDI File, GM drum mapping) or render it offline to **.wav**
- **Presets** — Lead, Bass, Pad, Pluck, Acid, Sub — plus a 🎲 **dice roller** that generates a random patch and previews it
- **Oscilloscope** — live waveform visualizer
- Works with mouse, touch, and computer keyboard

## Keyboard shortcuts

| Key | Action |
| --- | --- |
| `Space` | Play / Stop |
| `Z`–`M` | Lower octave (`S`, `D`, `G`… for sharps) |
| `Q`–`I` | Upper octave (`2`, `3`, `5`… for sharps) |
| `1`–`4`, `Q`–`R` | Drum pads (with keys set to Drums) |

The **Keys play** toggle in the Controller panel decides whether your computer keyboard plays the synth or the drum pads — mouse and touch always play whatever you tap.

## Usage

1. Hit **Rec** — playback starts automatically
2. Play notes on the keyboard or tap the drum pads
3. Notes land on the timeline, quantized to the grid
4. Click a note in the timeline to delete it, or **Clear** to start over
5. Export your loop with **.mid** or **.wav** in the top bar

## Development

It's a single `index.html`. Open it in a browser, or serve it locally:

```sh
python3 -m http.server
```

Pushes to `main` deploy automatically to GitHub Pages via [`deploy.yml`](.github/workflows/deploy.yml).
