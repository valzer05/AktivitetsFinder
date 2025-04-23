AktivitetsFinder

Aggregator of kid‑friendly activities across Denmark, built with Next.js & Supabase

🚀 Product Vision

A single, intuitive hub where parents in Denmark (kids 0‑18 y/o) can discover the best activities in their city and jump straight to the organiser’s booking page.  Filters for city, child age and price range plus an AI helper that suggests the ideal activity.

🥇 MVP Scope

Live activity list refreshed nightly.

Filters – city · age · price.

Outbound click‑through to the provider’s landing page.

🏗️ Tech Stack (v0)

Layer

Choice

Why

Front‑end + API

Next.js 14 App Router

SEO‑friendly SSR, file‑based routing, API routes.

Styling

Tailwind CSS

Rapid prototyping, utility‑first.

Database

Supabase (Postgres)

Free tier, SQL, auth, REST/GraphQL.

Crawler

Node script + Cheerio / playwright‑crawler

Lightweight scraping.

Hosting

Vercel Hobby

Auto‑deploy from GitHub.

🛠️ Getting Started (local)

# prerequisites: Node 20 LTS, npm, git installed

# clone the repo
 git clone https://github.com/<your‑user>/AktivitetsFinder.git
 cd AktivitetsFinder

# create the Next.js app (only once)
 npx create-next-app@latest web --typescript --eslint --tailwind --src-dir --app --import-alias "@/*"

# run locally
 cd web
 npm run dev
# visit http://localhost:3000

📂 Project Structure (after first commit)

AktivitetsFinder/
├─ web/            # Next.js front‑end & API routes
│  ├─ src/
│  └─ ...
├─ crawler/        # Node scrapers (MVP: one file per source)
├─ README.md
└─ .gitignore

🗺️ Roadmap (high level)

Phase 1 – Hello World skeleton & Supabase connection

Phase 2 – Crawler for 1 public data source

Phase 3 – Listing UI with filters

Phase 4 – Ads & Analytics

Phase 5 – Beta launch + user feedback

📜 Licence

MIT (to be confirmed)

