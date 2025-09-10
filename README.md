# Japa-Translate

A web app for seamless live English-Japanese translation using Google APIs and Voicevox anime voices.

## Features

- Speech-to-text (Google Cloud)
- Text-to-text translation (Google Cloud)
- Text-to-speech (Google Cloud, Voicevox anime voices)
- Speech-to-speech translation
- Select anime-style Japanese voices
- Use browser speech recognition or backend audio recognition
- Translation history
- Multi-language support
- Docker support for deployment

## Install & Run (Local)

1. Clone repo:  
   `git clone https://github.com/arielmeza5-glitch/Japa-Translate`
2. Copy your Google Cloud credentials file to `server/credentials.json`.
3. Copy `.env.example` to `.env` in the `server` folder and adjust as needed.
4. Download and run [Voicevox Engine](https://github.com/VOICEVOX/voicevox_engine/releases) locally.
5. Run install script:  
   `bash install.sh`
6. Start backend:  
   `cd server && npm start`
7. Start frontend:  
   `cd client && npm start`
8. Open [http://localhost:3000](http://localhost:3000)

## Docker Deployment

1. Build and start all services:
   ```
   docker-compose up --build
   ```
2. Make sure to mount your Google credentials file and `.env` as described in `docker-compose.yml`.

## Voicevox Engine Health Check

You can check if Voicevox is running:
```
curl http://localhost:4000/api/voicevox-health
```

## Environment Variables

See `server/.env.example`.  
You must set up your own Google Cloud credentials.

## Testing

Backend tests:
```
cd server
npm test
```

## Usage

- Select input/output language and voice type.
- Type text or use speech input.
- Click "Translate & Speak" for live translation and voice output.
- View your translation history below.

## Credits

- Google Cloud Speech, Translate, TTS
- Voicevox (anime voices)