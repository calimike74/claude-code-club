# 02 — The Toolkit

## The Core Stack

Every student should be set up with these before they build anything else. This is the baseline.

| Layer | Tool | What It Does | Free Tier |
|-------|------|-------------|-----------|
| **Build** | Claude Code | AI-assisted development from the terminal | Included with Claude subscription |
| **Database + Auth** | Supabase | PostgreSQL database, authentication, file storage, real-time | Generous free tier |
| **AI** | Google AI Studio | Gemini API for text, image, and multimodal understanding | Free |
| **Deploy** | Vercel | Hosting and deployment for web apps | Free hobby tier, unlimited deploys |
| **Version Control** | GitHub | Code hosting, collaboration, CI/CD | Free for public and private repos |

---

## Communication — Making Apps That Talk to People

### Resend
**What it is:** Email API designed for developers.
**Free tier:** 3,000 emails per month (100 per day).
**No credit card required.**

**What it unlocks:** The moment your app can send an email, it feels real. Automated reminders, confirmation emails, weekly summaries, password resets, magic link authentication.

**Why it matters:** Most student projects feel like toys because they can't communicate with the outside world. Resend fixes this in about ten minutes of Claude Code work.

**Get it:** [resend.com](https://resend.com)

---

### Twilio
**What it is:** SMS, WhatsApp, and voice API.
**Free tier:** Trial account with approximately £12 credit. Can only message verified phone numbers on the trial.
**After trial:** Pay-per-message, roughly 1p per SMS.

**What it unlocks:** SMS notifications, two-factor authentication, automated alerts. A sports fixture tracker that texts parents when a match is cancelled. A reminder system that nudges via text.

**Caveat:** The trial is limited to verified numbers only, so it's best for demos and prototypes. Real-world use requires a small ongoing cost.

**Get it:** [twilio.com](https://www.twilio.com)

---

## Maps and Location — Making Apps That Know Where Things Are

### Mapbox
**What it is:** Mapping platform with customisable maps, directions, geocoding, and search.
**Free tier:** 50,000 web map loads/month, 25,000 mobile active users, 100,000 directions API requests.

**What it unlocks:** Store/venue locators, travel planners, school campus maps, local event maps, delivery route visualisers, "things to do near me" apps, geography revision tools with real maps. Much more customisable than Google Maps.

**Why it matters:** Any project involving location becomes dramatically more impressive with a real map. The free tier is enormous — a school project will never come close to hitting it.

**Get it:** [mapbox.com](https://www.mapbox.com)

---

## Images and Media — Making Apps That Handle Photos

### Cloudinary
**What it is:** Image and video upload, storage, transformation, and delivery via CDN.
**Free tier:** 25 credits/month (covers storage, bandwidth, and transformations). No credit card required.

**What it unlocks:** Any project that handles user-uploaded photos — lost property systems, portfolio sites, recipe apps, plant identifiers, profile pictures. Automatic resizing, format conversion, cropping. AI features like auto-tagging and background removal.

**Why it matters:** Handling image uploads properly is surprisingly hard. Cloudinary makes it trivial. Upload via API, get back a URL that serves an optimised image.

**Get it:** [cloudinary.com](https://cloudinary.com)

---

## Browser APIs — Free, No Setup, No Account Needed

These are built into every modern browser. No API key, no account, no cost. Most students (and most developers) don't know they exist.

### Web Speech API
**What it does:** Speech-to-text and text-to-speech in the browser.
**Works in:** Chrome (best support), Edge, Safari (partial).

**What it unlocks:** Voice-controlled apps, apps that read content aloud, dictation tools, accessibility features. Build a revision tool that reads questions aloud and accepts spoken answers.

---

### Web Audio API
**What it does:** Audio synthesis, processing, and analysis directly in the browser.
**Works in:** All modern browsers.

**What it unlocks:** Browser-based synthesisers, audio visualisers, effects processors, audio analysis tools, beat makers, tone generators. Particularly relevant for music technology students.

---

### Canvas / WebGL
**What it does:** 2D and 3D drawing, animation, and data visualisation.
**Works in:** All modern browsers. p5.js makes Canvas much more approachable.

**What it unlocks:** Data visualisation, simple games, interactive graphics, generative art, diagram tools.

---

### Geolocation API
**What it does:** Gets the user's GPS coordinates (with their permission).
**Works in:** All modern browsers.

**What it unlocks:** Location-aware apps. Combine with Mapbox for "what's near me" features, automatic location tagging, distance calculations.

---

### Camera / MediaDevices API
**What it does:** Access the device camera for photo capture, video recording, or barcode scanning.
**Works in:** All modern browsers (requires HTTPS).

**What it unlocks:** Photo capture for identification projects (combine with Gemini), barcode scanning, video recording, document scanning. The bridge between the physical and digital.

---

### Web Bluetooth / Web USB
**What it does:** Connect to physical devices (like micro:bits) from a web app.
**Works in:** Chrome, Edge.

**What it unlocks:** If the school has micro:bits gathering dust (most do), students can read sensor data directly into a web app. Temperature, light level, accelerometer data — all piped into a dashboard.

---

## Data and Automation — Making Apps That Do Things on Their Own

### GitHub Actions
**What it is:** Automated workflows that run on GitHub's servers.
**Free tier:** 2,000 minutes/month for private repos, unlimited for public repos.

**What it unlocks:** Automated testing, scheduled tasks, deployment pipelines. A script that runs every morning to compile a daily digest. A workflow that checks a website for changes.

---

### Cron-job.org
**What it is:** Free service that hits a URL on a schedule.
**Free tier:** Unlimited cron jobs.

**What it unlocks:** Combined with a Supabase edge function, students can build apps that do things automatically. Send a daily email digest, check for price changes, compile a weekly report. Anything that needs to happen on a cycle without someone pressing a button.

**Get it:** [cron-job.org](https://cron-job.org)

---

## Hardware — Making Digital Things Physical

### Raspberry Pi
**Cost:** £30–60 depending on model (one-off purchase).

**What it unlocks:** A Pi running a web server on the school network could power a digital noticeboard, a sensor dashboard, or a school radio stream. Claude Code can build the software side quickly.

**Note:** This is the only item on this list that costs real money upfront.

---

### Micro:bits (the school probably already owns)
**Cost:** Free (they're in a cupboard somewhere).

**What it unlocks:** Via Web Bluetooth, students can read sensor data into a web app. Temperature monitoring, light levels, movement detection — all feeding into a live dashboard.

---

## The Full Stack at a Glance

| Category | Tool | Free Tier | Account Needed? |
|----------|------|-----------|----------------|
| Build | Claude Code | With subscription | Yes |
| Database | Supabase | Generous | Yes |
| AI | Google AI Studio | Free | Yes (Google account) |
| Deploy | Vercel | Unlimited deploys | Yes |
| Code hosting | GitHub | Unlimited repos | Yes |
| Email | Resend | 3,000/month | Yes |
| SMS | Twilio | ~£12 trial credit | Yes |
| Maps | Mapbox | 50,000 loads/month | Yes |
| Images | Cloudinary | 25 credits/month | Yes |
| Voice | Web Speech API | Unlimited | No |
| Audio | Web Audio API | Unlimited | No |
| Drawing | Canvas / p5.js | Unlimited | No |
| Location | Geolocation API | Unlimited | No |
| Camera | MediaDevices API | Unlimited | No |
| Hardware bridge | Web Bluetooth | Unlimited | No |
| Automation | GitHub Actions | 2,000 mins/month | Yes (GitHub) |
| Scheduling | Cron-job.org | Unlimited | Yes |
| Physical computing | Raspberry Pi | ~£35 one-off | No |

Most startups in 2024 were paying hundreds per month for less capability than this. Your students can access the entire stack for nothing.
