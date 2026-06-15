# Zundamon Desktop

Zundamon Live2D desktop companion powered by Ollama and VOICEVOX.

![Live2D](https://img.shields.io/badge/Live2D-Cubism4-green)
![Vite](https://img.shields.io/badge/Vite-TypeScript-blue)

## Features

- Live2D character with full-body display and smooth animations
- Chat with Zundamon via text or microphone (Web Speech API)
- Voice synthesis with lip sync (VOICEVOX)
- Local LLM responses (Ollama)
- Expression changes based on conversation sentiment
- Cursor tracking, idle gaze wander, and body movement

## Requirements

- [Node.js](https://nodejs.org/)
- [Ollama](https://ollama.com/) running locally with `gemma4:latest` pulled
- [VOICEVOX](https://voicevox.hiroshiba.jp/) running locally (port 50021)
- Zundamon Live2D model files (place in `zundamon/public/zundamon/`)

## Setup

```bash
cd zundamon
npm install
npm run dev
```

Open http://localhost:5173 in your browser.

## Model

Change the model in `src/main.ts`:

```ts
const MODEL_ID = "gemma4:latest";      // Ollama model
const VOICEVOX_SPEAKER = 3;            // VOICEVOX speaker ID (3 = ずんだもん ノーマル)
```
