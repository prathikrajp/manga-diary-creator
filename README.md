# Personal Manga Diary Creator

A zero-budget, single-file web app that converts your weekly life updates into anime-style manga pages and compiles them into a downloadable comic book PDF.

## Live Demo
**https://manga-diary-creator.vercel.app**

## Features
- **AI Prompt Engineering** – Gemini 1.5 Flash rewrites your diary entry into a detailed anime visual prompt
- **AI Image Generation** – HuggingFace cagliostrolab/animagine-xl-3.1 generates a 832x1216 manga-style image
- **Character Consistency** – Every image includes your custom character base (Indian male, engineering student, hostel room, anime style)
- **Manga Timeline** – All pages displayed in a dark-themed manga reader grid
- **LocalStorage Persistence** – Your diary survives tab closes and refreshes
- **PDF Export** – Download all pages as a proper A5 comic book via jsPDF
- **Zero Dependencies** – Single index.html file, no build step, no frameworks

## Quick Start
1. Open the [live app](https://manga-diary-creator.vercel.app) or run locally:
   `
   python -m http.server 5500
   `
   Then visit http://localhost:5500

2. Enter your **Google Gemini API Key** and **HuggingFace Access Token**
3. Write your weekly diary entry and click **Process Entry**
4. Watch your life become a manga page!
5. Repeat weekly — pages stack up in your timeline
6. Click **Download as Book (PDF)** to export your comic

## API Keys (Free)
| Service | Get Key | Used For |
|---|---|---|
| Google Gemini | [aistudio.google.com](https://aistudio.google.com) | Diary → Visual Prompt |
| HuggingFace | [huggingface.co/settings/tokens](https://huggingface.co/settings/tokens) | Prompt → Anime Image |

## Tech Stack
- Pure HTML/CSS/JS (single file)
- Google Gemini 1.5 Flash API
- HuggingFace Inference API (animagine-xl-3.1)
- jsPDF (CDN) for PDF export
- Deployed on Vercel

## Character Base
Every image generation appends:
> 1boy, Indian male, college student, short hair, electronics engineering student, hostel room background, anime style, highly detailed

---
Made with ❤️ and anime dreams.