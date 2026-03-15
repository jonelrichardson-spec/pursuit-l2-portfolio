# 📁 My L2 Portfolio - Jonel Richardson

Hi, I'm Jonel. I spent 10 years as a preschool teacher, including 8 years in Japan, and now I'm building AI-powered applications as an AI-Native Builder at [Pursuit Fellowship](https://www.pursuit.org/) (Sept 2025–May 2026).

My background in education shapes how I approach building: I care about clarity, accessibility, and designing for real people. I'm drawn to civic infrastructure problems. I want to build tools that surface invisible issues, create accountability through data, and help systems work better for vulnerable populations.

This repo is a collection of my L2 projects, built during Pursuit's collaborative development module. Each project involved branching workflows, code reviews, and shipping alongside teammates.

---

## 🗂 Projects

---

### 🌨 Snowed-In MTA Bus Stops
**Team:** Carolina, Jawad, Dawn, Kelvin | **Built:** January 2026

NYC's 311 system is reactive. A bus stop has to be reported as blocked before anyone responds, and during winter storms, that delay hits elderly riders and people with disabilities hardest. We built an AI tool that uses existing NYC DOT traffic camera feeds to automatically detect snow-blocked bus stops and flag them for proactive clearing, so riders aren't stranded waiting for a response that hasn't been triggered yet.

The Claude API analyzes camera images near bus stop coordinates and returns a confidence score (clear / at risk / blocked). Results surface on a map interface for transit operators or 311 dispatchers.

**Stack:** Next.js · Tailwind CSS · Claude API (vision) · MTA Bus Stop data · NYC DOT camera feeds  
**Live Demo:** [snowedinbusstop.netlify.app](https://snowedinbusstop.netlify.app/) | **Repo:** [jonelrichardson-spec/SnowedInMTABusStop](https://github.com/jonelrichardson-spec/SnowedInMTABusStop)

---

### 🍷 Vivino Clone
**Team:** Luba | **Built:** February 2026

A pixel-perfect clone of the Vivino wine app featuring a two-layer scrollable mobile architecture. Replicating Vivino's nested scroll behavior was the core technical challenge. The outer page and inner wine list panels needed to scroll independently, which took real care to get right.

Building this taught me how much design complexity hides inside interfaces that feel simple to use. Getting the scrollable layout right required careful attention to CSS overflow behavior, fixed vs. relative positioning, and how scroll events propagate through nested containers.

**Stack:** React · Vite · Tailwind CSS  
**Live Demo:** [lubakaper.github.io/VivinoVersion2](https://lubakaper.github.io/VivinoVersion2/#/shop) | **Repo:** [jonelrichardson-spec/vivino-clone](https://github.com/jonelrichardson-spec/vivino-clone)

---

### 🛍 Too Good To Go Clone
**Team:** Victor | **Built:** February 2026

A pixel-perfect desktop clone of the Too Good To Go mobile app, plus a new feature we designed: **dietary restriction badges** on store listings. The original app gives users with dietary needs (vegan, gluten-free, nut-free, halal, kosher) no way to preview what's in a surprise bag before purchasing. Our feature adds color-coded dietary badges sourced from store menu data and a filter on the browse view.

We reviewed NYC Health Code §81.49 allergen disclosure requirements to ground the feature in what restaurants already disclose, so the data sourcing was realistic, not hypothetical. The clone exercise itself was about close attention to UI details: spacing, hierarchy, component reuse, and adapting a mobile-first layout to desktop.

**Stack:** React · Vite · Tailwind CSS · localStorage  
**Live Demo:** [toogoodtogo.netlify.app](https://toogoodtogo.netlify.app/) | **Repo:** [jonelrichardson-spec/toogoodtogo](https://github.com/jonelrichardson-spec/toogoodtogo)

---

### 📹 Zoom Clone
**Team:** Gary (backend) | **Built:** February 2026

A 1-to-1 browser-based video calling app using WebRTC. Users create or join a room and connect via live audio and video. I built the entire frontend: room creation/join flow, video grid layout, mute/camera controls, and Socket.io client integration.

The trickiest part was understanding the WebRTC event sequence: signaling must complete before the peer connection opens, and the peer connection must open before media streams attach. Getting the order wrong causes silent failures. PeerJS abstracts the handshake without hiding how it works; Socket.io handles the signaling server that makes peer discovery possible even in a "peer-to-peer" setup.

**Stack:** Next.js 14 · TypeScript · Tailwind CSS · PeerJS · Socket.io · Node.js · Railway  
**Live Demo:** [zoom-clone-beta-henna.vercel.app](https://zoom-clone-beta-henna.vercel.app/room/719251ee) | **Repo:** [jonelrichardson-spec/zoom-clone](https://github.com/jonelrichardson-spec/zoom-clone)

---

### 🌬 AeroStress: Wind Turbine Predictive Maintenance Platform
**Team:** Pape (backend), Jagger (PDF reports) | **Built:** Spring 2026 (MVP Complete)

A predictive maintenance platform for wind turbines that calculates **True Age**: how much a turbine has actually aged relative to its calendar age, based on IEC 61400-1 terrain stress multipliers. A turbine on a flat plain and one on a ridge may be the same calendar age, but the ridge turbine has been under significantly more stress. AeroStress makes that difference visible and actionable.

I was the frontend lead, building the Next.js dashboard and Expo mobile app. Delivered features include: a Mapbox stress heatmap with SDF triangle markers and terrain filters, a turbine detail page with True Age breakdown, inspection CRUD with photo upload, and PDF report download. The backend is a FastAPI/Python service with 500 seeded turbines and PostGIS for geospatial queries.

**Stack:** Next.js 16 · Tailwind CSS v4 · Zustand · Mapbox GL JS · Expo · FastAPI · Supabase/PostGIS  
**Live Demo:** [Add link here] | **Repo:** [jonelrichardson-spec/AeroStress](https://github.com/jonelrichardson-spec/AeroStress)

---

### 🗂 Cold Case Cluster Finder
**Team:** Manny (backend/data engineering) | **Built:** Spring 2026 (Capstone)

The FBI's Supplemental Homicide Reports contain nearly 900,000 records of unsolved homicides dating back to 1976, but that data has never been easy to explore geographically. I built the full frontend for a data journalism and law enforcement intelligence tool that clusters unsolved cases on an interactive map, so investigators and journalists can surface patterns that are invisible in a spreadsheet.

The dashboard includes custom filtering, a drag-resizable case detail panel, Mapbox cluster animations, and an Insights page that contextualizes the data. I owned all 7 build phases from landing page through E2E testing, with 189 passing tests and a type-check clean codebase at Demo Day.

**Stack:** Next.js · Tailwind CSS v4 · Zustand · Mapbox GL JS  
**Live Demo:** [cold-case-flame.vercel.app](https://cold-case-flame.vercel.app/) | **Repo:** [OasisView/cold-case](https://github.com/OasisView/cold-case)

---

## 🛠 Tech I Work With

**Frontend:** React · Next.js · Vite · Tailwind CSS · TypeScript  
**State:** Zustand · localStorage  
**APIs & AI:** Claude API · MTA APIs · Mapbox GL JS · PeerJS (WebRTC)  
**Backend (learning):** Node.js · Express · FastAPI · Socket.io  
**Tools:** Git/GitHub · Vercel · Railway · Claude Code

---

## 🔗 Connect

- **LinkedIn:** [jonel-richardson-09a399382](https://www.linkedin.com/in/jonel-richardson-09a399382)
- **Pursuit Fellowship:** [pursuit.org](https://www.pursuit.org/)
