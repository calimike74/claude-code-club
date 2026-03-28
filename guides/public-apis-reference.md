# Public APIs Reference — Claude Code Club

*Compiled from [public-apis/public-apis](https://github.com/public-apis/public-apis)*

---

## Quick Start: No-Auth APIs (Copy-Paste Ready)

Every one of these works with a bare `fetch()` call — no keys, no registration:

```
Open Trivia DB     https://opentdb.com/api.php?amount=10
PoetryDB           https://poetrydb.org/random
Datamuse           https://api.datamuse.com/words?rel_rhy=code
Open-Meteo         https://api.open-meteo.com/v1/forecast?latitude=51.5&longitude=-0.1&current_weather=true
Deck of Cards      https://deckofcardsapi.com/api/deck/new/shuffle/
JokeAPI            https://v2.jokeapi.dev/joke/Programming?safe-mode
JSONPlaceholder    https://jsonplaceholder.typicode.com/posts
xkcd               https://xkcd.com/info.0.json
Free Dictionary    https://api.dictionaryapi.dev/api/v2/entries/en/algorithm
Sunrise/Sunset     https://api.sunrise-sunset.org/json?lat=51.5&lng=-0.1
UK Carbon          https://api.carbonintensity.org.uk/intensity
Website Carbon     https://api.websitecarbon.com/site?url=google.com
Frankfurter        https://api.frankfurter.app/latest
MusicBrainz        https://musicbrainz.org/ws/2/artist/?query=radiohead&fmt=json
Lyrics.ovh         https://api.lyrics.ovh/v1/coldplay/yellow
Radio Browser      https://de1.api.radio-browser.info/json/stations/byname/bbc
CoinGecko          https://api.coingecko.com/api/v3/simple/price?ids=bitcoin&vs_currencies=gbp
Econdb             https://www.econdb.com/api/series/?search=GDP
UK Parliament      https://members-api.parliament.uk/api/Members/Search?Name=
UK Bank Holidays   https://www.gov.uk/bank-holidays.json
```

---

## Music APIs

### Best for Teaching (A-Level Music Technology)

| API | Auth | Why It Matters |
|-----|------|----------------|
| **Freesound** | OAuth | CC-licensed audio samples — compression examples, synthesis types, EQ demos. Could feed SRS wrong-answer deep links |
| **Spotify Web API** | OAuth | Audio Features endpoint returns BPM, key, loudness, energy per track — "blind analysis" quizzes |
| **MusicBrainz** | None | Open music encyclopedia — artists, recordings, releases. Zero auth for classroom demos |
| **Radio Browser** | None | Internet radio stations worldwide. No auth + CORS = works directly from browser JS |
| **TheAudioDB** | apiKey | Album art and metadata for visually rich topic cards |

### Best for Student Projects

| API | Auth | Project Idea |
|-----|------|-------------|
| **Lyrics.ovh** | None | Lyrics finder — simplest possible first API project (one endpoint) |
| **Genrenator** | None | Random music genre generator — fun warm-up activity |
| **iTunes Search** | None | Music search app — rich results, good for building a search interface |
| **Songsterr** | None | Guitar/bass tabs — students who play instruments will love this |
| **MusicBrainz** | None | "Music Connections" explorer — how artists, recordings, and labels relate |
| **Radio Browser** | None | "World Music Radio" app — buildable in a single lesson |

### Full Music API List (33 total)

| API | Description | Auth | HTTPS |
|-----|-------------|------|-------|
| 7digital | Music store | OAuth | Yes |
| AI Mastering | Automated music mastering | apiKey | Yes |
| Audiomack | Streaming music hub | OAuth | Yes |
| Bandcamp | Music community and streaming | OAuth | Yes |
| Bandsintown | Music events | None | Yes |
| Deezer | Music streaming service | OAuth | Yes |
| Discogs | Music database (artists, labels, releases) | OAuth | Yes |
| Freesound | Music samples and sound effects | OAuth | Yes |
| Gaana | Song information | None | Yes |
| Genius | Crowdsourced lyrics and music knowledge | OAuth | Yes |
| Genrenator | Music genre generator | None | Yes |
| iTunes Search | Search iTunes catalogue | None | Yes |
| Jamendo | Creative Commons licensed music | OAuth | Yes |
| JioSaavn | Song information and album metadata | None | Yes |
| KSoft.Si | Lyrics database (aimed at Discord bots) | apiKey | Yes |
| Last.fm | Music scrobbling, metadata, recommendations | apiKey | Yes |
| ListenBrainz | Open music listening history | apiKey | Yes |
| Lyrics.ovh | Simple lyrics retrieval | None | Yes |
| Mixcloud | DJ mixes, radio shows, podcasts | OAuth | Yes |
| MusicBrainz | Open music encyclopedia | None | Yes |
| Musixmatch | Lyrics database (millions of songs) | apiKey | Yes |
| Napster | Music streaming service | apiKey | Yes |
| Openwhyd | Curated playlists of streaming tracks | None | Yes |
| Radio Browser | Internet radio stations worldwide | None | Yes |
| Shazam | Music recognition from audio | apiKey | Yes |
| Songkick | Live music events (6M+ concerts) | OAuth | Yes |
| Songsterr | Guitar, bass and drums tabs | None | Yes |
| SoundCloud | Sound recording and sharing | OAuth | Yes |
| Spotify | Music catalog, recommendations, playback | OAuth | Yes |
| TasteDive | Similar music/film recommendations | apiKey | Yes |
| TheAudioDB | Community music database with artwork | apiKey | No |
| Tidal | Lossless hi-fi streaming | OAuth | Yes |
| Vagalume | Crowdsourced lyrics (Portuguese focus) | apiKey | Yes |

---

## Finance APIs

### Top Picks for Club

| API | Auth | Best For | Project Idea |
|-----|------|---------|-------------|
| **CoinGecko** | None | First API project | Crypto dashboard — top 100 coins by market cap |
| **Alpha Vantage** | apiKey (free) | All-rounder | Stock tracker, currency converter, moving average analysis |
| **Aletheia** | apiKey (free) | Congressional trading | Insider trade dashboard, politician trade timeline |
| **SEC EDGAR** | None | Government transparency | Parse financial disclosures, track institutional holdings |
| **FRED** | apiKey (free) | Economics education | UK vs US economy comparison, inflation calculator |
| **Econdb** | None | Global economics | "Brexit Effect" dashboard — UK indicators pre/post 2016 |
| **WallstreetBets** | None | Student engagement | Reddit sentiment vs actual stock performance |
| **Frankfurter** | None | Currency/economics | "Brexit pound tracker" — GBP vs EUR since 2016 |
| **Portfolio Optimizer** | None | Maths crossover | Build a robo-advisor, diversification demo |
| **Finnhub** | apiKey (free) | Real-time data | Live stock ticker via WebSocket, ESG scoring tool |

### Best Pairings

| Goal | Primary | Supporting |
|------|---------|-----------|
| Congressional trading analysis | Aletheia + SEC EDGAR | Alpha Vantage (prices), Finnhub (news) |
| First-ever API project | CoinGecko (no auth) | Econdb, Frankfurter |
| Economics/financial literacy | FRED + Econdb | Fed Treasury, Alpha Vantage |
| Most "wow factor" | WallstreetBets + Alpha Vantage | CoinGecko, Finnhub |
| Maths crossover | Portfolio Optimizer | Alpha Vantage, CoinGecko |

---

## Government & News APIs

### UK-Specific APIs (flagged)

| API | Auth | Description |
|-----|------|-------------|
| **UK Parliament** | None | Written questions, bills, debates, voting records |
| **The Guardian** | apiKey (free) | UK newspaper content — 5,000 calls/day free tier |
| **UK Bank Holidays** | None | Single JSON endpoint — perfect first API project |
| **UK Carbon Intensity** | None | Real-time British electricity grid carbon data |
| **National Grid ESO** | None | UK electricity generation by type (wind, solar, gas) |
| **Open Government UK** | None | Portal to thousands of UK government datasets |
| **Reed** | apiKey | UK job listings |

### News APIs

| API | Auth | Description |
|-----|------|-------------|
| **NewsAPI** | apiKey (free) | 80,000+ sources worldwide — media literacy projects |
| **The Guardian** | apiKey (free) | UK news with structured metadata |
| **GNews** | apiKey (free) | Search news from any country/language |
| **Inshorts** | None | Short news summaries |

### Best Combination Projects

| Combination | Project | Cross-Curricular |
|-------------|---------|-----------------|
| UK Parliament + Guardian | "Democracy Dashboard" — Parliament debates vs media coverage | Politics, Media Studies |
| UK Carbon + National Grid | "Green Britain Tracker" — energy + carbon visualisation | Geography, Physics |
| Econdb + Frankfurter + NewsAPI | "Brexit Impact Monitor" — economics + exchange rates + news | Economics, Business, Politics |
| NewsAPI + Guardian | "Media Literacy Lab" — compare framing across sources | Media Studies, English |

---

## Hidden Gems (Best for Engagement)

### Top 15 — Ranked by Student Appeal

| # | API | Auth | One-Line Pitch | Project Idea |
|---|-----|------|---------------|-------------|
| 1 | **Open Trivia DB** | None | Trivia questions by category/difficulty | Quiz app with score tracking |
| 2 | **PoetryDB** | None | Search classic poetry by author/keyword | "Poem of the day" generator |
| 3 | **Datamuse** | None | Words that rhyme/mean/sound-like | Rhyme finder, creative writing tool |
| 4 | **Open-Meteo** | None | Global weather (current + forecast + historical) | Weather dashboard with Chart.js |
| 5 | **UK Carbon Intensity** | None | Real-time GB electricity grid carbon | "When to charge your phone" app |
| 6 | **Sunrise/Sunset** | None | Golden hour times for any location | Photography calculator |
| 7 | **Deck of Cards** | None | Virtual deck with card images | Blackjack game, probability simulator |
| 8 | **JokeAPI** | None | Jokes with content filters | Discord bot, joke-of-the-day |
| 9 | **JSONPlaceholder** | None | Fake REST API (full CRUD) | Training ground for learning REST |
| 10 | **Pixela** | apiKey (free) | GitHub-style contribution heatmaps | Personal habit tracker |
| 11 | **xkcd** | None | Comic data as JSON | Random xkcd viewer |
| 12 | **Free Dictionary** | None | Definitions with audio pronunciation | Vocabulary builder (speaks!) |
| 13 | **Frankfurter** | None | ECB exchange rates since 1999 | Currency converter, GBP tracker |
| 14 | **Wger** | None | Exercise database with muscle diagrams | Workout planner |
| 15 | **Website Carbon** | None | Carbon footprint of any webpage | "Greenest website" competition |

### Honourable Mentions

| API | Auth | Best For |
|-----|------|---------|
| Rick and Morty | None | Fun first fetch project |
| PokeAPI | None | Great docs, huge dataset |
| Chess.com | None | Chess club crossover |
| FunTranslations | None | Yoda/Pirate/Shakespeare translator |
| HTTP Cat / HTTP Dog | None | Teaching HTTP status codes with humour |
| Colormind | None | AI-generated colour schemes for design |
| Nager.Date | None | Public holidays for 90+ countries |

---

## Suggested Learning Progression

### Phase 1: First API Call (Sessions 4-5)
Start with zero-auth APIs to learn `fetch()` and JSON rendering:
- **UK Bank Holidays** or **JokeAPI** — single endpoint, instant results
- **JSONPlaceholder** — learn full CRUD (GET, POST, PUT, DELETE)

### Phase 2: Real Data (Sessions 6-7)
Graduate to APIs that return meaningful, changing data:
- **Open-Meteo** or **UK Carbon Intensity** — real-time data + Chart.js visualisation
- **CoinGecko** or **Frankfurter** — financial data, still no auth

### Phase 3: Auth & Ambition (Sessions 8-10 / Demo Day)
Introduce API keys and more complex projects:
- **Alpha Vantage** or **The Guardian** — API key management
- **Aletheia + SEC EDGAR** — congressional trading tracker
- **Spotify** — audio analysis features
- **Freesound** — audio samples for Music Tech integration

### Phase 4: Multi-API Projects (Advanced/Ongoing)
Combine 2+ APIs for rich applications:
- Parliament + Guardian = Democracy Dashboard
- WallstreetBets + Alpha Vantage = Sentiment Tracker
- Datamuse + PoetryDB = Creative Writing Toolkit
- UK Carbon + National Grid = Green Britain Tracker

---

## Source

All APIs sourced from [github.com/public-apis/public-apis](https://github.com/public-apis/public-apis) — a community-maintained collection of free APIs for software and web development.
