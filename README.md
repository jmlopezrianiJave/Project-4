# OSC Sequencer for Pure Data

Video Link: https://youtu.be/v1r74EWErpU

A minimalist **OSC-controlled** music sequencer built in **Pure Data**. Control transport, individual voices (bass, hi-hat, snare, kick), and FX (reverb, distortion) from any OSC controller.

> **Main patch:** `seqMain.pd`

---

## What it does
- **Random music generator**: a lightweight step sequencer that creates evolving patterns.
- **Live control**: start/stop the loop, toggle voices, and shape effects in real time.
- **OSC-first workflow**: designed to be played from a phone/tablet over Wi‑Fi.

---

## Controls (OSC)

The rig expects **7 buttons** and **7 sliders**. Numbers below refer to the control index shown in your OSC app.

### Buttons
1. **Start / Stop** the main loop  
2. **Toggle Bass**  
3. **Toggle Hi-hat**  
4. **Toggle Snare**  
5. **Toggle Kick**  
6. **Toggle Reverb**  
7. **Toggle Distortion**

### Sliders
1. **Main Loop Volume** (master for the sequence)  
2. **Bass Volume**  
3. **Hi-hat Volume**  
4. **Snare Volume**  
5. **Kick Volume**  
6. **Reverb Amount** (dry ↔ wet)  
7. **Distortion Level** (gain/drive)


---

## Requirements
- **Pure Data (vanilla)** 0.52+ recommended
- A phone/tablet **OSC app** (e.g., TouchOSC, mrmr, Lemur)
- Both devices on the **same network**


---

## Quick Start
1. **Open** `seqMain.pd` in Pure Data.
2. **Set OSC input**  
   - Go into "pd connection" and start listening on port 8000
3. **Configure your OSC app**  
   - **Target IP**: your computer’s local IP (e.g., `192.168.1.xxx`)  
   - **Target Port**: the Pd port from step 2 (e.g., `8000`)