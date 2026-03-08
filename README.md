# ResonanceDump_MusicNoteBox
New music file format
--- Resonance Dump: Music Note Box v1 ---
High-Performance Text-to-Audio Synthesis
Resonance Dump (RD) is a lightweight, portable music engine that turns
logic-based script files (.mnb) into system-level audio frequencies.

[ QUICK START ]
To install the engine on your system:

Place 'core_mnb.ps1' and 'install_mnb.reg' in any folder of your choice.

Right-click 'install_mnb.reg' and select 'Merge'.

Click 'Yes' on the system prompts.

Now, simply double-click any .mnb file to play the music.

Note: Ensure 'core_mnb.ps1' remains in the same folder as your tracks.

[ ADVANCED SYNTAX GUIDE ]
The RD Engine uses a Token-Based Interpretation system. It scans for executable commands within brackets while allowing for organized code structure.

1. Variables & Global Settings
soundbox = [X] : Sets the global tempo. X is the duration in milliseconds for each note or pause. You can change this multiple times within one file to create speed-up effects.
Example: soundbox = [150]

2. Audio Tokens (Notes & Pauses)
Octaves: Supports two full octaves from [C4] to [B5].

Sharps (#): Use the # symbol inside the bracket for half-tones.
Example: [C#4], [D#5], [F#4]

Silence: Use [P] (Pause) to create a rest based on the current soundbox value.

3. Structural Labels (The "sb ::" System)
To keep your code clean, the engine allows the use of Prefix Labels. Everything outside the square brackets [] (except for the soundbox command) is treated as a label and ignored by the synthesizer.

Valid Structure: sb :: intro = [D4][D4][D5]

Part Separation: part_1 : melody = [A4][G4][F4]
This allows you to name your patterns and sections without breaking the playback.

4. Documentation
Comments: Lines starting with # are completely ignored. Use them for metadata or track titles.

[ SYSTEM REQUIREMENTS ]
Windows 10 / 11

PowerShell 5.1+

Internal PC Speaker or System Audio (Beep Service)

[ SECURITY & PERMISSIONS ]
If the engine is blocked by Windows Execution Policy, run PowerShell as Administrator and execute:
Set-ExecutionPolicy -ExecutionPolicy Bypass -Scope CurrentUser -Force

[ CREDITS ]
Engine Architecture: Workstation5495
GitHub: https://github.com/Workstation5495
Project: Resonance Dump

"Where code meets the rhythm of the machine."
