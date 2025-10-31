# WHATS_EduCentre™

**Built for the Google Chrome Built-in AI Challenge 2025**

[Live Demo](https://educentre.hermanus.me) · [WHATS_EduCentre™ Demonstration License (2025)
License](LICENSE)

---

## Overview

**WHATS_EduCentre™** is a fully local, multimodal AI operating environment built inside Google Chrome.  
It transforms the browser into a complete education and creativity studio that runs offline, handles all data locally, and interfaces directly with Google’s **Built-in AI APIs** and **Gemini Nano** models.

Unlike traditional AI platforms, WHATS_EduCentre™ does not send user data to the cloud.  
It uses Chrome’s **File System Access API** and **IndexedDB** to create encrypted local workspaces called **Backpacks**.  
Every file, project, transcript, image, and model interaction remains stored on the user’s device — a secure, private sandbox that becomes a personal AI studio for teachers, students, and creators.

The system follows a clear “**Pantry → Extract → Compose → Produce → Export**” pipeline, guiding a user from data capture to finished output while keeping AI assistance fully embedded in every stage.

---

## System Structure

### 1. Dashboard
The control hub that aggregates all project data.  
Displays:
- Active personas and context (Teacher, Principal, Parent)
- Connected camera feeds and live sensors  
- Project health indicators, task timers, and AI activity logs  

It serves as both mission control and a teaching aid — giving users a live window into what their AI systems are analyzing, producing, or archiving.

---

### 2. Resources
The **Pantry** of the system.  
Users collect source materials — text, images, audio, PDFs, videos, and datasets.  
Each file is stored locally through the File System Access API and automatically indexed with metadata (format, origin, tags).  
Users can drag-and-drop files which become instantly available for AI extraction or creative use later in the workflow.

---

### 3. Extract
The first layer of AI processing.  
Powered by **Gemini 2.5 Flash**, this module performs multimodal extraction:
- OCR from images and scanned PDFs  
- Speech-to-Text transcription from uploaded or recorded audio  
- Scene labeling from still frames or videos  
- Key insight summarization from long documents  
- Named entity extraction for structured metadata  

Outputs include:
- A readable summary for users  
- A structured JSON object reusable across the system

These results form the knowledge layer for composition and production.

---

### 4. Compose
The **creative desk**.  
This editor merges writing, research, and prompt design into one workspace with dynamic persona switching.  
Users can toggle between **Teacher**, **Principal**, **Student**, or **Parent** roles, each with a unique tone and reasoning model.

Functions include:
- AI-assisted drafting and outlining  
- Real-time grammar correction via **Proofreader API**  
- Context-aware rewriting via **Writer** and **Rewriter APIs**  
- Inline summarization via **Summarizer API**  
- Full multilingual translation via **Translator API**

---

### 5. Creative Canvas
The heart of WHATS_EduCentre™ — a **multi-asset synthesis engine** capable of generating:
- Text (Gemini Flash)  
- Still images (Imagen 4)  
- Narrated audio (Gemini TTS)  
- Full video compositions (Veo)

Users select any combination of assets — notes, images, transcripts, voice files — and feed them through a creative brief.  
The Canvas orchestrates multimodal API calls and writes all outputs directly back into the project folder.

---

### 6. WHATS_sight™ (Live Vision)
A real-time AI vision engine that:
- Analyzes ANY SOURCE FILE, Video, Audio, Pdf, Text webcam or uploaded video feeds ANY SIZE ON DEVICE
- Detects and labels objects frame-by-frame using structured Gemini schemas  
- Generates synchronized audio narration through the Gemini Live API  
- Produces scene cards for later use in Compose or Canvas  

Each analysis generates text, audio, and JSON saved to the Backpack — a practical example of multimodal streaming running locally in Chrome.

---

### 7. WHATS_showme™ AI LAZERPOINTER  (UI Analysis)
A self-referential assistant that can analyze the interface itself.  
Users can click any UI element to:
- Identify the element and explain its function  
- Describe its relation to the user’s workflow  
- Provide guided instructions (“You are in Extract mode — click Compose to draft from results.”)

Demonstrates **Gemini multimodal comprehension** applied to live UI state.

---

### 8. Educator Workbench
An AI-persona layer embedded in every workspace.  
Each persona carries its own **systemInstruction** defining voice, tone, and context.  
Before each message, the current view, file list, and scene data are compiled into model context so that the persona can reason specifically about the user’s current work.

---

### 9. Utilities and Mini-Apps
A collection of lightweight, offline-ready utilities integrated into the shell:
- Timer, Translator, Calculator, Flashcard Generator  
- Voice Chat with Gemini Live  
- Game modules for classroom engagement  
- QR Generator and Safe-Book for parental controls  
- Local Slides and Document viewers  

All tools are part of the same local sandbox — no external servers required.

---

### 10. System and Governance Layer
The ethical and operational backbone:
- **SAAIS** — System governor for AI ethics and persona delegation  
- **WHATS_AI™** — Internal prompt router for Gemini and local APIs  
- **WHATS_Currency™** — Tracks Return on Obedience (ROO) metrics  
- **Settings** — Access control, privacy audit, and sandbox management  

Together, they make WHATS_EduCentre™ a sovereign, auditable AI ecosystem.

---

## How We Built It

| Layer | Technology |
|-------|-------------|
| Frontend | Angular 18, TypeScript, TailwindCSS |
| Storage | File System Access API (OPFS), IndexedDB (Dexie.js) |
| Runtime | Chrome Built-in AI / Gemini Nano |
| APIs | Prompt API, Proofreader API, Summarizer API, Translator API, Writer API, Rewriter API |
| Hybrid AI | Gemini 2.5 Flash, Gemini Live API, Gemini TTS API, Imagen 4, Veo |
| Deployment | Google Cloud Run + Firebase AI Logic |
| UX | Progressive Web App (PWA) with offline caching and full local integrity |

---

## Why It Matters

Most AI tools depend on centralized servers.  
**WHATS_EduCentre™** proves that a full-scale, multimodal AI studio can live entirely in the browser — private, offline, and locally sovereign.  
It unifies education, creativity, and governance in one system and demonstrates the future of ethical client-side AI.

---

## Accomplishments

- 27+ operational modules across education, creation, and governance  
- True multimodal generation: text, image, video, and voice  
- Real-time narration and scene analysis of live feeds  
- Seamless offline persistence using OPFS + IndexedDB  
- Persona-driven guidance and ethical AI oversight  
- Deployed as a Cloud Run PWA powered 100% by Google AI and Chrome Built-in APIs

---

## License

WHATS_EduCentre™ Demonstration License (2025) 
See [LICENSE](LICENSE) for details.

---

## Links

- Live Application: https://educentre.hermanus.me  
- System Home: https://saai.services
- Repository: https://github.com/saaisdev/WHATS_EduCentre
