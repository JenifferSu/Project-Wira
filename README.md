# AI Disaster Resilience Platform

> A gamified, mobile-first AI disaster resilience platform designed for children and communities. The platform combines AI-powered interactive learning, augmented reality (AR), and AI real-time emergency support tools to help users understand disaster risks while also providing practical survival features during real emergencies.

---
## Demo Video
https://www.youtube.com/watch?v=9-Y7TCkZXbg

## Final Report
https://drive.google.com/file/d/1BvBxPdb5UqVc4Zdx0weThzLgVEW48YJn/view?usp=sharing


## What is This Platform?

The AI Disaster Resilience Platform is an **educational web application** that teaches disaster preparedness through **gamified learning experiences**. Designed specifically for the ASEAN region, it combines:

- **Real disaster data** from 10 ASEAN countries
- **Interactive AR-based training** for flood, earthquake, and other disasters
- **Emergency survival tools** that work offline (Possum Protocol)
- **Community-driven safety scores** (Village system)
- **Child-friendly design** with mascots, badges, and rewards

## 🌏 Background
 
Natural disasters — floods, storms, and landslides — occur frequently across ASEAN, with countries like Malaysia experiencing severe seasonal monsoon flooding. These events disproportionately affect vulnerable populations, especially rural communities and school-aged children who often lack the knowledge and tools to respond effectively.
 
Traditional disaster education fails because it is:
 
- 📖 **Lecture-based and forgettable** — passive content doesn't build muscle memory
- 😨 **Not designed for children** — complex language and scary imagery alienate younger audiences
- 📵 **Useless during actual disasters** — existing apps stop working when networks and power go down
- 🧩 **Fragmented** — no single platform combines education, immersive training, and real emergency tools
 
---
 
## 🎯 Problem Statement
 
> Communities in disaster-prone regions, particularly children, often lack accessible and engaging disaster preparedness education as well as reliable emergency communication tools that function during infrastructure failures such as power outages or network disruptions — making it difficult for them to respond safely and effectively during disasters such as floods, earthquakes, and severe storms.
 
---
 
## 🌱 SDG Alignment
 
| SDG | Contribution |
|---|---|
| **SDG 11** — Sustainable Cities & Communities *(Primary)* | Strengthens disaster preparedness and resilience through AI-powered education and emergency response tools |
| **SDG 4** — Quality Education *(Secondary)* | Delivers interactive, gamified digital learning that improves children's disaster safety knowledge |
| **SDG 13** — Climate Action *(Secondary)* | Raises awareness of climate-related disasters and promotes community preparedness across ASEAN |
 
---
 
## 💡 Solution Overview
 
**Project Wira** is a gamified, mobile-first AI disaster resilience platform that transforms passive disaster awareness into active, practised survival readiness. It is the first platform to unify all three pillars of disaster preparedness in a single child-friendly application:
 
```
┌─────────────────────────────────────────────────────────────────┐
│                        PROJECT WIRA                             │
├──────────────┬──────────────┬──────────────┬────────────────────┤
│  DASHBOARD   │    ATLAS     │  AR TRAINING │  POSSUM PROTOCOL   │
│  Home Base   │  Map & Risk  │  Simulation  │  Emergency Tools   │
│  AI Alerts   │  AI Data     │  Training    │  Offline AI Suite  │
│  Missions    │  Explorer    │  Practice    │  Mesh Network      │
└──────────────┴──────────────┴──────────────┴────────────────────┘
```
 
**The core learning loop:**
 
```
LEARN (Atlas)  →  TRAIN (AR Time Machine)  →  EARN (XP & Badges)
     ↑                                               ↓
     └──────────────────── REPEAT ──────────────────┘
                                  ↓
                        SURVIVE (Possum Protocol)
```
 
Unlike traditional platforms, Project Wira provides offline emergency functions — SOS alerts, GPS sharing, flashlight signalling, and AI-powered mesh communication — enabling users to seek help even when internet and power infrastructure fail.
 
---
 
## 🤖 AI Integration
 
AI is not a superficial layer in Project Wira — it is embedded as a continuous thread across every module, operating in two modes depending on connectivity.
 
### AI by Module
 
| Module | AI Component | What It Does |
|---|---|---|
| **Dashboard** | Threat Detection Engine | Ingests satellite, seismic & news feeds; generates probabilistic threat scores and pushes alerts *before* official warnings are issued |
| **Dashboard** | Adaptive Mission Recommender | Personalises daily mission queues based on user region, skill gaps, and training history |
| **Atlas** | Multi-Modal Risk Classifier | Dynamically updates SVG map markers with live AI-generated risk scores |
| **Atlas** | RAG Brief Generator | Assembles real-time country risk briefs from verified source documents — prevents hallucination in safety-critical outputs |
| **Atlas** | LSTM Forecast Model | Projects 30/60/90-day disaster probability trained on 30+ years of ASEAN data |
| **Atlas** | Anomaly Detection | Monitors sensor streams for statistical deviations that precede disasters |
| **AR Training** | RL Adaptive Difficulty Engine | Adjusts scenario complexity per user in real time based on performance telemetry |
| **AR Training** | AI Performance Coach | Generates personalised post-simulation debrief with targeted improvement recommendations |
| **Possum Protocol** | On-Device Audio CNN | Detects rescue whistle frequencies offline via quantised TensorFlow.js — no connectivity required |
| **Possum Protocol** | Mesh Route Neural Net | Graph neural network optimises P2P device relay topology for maximum offline coverage |
| **Possum Protocol** | AI Battery Governor | Regression model predicts remaining battery life and enforces hibernation to extend survival window |
| **Possum Protocol** | Offline LLM (<50MB) | Compressed on-device language model answers survival queries without any network connection |
| **UI Layer** | Stress-Adaptive Inference | Detects stress via touch pressure and gesture velocity; auto-simplifies UI during active emergencies |
 



