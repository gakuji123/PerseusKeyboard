# PerseusKeyboard

PerseusKeyboard is an AutoHotkey (AHK) script that allows you to control the Perseus SDR receiver software, developed by Nico Palermo, using your keyboard instead of your mouse.
It simulates mouse clicks on the Perseus interface in response to keyboard shortcuts, making receiver operation more convenient.

## Download

The source code is available from the following public GitHub Gist:

**[Download PerseusKeyboard — GitHub Gist](https://gist.github.com/f6fvy/adf5997d8e78922ca2563d9d795161b0)**

Please download the script from the Gist linked above.

## History and Credits

PerseusKeyboard has been developed and improved by several contributors over the years.
- **Laurent Haas (F6FVY)** — Original author, November 2008
- **Aldo Moroni (IW2DZX) and Salvo Micciché (SWL IT9-4639)** — Modifications
- **WoodBoxRadio (IK3VIG)** — Added special commands for ShuttleProV2 USB Human Interface Device control
- **Ferdinand Lenhardt (`perseus_only`)** — Further extensions
- **Gakuji Masuo (7N4NJN)** — Reliability improvements to the frequency input dialog
- **Wolfgang (OE1MWW)** — Valuable suggestions and technical advice

Gakuji Masuo's improvements include repeatedly clicking the kHz confirmation button to improve input reliability, followed by automatically closing the frequency keypad.
Thank you to everyone who has contributed to this project.

## Features

### Frequency Navigation

- Use the arrow keys to adjust the frequency in small steps.
- Hold `Shift` to multiply the frequency step by 10.
- Use `Page Up` and `Page Down` to adjust the tuning step.

### Direct Frequency Entry

- Type digits (`0–9`) and press `Enter` to open the frequency dialog, enter the frequency, and close the dialog automatically.
- Press `m` after entering digits to confirm the value in MHz.
- Press `k` after entering digits to confirm the value in kHz.
- The kHz confirmation routine clicks the confirmation button up to 30 times to improve reliability before closing the keypad.

### Demodulation Modes

Use the following keyboard shortcuts to select the demodulation mode.

| Key | Mode |
|---|---|
| a | AM |
| s | SAM |
| c | CW |
| r | RTTY |
| l | LSB |
| u | USB |
| f | FM |
| d | DRM |
| e | User |

### Receiver Controls

- Span adjustment
- Reference level adjustment
- Notch filter
- Passband Tuning (PBT)
- Autonotch
- Noise Blanker
- Noise Reducer
- SpkRej
- CWPeak
- Mute and volume toggle

### Display Controls

- Switch between waterfall and spectrum views.
- Adjust the center frequency.
- Toggle waterfall zoom.

### WAV Playback

Special shortcuts support navigation through recorded WAV files.

- `Tab` / `Shift+Tab` — Jump forward or backward in the playback bar by a configurable number of seconds.
- `Ctrl+Tab` — Open a dialog to change the jump interval and WAV file length.
- `z` — Switch between WAV files or rewind when only one file is loaded.

### Exit

- `Shift+Q` or `Alt+F4` — Close Perseus and exit the script.

## Requirements

- AutoHotkey v1
- Perseus SDR receiver software (v4.1)
The script expects the Perseus software to be located in the same directory as the script.

## Usage

1. Download [PerseusKeyboard.ahk](https://gist.github.com/f6fvy/adf5997d8e78922ca2563d9d795161b0) from the public Gist linked above.
2. Make sure AutoHotkey v1 is installed.
3. Run `PerseusKeyboard.ahk`.
4. If Perseus is not already running, the script will attempt to launch it.

The keyboard shortcuts are active only while the Perseus window is focused.
Please note that the script simulates mouse clicks at specific positions in the Perseus interface. Its behavior may depend on the software version, screen resolution, display scaling, and window layout.

## Bug Reports and Feedback

If you encounter a problem or have a suggestion for improvement, please report it through the [Issues section](https://github.com/gakuji123/PerseusKeyboard/issues) of this GitHub repository.
When submitting a report, please include:

- Your Windows version
- Your Perseus software version
- Your screen resolution and display scaling, if relevant
- A description of the problem
- The steps required to reproduce it

Please do not include personal or sensitive information in your report.

## Disclaimer

PerseusKeyboard is provided "as is", without any guarantee that it will work in every system configuration.
Please ensure that you have saved any important work before testing the script.

## Acknowledgments

Special thanks to Laurent Haas (F6FVY) and all the contributors who have developed and improved PerseusKeyboard over the years.
