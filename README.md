# Learning OS – 520-Hour Engineering Roadmap

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Built with Vite](https://img.shields.io/badge/Vite-5.x-646CFF.svg?logo=vite&logoColor=white)](https://vitejs.dev/)
[![Stack: Vanilla JS](https://img.shields.io/badge/Frontend-Vanilla%20JavaScript-F7DF1E.svg?logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Deploy to GitHub Pages](https://github.com/vishnukumar001/learning-os-520-hour-roadmap/actions/workflows/deploy.yml/badge.svg)](https://github.com/vishnukumar001/learning-os-520-hour-roadmap/actions/workflows/deploy.yml)
[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-2ea44f.svg?logo=github&logoColor=white)](https://vishnukumar001.github.io/learning-os-520-hour-roadmap/)

A personal engineering command center designed to track, measure, and navigate an intensive **520-hour curriculum** spanning **AI Automation & Agent Engineering**, **Cybersecurity Engineering**, and **Production-Ready Capstone Projects**.

Designed with a zero-framework, privacy-first philosophy: 100% client-side, zero external telemetry, instant startup, and zero backend maintenance.

---

## Table of Contents

- [Overview](#overview)
- [Curriculum Breakdown](#curriculum-breakdown)
- [Key Features](#key-features)
- [Technology Stack](#technology-stack)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Local Development](#local-development)
  - [Production Build](#production-build)
  - [Preview Build](#preview-build)
- [Data Storage & Privacy](#data-storage--privacy)
  - [Storage Model](#storage-model)
  - [Backup & Migration](#backup--migration)
- [Deployment](#deployment)
  - [Deploy to Vercel (Recommended)](#deploy-to-vercel-recommended)
  - [Deploy to GitHub Pages](#deploy-to-github-pages)
  - [Deploy to Netlify](#deploy-to-netlify)
- [Contributing & Customization](#contributing--customization)
- [License](#license)

---

## Overview

Self-directed technical education often fails due to fragmented notes, lack of verifiable evidence of mastery, and unclear progress tracking. **Learning OS** solves this by combining:

1. **A Structured 520-Hour Syllabus**: High-leverage skills categorized into concrete modules, topics, and real-world deliverables.
2. **Evidence-Gated Mastery**: Topics require real evidence (code repositories, pull requests, deployed links, lab write-ups) before being marked complete.
3. **Execution Dashboard**: Real-time progress metrics, milestone achievements, streak tracking, and active study session timers.

---

## Curriculum Breakdown

The 520 hours are systematically allocated across three major engineering tracks:

```
Total Hours: 520 Hours
├── Track A: AI Automation & Agent Engineering (340 Hours)
│   ├── Module 1: Programming & Technical Fundamentals (40h)
│   ├── Module 2: API & Integration Engineering (41h)
│   ├── Module 3: n8n Automation Engineering (35h)
│   ├── Module 4: Database Engineering (30h)
│   ├── Module 5: AI & LLM Engineering (45h)
│   ├── Module 6: AI Agent Engineering (55h)
│   ├── Module 7: WhatsApp & Business Automation (24h)
│   ├── Module 8: Backend Engineering (38h)
│   └── Module 9: Production & Deployment (32h)
│
├── Track B: Cybersecurity Engineering (125 Hours)
│   ├── Module 10: Cybersecurity Fundamentals (59h)
│   ├── Module 11: Web & API Security Engineering (45h)
│   └── Module 12: AI & Automation Security (21h)
│
└── Track C: Final Practical Projects (55 Hours)
    ├── Capstone 1: Enterprise Multi-Agent Business Workflow
    ├── Capstone 2: Production WhatsApp AI Support System
    └── Capstone 3: Security-Hardened API with Vulnerability Audit
```

---

## Key Features

- **Evidence-Gated Topic Completion**: Rather than simple checkboxes, topics enforce accountability by accepting evidence URLs and verification notes.
- **Built-in Study Session Timer**: Integrated live stopwatch and manual session logger categorized by module and practical vs. theoretical focus.
- **Milestones & Achievements**: Automatically unlocks achievements as milestone thresholds (e.g., first module, streak targets, 100h milestone) are met.
- **Project Command Center**: Track deliverables, GitHub repositories, live demo URLs, tech stacks, and individual checklist tasks.
- **Module Notes Hub**: Markdown-friendly notes management linked directly to roadmap modules.
- **Curated Technical Resources**: Direct links to documentation and learning materials (n8n, FastAPI, OWASP, PortSwigger, TryHackMe, Hugging Face).
- **Comprehensive Analytics**: Visual breakdown of total hours completed, remaining hours, track ratios, active streaks, and extra learning hours logged.
- **Dark & Light Mode**: Seamless theme switching with OS color scheme detection and persistence.
- **Zero-Backend Privacy**: 100% of data lives locally in your browser's `localStorage`. No accounts, no database keys, and no telemetry.
- **Portable JSON Backup**: One-click JSON backup export and import to transfer study state between browsers or devices.

---

## Technology Stack

- **Core Runtime**: Vanilla JavaScript (ES Modules, modern DOM APIs, no heavy framework dependencies)
- **Styling**: Native CSS3 with CSS Custom Properties (design tokens for typography, spacing, and theme variables)
- **Tooling & Bundler**: [Vite 5](https://vitejs.dev/) for instant HMR and optimized production assets
- **Deployment Target**: Any static host (Vercel, Netlify, GitHub Pages, Cloudflare Pages)

---

## Project Structure

```
learning-os-520-hour-roadmap/
├── index.html          # HTML entry point, theme bootstrapper & web fonts
├── package.json        # Project metadata and build scripts
├── vite.config.js      # Vite build configuration (base path and outDir)
├── vercel.json         # Vercel deployment routing configuration
├── .gitignore          # Git exclusion rules for node_modules, build, secrets
├── public/
│   └── favicon.svg     # Modern SVG favicon
└── src/
    ├── main.js         # Core application logic, data models, router, components
    └── styles.css      # CSS styling, variables, layout, responsive design
```

---

## Getting Started

### Prerequisites

- **Node.js**: `v18.0.0` or higher ([Download Node.js](https://nodejs.org/))
- **npm**: `v9.0.0` or higher (bundled with Node.js)

Verify your installation:

```bash
node -v
npm -v
```

### Installation

Clone the repository and install the dev dependencies:

```bash
git clone https://github.com/vishnukumar001/learning-os-520-hour-roadmap.git
cd learning-os-520-hour-roadmap
npm install
```

### Local Development

Start the local Vite development server:

```bash
npm run dev
```

Open your browser at `http://localhost:5173`. Any edits in `src/main.js` or `src/styles.css` update instantly via hot module reloading.

### Production Build

Create an optimized static distribution in the `dist/` directory:

```bash
npm run build
```

### Preview Build

Preview the generated production build locally:

```bash
npm run preview
```

---

## Data Storage & Privacy

All user data is stored strictly in your browser via `localStorage`. No data is ever transmitted over the network.

### Storage Keys

| Key | Purpose |
| --- | --- |
| `learning_os_v1` | Core state: topics, evidence, session logs, notes, projects, timer state |
| `learning_os_theme` | Selected theme mode (`light` or `dark`) |
| `learning_os_nc` | Sidebar collapsed/expanded state |

> **Note**: `localStorage` is scoped to the exact domain and port. Data on `http://localhost:5173` will not automatically appear on your deployed URL.

### Backup & Migration

1. Navigate to the **Settings** view in the application.
2. Click **Copy backup** to export your progress as a JSON string.
3. On your target browser or device, open **Settings**, paste the JSON into **Import backup**, and click **Import and replace data**.

Regularly backing up your JSON data ensures your progress is safely preserved across browser clears.

---

## Deployment

### Deploy to Vercel (Recommended)

1. Fork or push this repository to your GitHub account.
2. Log in to [Vercel](https://vercel.com/) and click **Add New → Project**.
3. Select `learning-os-520-hour-roadmap` from your GitHub repositories.
4. Vercel automatically detects the Vite configuration using `vercel.json`:
   - **Framework Preset**: Vite
   - **Build Command**: `npm run build`
   - **Output Directory**: `dist`
5. Click **Deploy**.

### Deploy to GitHub Pages (Automated via GitHub Actions)

This repository includes a pre-configured GitHub Actions workflow at [`.github/workflows/deploy.yml`](.github/workflows/deploy.yml) that automatically builds and deploys the site whenever commits are pushed to the `main` branch.

- **Live URL**: [https://vishnukumar001.github.io/learning-os-520-hour-roadmap/](https://vishnukumar001.github.io/learning-os-520-hour-roadmap/)
- **Workflow Triggers**: Automatic on pushes to `main`, or manually via **Actions → Deploy to GitHub Pages → Run workflow**.

### Deploy to Netlify

1. Link your repository in [Netlify](https://www.netlify.com/).
2. Set **Build command** to `npm run build` and **Publish directory** to `dist`.
3. Deploy!

---

## Security & Secrets

This project operates strictly on the client side:
- **No API keys or backend tokens** are required.
- `.env` files and environment variables are excluded via `.gitignore`.
- Safe for public GitHub hosting.

---

## License

This project is licensed under the [MIT License](LICENSE).