---

### How The System Works

```mermaid
flowchart LR
    Start([Sign Up and Create Profile]) --> Learn[Learn About Disasters]
    Learn --> Practice[Practice via AR Training]
    Practice --> Earn{Earn XP and Badges}
    Earn --> LevelUp[Level Up]
    Earn --> Unlock[Unlock New Missions]
    LevelUp --> Return[Return to Dashboard]
    Unlock --> Return
    Return --> Practice
```

```mermaid
flowchart TD
    Dashboard[Dashboard - Home Base]
    Atlas[Atlas - Map Explorer]
    AR[AR Training - Simulation]
    Possum[Possum Protocol - Emergency Tools]

    Dashboard --> Atlas
    Dashboard --> AR
    Atlas --> XP[Earn XP]
    AR --> XP
    XP --> Dashboard
    Dashboard --> Possum
```

---

## Complete User Journey

### Phase 1: Getting Started

```mermaid
flowchart TD
    Launch([First Launch]) --> Welcome[Welcome Screen]
    Welcome --> Profile[Create Profile]
    Profile --> Tutorial[Mascot Introduction]
    Tutorial --> Dashboard[Enter Dashboard]
```

### Phase 2: Daily Usage Loop

```mermaid
flowchart TD
    Open([Open App]) --> Check[Check Dashboard]
    Check --> Select[Select Mission]
    Select --> Mission{Mission Type}

    Mission --> Complete[Complete Mission]
    Mission --> Learn[Learn Disaster History]

    Complete --> Progress[Progress Saved]
    Learn --> Progress

    Progress --> CheckReward{Reward Check}
    CheckReward -->|Level Up| LevelUp[Level Up]
    CheckReward -->|Badge Earned| Badge[Badge Unlocked]
    CheckReward -->|No Reward| Return([Return to Dashboard])

    LevelUp --> Return
    Badge --> Return
    Return --> Select
```

--

## Gamification System

### Progression Levels

```mermaid
timeline
    title Level Progression System
    Level 1 : Novice (0 XP) : Tutorial complete
    Level 2 : Explorer (500 XP) : 5 missions completed
    Level 3 : Scout (1000 XP) : 10 missions
    Level 4 : Ranger (1500 XP) : YOU ARE HERE
    Level 5 : Expert (2500 XP) : 40 missions
    Level 6 : Master (5000 XP) : All complete
```

### Badge Collection

```mermaid
graph TD
    subgraph Exploration["EXPLORATION BADGES"]
        Flood[Flood Explorer]
        Storm[Storm Spotter]
    end

    subgraph Training["TRAINING BADGES"]
        Drill[Drill Master]
        Night[Night Scout]
    end

    subgraph Community["COMMUNITY BADGES"]
        Hero[Village Hero]
    end

    Flood --> LevelUp[Level Up]
    Storm --> LevelUp
    Drill --> LevelUp
    Night --> LevelUp
    Hero --> LevelUp
```


## Technology Stack

### Frontend

| Technology | Purpose | Version |
|------------|---------|---------|
| **React** | UI Library | 18.3.1 |
| **Vite** | Build Tool | 6.3.5 |
| **TypeScript** | Type Safety | 5.x |
| **React Router** | Routing | 7.13.0 |
| **TailwindCSS** | Styling | 4.1.12 |
| **Radix UI** | Component Primitives | Various |
| **Motion** | Animations | 12.23.24 |
| **Recharts** | Data Visualization | 2.15.2 |



## Installation & Setup

### Prerequisites
- Node.js 18+ installed
- npm, yarn, or pnpm package manager

### Quick Start
Download github zipped file
Go to Terminal:

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```
Open `http://localhost:xxxx` in your browser

### Available Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server with hot reload |
| `npm run build` | Build for production (outputs to `/dist`) |

---

## Original Design

The original design is available at [Figma](https://www.figma.com/design/nXSyHFCcEQ4jQrXt7gQHWG/AI-Disaster-Resilience-Platform).
But we made some changes to the current one, so a bit different with final product.
---

## License

This project is part of the AI Disaster Resilience Platform initiative.

---

## Attribution

See [ATTRIBUTIONS.md](./ATTRIBUTIONS.md) for third-party licenses.

---

**Built for the ASEAN region. Designed to save lives.**

*Version 1.0.0 | Last Updated: 2026-03-12*
