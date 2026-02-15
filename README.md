# GreenGuard

**The AI-Powered Truth Detector for the Green Economy.**

Built for [Insert Hackathon Name] 2026

GreenGuard detects corporate "greenwashing" in real-time. By combining Google's Gemini AI with web scraping, we analyze marketing text, sustainability reports, and URLs to separate verified facts from vague marketing fluff.

---

## Screenshots

| Dashboard Analysis | X-Ray Mode |
|:---:|:---:|
| ![Dashboard](https://via.placeholder.com/400x200?text=Dashboard+Screenshot) | ![XRay](https://via.placeholder.com/400x200?text=X-Ray+Mode) |
| *Risk Scoring & Gauges* | *Real-time Keyword Highlighting* |

| The "De-Greenwash" Reveal | Wall of Shame |
|:---:|:---:|
| ![Reveal](https://via.placeholder.com/400x200?text=De-Greenwash+Result) | ![Social](https://via.placeholder.com/400x200?text=Wall+of+Shame) |
| *Generative AI Rewrite* | *Community Tracking Feed* |

---

## Key Features

* **AI Risk Analysis:** Scores marketing claims (0-100) based on verified data vs. vague buzzwords.
* **Industry Context:** Tailored prompts for Fashion, Energy, Automotive, and Food sectors.
* **X-Ray Vision:** Instantly highlights red-flag keywords like "Eco-friendly", "Natural", and "Carbon-neutral".
* **De-Greenwash Button:** Uses Generative AI to rewrite misleading copy into brutally honest, factual statements.
* **URL Scanner:** Scrapes and analyzes external websites and press releases instantly.
* **Wall of Shame:** A live community feed tracking the worst offenders and verified greenwashing reports.

---

## Tech Stack

**Frontend:**
* React (Vite)
* Tailwind CSS
* Axios (API Requests)

**Backend:**
* Node.js & Express
* Cheerio (Web Scraping)
* Google Gemini API (1.5 Flash Model)

---

## Installation & Setup

Follow these steps to run GreenGuard locally.

### 1. Clone the Repository
```bash
git clone [https://github.com/adnanfaris495/green-guard.git](https://github.com/adnanfaris495/green-guard.git)
cd green-guard

2. Backend Setup
Navigate to the server directory and install dependencies:

Bash
cd server
npm install
Create a .env file in the /server directory:

Code snippet
PORT=5001
GEMINI_API_KEY=your_google_gemini_key_here
Start the server:

Bash
node index.js
3. Frontend Setup
Open a new terminal window:

Bash
cd client
npm install
npm run dev
4. Access the App
Open your browser and navigate to http://localhost:5173 (or the port shown in your terminal).
