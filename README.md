# Japa-Translate

A web app for seamless live English-Japanese translation using Google APIs and Voicevox anime voices.

## Features

- Speech-to-text (Google Cloud)
- Text-to-text translation (Google Cloud)
- Text-to-speech (Google Cloud, Voicevox anime voices)
- Speech-to-speech translation
- Select anime-style Japanese voices
- Use browser speech recognition or backend audio recognition

## Install & Run

1. Clone repo:  
   `git clone https://github.com/arielmeza5-glitch/Japa-Translate`
2. Run install script:  
   `bash install.sh`
3. Set up Google Cloud credentials for Speech, TTS, Translate (see Google Cloud docs).
4. Download and run [Voicevox Engine](https://github.com/VOICEVOX/voicevox_engine/releases) locally.
5. Start backend:  
   `cd server && npm start`
6. Start frontend:  
   `cd client && npm start`
7. Open [http://localhost:3000](http://localhost:3000)

## Usage

- Select input/output language and voice type.
- Type text or use speech input.
- Click "Translate & Speak" for live translation and voice output.

## Credits

- Google Cloud Speech, Translate, TTS
- Voicevox (anime voices)