# 01 — What to Build

## The Original Problem

Someone posted a list of 60+ "things to build" on Twitter. Operating systems, compilers, blockchain consensus algorithms, hypervisors, CPU emulators, kernel development in assembly. All completely inappropriate for sixth formers using Claude Code. Most of them are inappropriate for professional developers with five years' experience.

This document replaces that list with projects that are achievable, deployable, and solve real problems.

---

## Principles

- Every project should be **finishable** in a realistic timeframe (one session to a few weeks)
- Every project should be **deployable** — a URL someone can visit
- Every project should **solve a real problem** for a real person
- The question is never "what's technically impressive" — it's "what would someone actually use?"

---

## Level 1 — Single Session Builds

These can be started and deployed in one club session with Claude Code. Good for building confidence and establishing the build → deploy → share workflow.

### Split-the-Bill Calculator
A genuinely good one that handles "I didn't have a starter" and uneven splits. Everyone needs this. Sounds trivial, but making it work well with edge cases teaches real thinking.

### Personal Dashboard
One page showing timetable, next deadline, weather, and a quote. Becomes their homepage on every device. Teaches API integration basics.

### Habit Tracker
Daily check-ins, streaks, simple charts showing progress. Introduces data persistence via Supabase.

### Countdown Timer Collection
Exam countdowns, university offer deadlines, end of term. Shareable links so friends can see the same countdowns. Simple but immediately useful.

---

## Level 2 — School Problems That Need Solving

These take a few sessions and involve Supabase for data storage. Real users within the school.

### Revision Timetable Generator
Input subjects, exam dates, and free periods — get a study schedule. Deploy it and share it with the year group. Could incorporate spaced repetition logic.

### House/Team Points Tracker
Live leaderboard that updates from a simple form. Every school needs one and they're always ugly.

### "What's for Lunch" App
Weekly menu displayed nicely on a phone. Genuinely useful every single day. Could scrape or manually input the data.

### Study Group Finder
Post what you're revising, find others doing the same subject at the same time. A noticeboard with structure.

### Sports Fixture Tracker
Scores, results, league table, upcoming matches for a school team. The PE department will value this.

### Lost Property Board
Photo upload, description, claimed/unclaimed status. Simple database project with a real audience.

---

## Level 3 — Solve a Problem for Someone Else

These involve building for an external user or audience. Portfolio-worthy.

### Local Business Website
Find a real shop, café, or tradesperson near school with no website or a terrible one. Build them one. Real client, real portfolio piece, real reference.

### Charity Event Sign-Up Page
Next time a house or society runs something, build the registration and ticketing instead of using Google Forms. Real audience, real deadline.

### Community Event Aggregator
One page showing everything happening locally this week. Nobody does this well for small towns. Add Gemini to auto-categorise and summarise events.

### "Is This a Scam?" Checker
Paste in a suspicious email or text, Gemini analyses it for red flags. Particularly useful for elderly relatives. A student could build this and give it to their grandparents.

### Local Tradesperson Review Platform
Hyper-local Trustpilot. Reviews in Supabase, Gemini summarises sentiment. Small towns don't have enough critical mass for the big platforms.

---

## Level 4 — AI-Powered Projects (Using Gemini via Google AI Studio)

These combine the full stack: Claude Code to build, Supabase to store, Gemini to think.

### AI-Powered Lost Property System
Photograph a lost item, Gemini identifies and tags it automatically (blue jacket, Nike, size M), Supabase stores it with location and date. Search by description instead of rummaging through a bin bag.

### Smart Noticeboard
Societies and staff post announcements into Supabase. Gemini auto-categorises and summarises. Students see a personalised feed of relevant items.

### Exam Question Bank with AI Marking
Teachers upload past paper questions to Supabase. Students answer them, Gemini marks against the mark scheme with structured feedback. Track progress over time.

### "What Should I Read Next" Engine
Scan a book cover with a phone camera, Gemini identifies it, Supabase stores reading history, AI recommends the next book based on patterns. Built for the school library.

### Recipe App From What You Actually Have
Photograph fridge contents, Gemini identifies ingredients, suggests recipes, Supabase stores dietary preferences and past meals.

### Plant Identifier and Care Tracker
Photograph a plant, Gemini identifies it and gives care instructions, Supabase tracks the collection with watering schedules and notifications.

### Debate Prep Tool
Enter a motion, Gemini generates arguments for and against with source suggestions, Supabase stores debate history.

### Art Portfolio with AI Critique
Upload artwork, Gemini offers structured feedback on composition and technique. Supabase stores the portfolio with progression over time.

---

## Level 5 — Projects the Business and Economics Students Will Love

These apply real business thinking and could genuinely become something.

### Micro-Business Launchpad
Supabase handles product listings, customer accounts, order tracking. Gemini generates product descriptions from photos and handles customer service chat. A student could launch a small online business in a week.

### Market Research Tool
Design a survey, store responses in Supabase, Gemini analyses open-text responses for themes and sentiment, generates charts and a summary report.

### Personal Finance AI Advisor
Log transactions in Supabase, Gemini categorises spending, spots patterns, gives plain-English advice. Economics concepts made tangible.

### Simple CRM for a School Society or Charity
Track donors, volunteers, or members in Supabase. Gemini drafts personalised thank-you emails, generates engagement reports.

### Price Comparison Tracker
Log prices from local shops over time, Gemini identifies trends, predicts when things get cheaper. Microeconomics made visible.

---

## Level 6 — "This Could Actually Become Something"

Ambitious but achievable. These would make a strong portfolio piece or even a real product.

### Specification-Mapped Revision Platform
Pick an exam board and subject, Supabase stores the spec points, Gemini generates targeted questions for each one, tracks confidence across the specification.

### Parents' Evening Booking System
Parents pick preferred teachers, Supabase handles scheduling, Gemini optimises the timetable to minimise gaps and conflicts. Every school pays for a clunky version of this.

### UCAS Personal Statement Workshop
Supabase stores drafts and feedback history, Gemini gives structured critique against what admissions tutors look for, tracks improvement across versions. Not writing it for them — coaching them through it.

### Mock Election Voting System
Anonymous ballots, live results, proper authentication so nobody votes twice. Timely and impressive.

### Quiz Platform for Teachers
A teacher creates a quiz, students take it on their phones, results appear on screen. A simple Kahoot clone.

### Accessibility Auditor
Paste in a website URL, Gemini analyses content for accessibility issues, Supabase tracks fixes over time. Offer it to school societies, then to local businesses.

---

## Creative and Cultural Projects

### School History Archive
Photograph old documents, trophies, programmes. Gemini transcribes and describes them, Supabase stores everything searchable. A living digital museum.

### Songwriting Collaborator
Write lyrics, Gemini suggests chord progressions, rhyme alternatives, structural feedback. Supabase stores drafts with version history.

### Language Exchange Matchmaker
Supabase stores who speaks what and who's learning what. Gemini facilitates practice conversations and corrects grammar.

### Music Recommendation Journal
Log what you're listening to, rate it, tag moods, get a wrapped-style summary. More interesting than Spotify's.

---

## Choosing a Project

The best project is the one that solves a problem the student actually has. Before picking from this list, ask them:

1. What annoys you about how something works at school?
2. What do you wish existed on your phone?
3. Is there a small business near you that could use help?
4. What would you show off to your mates?

If the answer to any of those points at a project on this list, that's the one. If it points at something not on this list, even better.
