# ResonanceDump_MusicNoteBox_SDK
# 🎵 Resonance Dump (RD): Music Note Box v1
### High-Performance Text-to-Audio Synthesis

**Resonance Dump (RD)** is a lightweight, portable music engine that transforms logic-based script files (`.mnb`) into system-level audio frequencies.

---

## 🚀 [ QUICK START ]
To install the engine on your system:

1. Place `core_mnb.ps1` and `install_mnb.reg` in any folder of your choice.
2. Right-click `install_mnb.reg` and select **'Merge'**.
3. Click **'Yes'** on the system prompts.
4. Now, simply **double-click** any `.mnb` file to play the music.

> **Note:** Ensure `core_mnb.ps1` remains in the same folder as your tracks for the player to function correctly.

---

## 🛠 [ ADVANCED SYNTAX GUIDE ]
The RD Engine uses a **Token-Based Interpretation** system. It scans for executable commands within brackets `[]` while allowing for an organized, human-readable code structure.

### 1. Variables & Global Settings
* **`soundbox = [X]`**: Sets the global tempo. `X` is the duration in milliseconds for each note or pause. You can change this multiple times within one file to create speed-up (accelerando) or slow-down effects.
    * *Example: `soundbox = [150]`*

### 2. Audio Tokens (Notes & Pauses)
* **Octaves**: Supports two full octaves from **[C4]** to **[B5]**.
* **Sharps (#)**: Use the `#` symbol inside the bracket for half-tones.
    * *Example: `[C#4]`, `[D#5]`, `[F#4]`*
* **Silence**: Use **[P]** (Pause) to create a rest based on the current `soundbox` value.

### 3. Structural Labels (The "sb ::" System)
To keep your code clean, the engine allows the use of **Prefix Labels**. Everything outside the square brackets `[]` (except for the `soundbox` command) is treated as a label and ignored by the synthesizer.
* **Valid Structure:** `sb :: intro = [D4][D4][D5]`
* **Part Separation:** `part_1 : melody = [A4][G4][F4]`
This allows you to name your patterns and sections without breaking playback.

### 4. Documentation
* **Comments**: Lines starting with `#` are completely ignored. Use them for metadata, track titles, or credits.

---

## 💻 [ SYSTEM REQUIREMENTS ]
* **OS:** Windows 10 / 11
* **Environment:** PowerShell 5.1+
* **Hardware:** Internal PC Speaker or System Audio (Beep Service)

---

## 🛡️ [ SECURITY & PERMISSIONS ]
If the engine is blocked by Windows Execution Policy, run PowerShell as Administrator and execute:
`Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope CurrentUser -Force`

---

## 👤 [ CREDITS ]
* **Engine Architecture:** Workstation5495
* **GitHub:** [https://github.com/Workstation5495](https://github.com/Workstation5495)
* **Project:** Resonance Dump

> *"Where code meets the rhythm of the machine."*
