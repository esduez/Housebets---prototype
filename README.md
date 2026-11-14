# Housebets Sportsbook — Prototype

A front-end-only sportsbook prototype built for the Housebets Challenge. Mobile-first (390px) and desktop-ready (1440px), with a fully working bet slip, live match simulation, and team following.

## 🚀 Live Demo
**[https://esduezz.github.io/Housebets/](https://esduezz.github.io/Housebets/)** 
## 📦 Tech Stack
- HTML5 / Vanilla JS / CSS3 (Single-file architecture)
- Tailwind CSS (CDN)
- Google Fonts (Inter + Poppins)
- GitHub Pages (Hosting)
- Claude (Anthropic) — Code & Copy Assistant

## 🏗️ Architecture

```text
┌───────────────────────────────────────────┐
│              BROWSER (CLIENT)             │
│                                            │
│  ┌──────────┐   ┌────────┐   ┌──────────┐ │
│  │ Mock     │──▶│ State  │──▶│ Render   │ │
│  │ Data     │   │ (slip, │   │ (DOM)    │ │
│  │          │   │  bets) │   │          │ │
│  └──────────┘   └────────┘   └──────────┘ │
│        ▲             │             │       │
│        │             ▼             ▼       │
│  ┌──────────┐   ┌────────┐   ┌──────────┐ │
│  │ Stats    │   │ Bet    │   │ Live     │ │
│  │ Engine   │   │ Slip   │   │ Sim      │ │
│  └──────────┘   └────────┘   └──────────┘ │
└───────────────────────────────────────────┘
                    │
                    ▼
         ┌─────────────────────┐
         │  GitHub Pages (CDN) │
         └─────────────────────┘
