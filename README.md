WHATS_EduCentre™

Built for the Google Chrome Built-in AI Challenge 2025

Live Demo
 · MIT License

Overview

WHATS_EduCentre™ is a fully local, multimodal AI operating environment built inside Google Chrome.
It transforms the browser into a complete education and creativity studio that runs offline, handles all data locally, and interfaces directly with Google’s Built-in AI APIs and Gemini Nano models.

Unlike traditional AI platforms, WHATS_EduCentre™ does not send user data to the cloud. It uses Chrome’s File System Access API and IndexedDB to create encrypted local workspaces called Backpacks.
Every file, project, transcript, image, and model interaction remains stored on the user’s device — a secure, private sandbox that becomes a personal AI studio for teachers, students, and creators.

The system follows a clear “Pantry → Extract → Compose → Produce → Export” pipeline, guiding a user from data capture to finished output while keeping AI assistance fully embedded in every stage.

System Structure
1. Dashboard

The control hub that aggregates all project data. It displays:

Active personas and context (Teacher, Principal, Parent, etc.)

Connected camera feeds and live sensors

Project health indicators, task timers, and AI activity logs
It serves as both mission control and a teaching aid — giving users a live window into what their AI systems are analyzing, producing, or archiving.

2. Resources

The “Pantry.”
Here users collect source materials — text, images, audio, PDFs, videos, and dataset fragments.
Each file is stored locally through the File System Access API and automatically indexed with metadata (format, origin, tags).
Users can manually add or drag-and-drop resources, which are instantly available for AI extraction or creative use later in the workflow.

3. Extract

The first layer of AI processing.
Gemini 2.5 Flash is used here for multimodal content extraction:

OCR from images and scanned PDFs

Speech-to-Text transcription from uploaded or recorded audio

Scene labeling from still frames or videos

Key insights & summaries from documents

Named entity extraction for structured metadata

Every extraction produces two outputs:

A readable summary (for user understanding)

A structured JSON object (for re-use across modules)

These results form the knowledge layer for subsequent composition and production.

4. Compose

The “creative desk.”
This environment merges writing, research, and prompt design into a single adaptive editor.
It supports live persona switching — for example, switching from Teacher (academic tone) to Dad (supportive tone) or Principal Wendy (administrative review).

Key features:

AI-assisted drafting, outlining, and rewriting

Real-time grammar correction via Proofreader API

Context-aware rephrasing via Writer and Rewriter APIs

Inline summarization of long sections

Multi-language translation via Translator API

The Compose view turns any extraction into a structured article, report, or story — guided by whichever persona is active.

5. Creative Canvas

The heart of WHATS_EduCentre™ — where all assets converge.
It is not limited to text; it is a multi-asset synthesis engine that can generate:

Text (Gemini Flash)

Still images (Imagen 4)

Narrated audio (Gemini TTS)

Full video compositions (Veo)

Users can select any combination of existing files — notes, images, voice tracks, transcripts, or generated JSON — and blend them through a creative brief (“Generate a 60-second explainer using these”).
The Canvas orchestrates multimodal API calls and assembles outputs directly back into the project.

It’s essentially a localized version of NotebookLM plus Studio — a single-screen production suite.

6. WHATS_sight™ (Live Vision)

A dedicated AI vision engine.

Analyzes webcam or uploaded video in real time

Detects and labels objects frame-by-frame (using Gemini structured schema)

Generates live narrations through Gemini Live API

Produces synchronized transcripts and “scene cards” for reuse in Compose or Canvas

Each analysis run saves text, audio, and structured JSON back to the Backpack.
It demonstrates true multimodal streaming — simultaneous vision, language, and audio synthesis running inside Chrome.

7. WHATS_showme™ (UI Analysis)

A meta-assistant that can analyze its own interface.
Users can click any part of the UI, capture it as an image, and receive:

Identification of the UI element

Explanation of its function

Contextual advice (“You are in Extract mode — this button links to Compose”)

This showcases practical use of Gemini multimodal comprehension on a live, running application.

8. Educator Workbench

An AI-persona layer embedded in every workspace.

Each persona (Teacher, Principal, Student, Parent) has its own systemInstruction with tone, role, and scope.

Before every chat, the current view, file list, and scene data are compiled into the model context.

This allows responses that are deeply specific — e.g., a “Teacher” persona reviewing a child’s assignment will cite data from Extract and Compose directly.

9. Utilities and Mini-Apps

WHATS_EduCentre™ includes a suite of lightweight utilities that operate fully offline:

Timer, Translator, Calculator, Flashcard Generator

Voice Chat with Gemini Live

Game modules and QR Generator for classroom engagement

Sleepover Safe-Book (parental mode)

Slides, Documents, and Trash Bin (local management)

These are all built into the shell, accessible from the lower navigation bar.

10. System and Admin Layer

SAAIS — System governor for AI ethics and role delegation.

WHATS_AI™ — Internal Gemini prompt router that coordinates between local and hybrid APIs.

WHATS_Currency™ — Manages Return on Obedience (ROO) and learning economy metrics.

Settings — Access control, sandbox reset, privacy audit.

This layer turns WHATS_EduCentre™ into a sovereign, auditable AI ecosystem, not just a single app.

How we built it
Layer	Technology
Frontend	Angular 18, TypeScript, TailwindCSS
Storage	File System Access API (OPFS), IndexedDB (Dexie.js)
Runtime	Chrome Built-in AI / Gemini Nano
APIs	Prompt API, Proofreader API, Summarizer API, Translator API, Writer API, Rewriter API
Hybrid AI	Gemini 2.5 Flash, Gemini Live API, Gemini TTS API, Imagen 4, Veo
Deployment	Google Cloud Run + Firebase AI Logic
UX	Progressive Web App with offline caching and full local data integrity
Why it matters

Traditional AI relies on cloud processing and external data collection.
WHATS_EduCentre™ proves that a multimodal, full-scale AI studio can live entirely in the browser — preserving privacy, running offline, and still delivering professional-grade generative power.

It’s not a chatbot. It’s a local AI operating system — the foundation for future classrooms, maker studios, and creative ecosystems.

Accomplishments

27+ operational modules under a unified local AI shell

True multimodal generation across text, image, video, and voice

Live narration and analysis of real-world feeds

Seamless offline persistence using OPFS and IndexedDB

Persona-driven governance and ethical AI framework

Fully deployed on Cloud Run, installable as a PWA

100% powered by Chrome’s Built-in AI + Gemini Nano

License

MIT © 2025 Commander Jaco / WHATS_SYSTEM™
See LICENSE
 for details.

Links

Live Application: https://educentre.hermanus.me

System Home: https://whatsai.africa

Repository: https://github.com/saaisdev/WHATS_EduCentre
