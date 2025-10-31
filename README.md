# WHATS_EduCentre™
**Built for the Google Chrome Built-in AI Challenge 2025**

[Live Demo](https://educentre.hermanus.me) · [MIT License](LICENSE)

---

## Overview

WHATS_EduCentre™ is a local-first, multimodal AI education studio that runs entirely inside Chrome.  
It combines Gemini Nano (on-device intelligence) with the Chrome Built-in AI APIs to create a secure learning workspace for teachers, students, and creators — no cloud dependency, no logins, full privacy.

Using the browser’s File System Access API, it stores all work locally in encrypted project folders.  
The result is an offline-capable environment for AI-assisted learning, analysis, and creation.

---

## What it does

- Prompt Builder — Generate structured prompts with multimodal context  
- Proofreader — Improve grammar and clarity in real time  
- Summarizer — Condense complex material into key insights  
- Translator — Translate any file or text instantly  
- Writer and Rewriter — Draft or refine content intelligently  
- WHATS_sight™ — Analyze Videos, Audio, images, PDFs, or live webcam feeds with Gemini 2.5 Flash  
- Creative Canvas — Combine text, images, and videos using Imagen 4, Veo, and Gemini TTS  
- Live Narrator — Real-time audio synthesis via Gemini Live API  

All processing occurs locally or through privacy-preserving hybrid calls — never uploading user data.

---

## How we built it

| Layer | Technology |
|-------|-------------|
| Frontend | Angular 18, TypeScript, TailwindCSS |
| Storage | File System Access API (OPFS), IndexedDB (Dexie.js) |
| Runtime | Chrome Built-in AI / Gemini Nano |
| APIs | Prompt API, Proofreader API, Summarizer API, Translator API, Writer API, Rewriter API |
| Hybrid AI | Gemini 2.5 Flash, Gemini Live API, Gemini TTS API, Imagen 4, Veo |
| Deployment | Google Cloud Run with Firebase AI Logic |
| UX | Progressive Web App with offline caching and local data integrity |

---

## How to test

1. Visit [https://educentre.hermanus.me](https://educentre.hermanus.me)  
2. Create a new project folder using the File System Access API  
3. Test the following modules:  
   - Summarizer — Drop in a PDF or text file  
   - Translator — Select a target language  
   - Creative Canvas — Select assets and generate a result  
   - WHATS_sight™ — Analyze any source file or feed with real-time narration and scene card creation
4. Observe structured JSON responses, streamed output, and real-time speech  
5. All generated files (.txt, .wav, .png, .mp4) are saved locally on the user’s device

---

## Why it matters

Traditional AI tools rely on centralized servers.  
WHATS_EduCentre™ demonstrates that a complete, multimodal AI studio can run entirely client-side, keeping data sovereign while delivering professional-grade learning and creative capabilities.

---

## Accomplishments

- Fully local workflow with no logins or uploads  
- Hybrid multimodal generation (text, image, audio, video)  
- Real-time narration for live and recorded media  
- 100% powered by Google AI and Chrome Built-in AI APIs  
- Deployed and functional as a PWA via Cloud Run

---

## License

MIT © 2025 Commander Jaco / WHATS_SYSTEM™  
See the [LICENSE](LICENSE) file for details.

---

## Links

- Live Application: https://educentre.hermanus.me  
- System Home: https://whatsai.africa  
- Repository: https://github.com/saaisdev/WHATS_EduCentre
