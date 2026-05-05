# ModuleDanishLanguagePack

Complete Danish language pack for MikoPBX including UI translations and voice prompts.

## What's Included

- **Voice Prompts**: Danish voice prompts for system menus, greetings, and notifications
- **UI Translations**: Complete Danish translation of MikoPBX admin interface
- **Text Mapping**: `Sounds/core-sounds-da-dk.txt` — full list of TTS-generated prompts with text

## Voice Generation

A subset of voice prompts (those missing from the upstream Asterisk Danish set) was generated using neural TTS (Text-to-Speech) technology:

- **Engine**: [Piper TTS](https://github.com/rhasspy/piper)
- **Voice model**: `da_DK-talesyntese-medium`
- **Sample rate**: 22050 Hz
- **Format**: WAV (PCM signed 16-bit, mono)

The text for each TTS-generated prompt is stored in `Sounds/core-sounds-da-dk.txt` for reference and regeneration.

On module installation, MikoPBX automatically converts WAV files to all Asterisk formats (ulaw, alaw, gsm, g722, sln) for optimal codec compatibility.

## TTS Attribution

The Piper TTS voice model `da_DK-talesyntese-medium` is published by the Rhasspy project on Hugging Face and is based on training data from Talesyntese (https://github.com/grammakov/danish-tts). TTS-generated audio in this package is provided under CC BY-SA 4.0.

## Installation

1. Download and install the module from MikoPBX Marketplace
2. Enable the module in **Modules** section
3. Go to **General Settings** and select Danish (Dansk) as the system language

## Requirements

- MikoPBX 2025.1.1 or later

## License

- Module code: GNU General Public License v3.0
- Sound files: CC BY-SA 4.0 (Asterisk Sound Files and TTS-generated audio)
- TTS engine: Piper TTS (https://github.com/rhasspy/piper)

## Copyright

- Module development: © 2017-2026 Alexey Portnov and Nikolay Beketov
- Voice synthesis: Generated using open-source TTS models
- Remaining system sounds (silence, tones): From official Asterisk release (CC BY-SA 4.0)
