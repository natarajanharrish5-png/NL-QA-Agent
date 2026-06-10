# NL Browser Test Agent
# Click the link for application
https://remix-nl-browser-test-agent-685069772929.asia-southeast1.run.app

AI-powered browser testing platform that converts natural language instructions into automated browser tests.

## Features

* Natural Language Testing
* Gemini AI Planning
* Playwright Browser Automation
* Real-Time Execution Logs
* Screenshot Capture
* JSON & HTML Reports

## Tech Stack

**Frontend:** React, Vite, TypeScript, Tailwind CSS

**Backend:** Express.js, TypeScript

**AI:** Gemini 3.5 Flash

**Automation:** Playwright, Chromium

**Storage:** JSON Database

## Setup

```bash
npm install
npx playwright install chromium
npm run dev
```

Create a `.env` file:

```env
GEMINI_API_KEY=your_api_key
JWT_SECRET=your_secret
```

## Architecture

```text
User
 ↓
Frontend
 ↓
Backend
 ↓
Gemini AI
 ↓
Playwright
 ↓
Target Website
 ↓
Reports
```

## Example

**Input**

```text
Login and search laptop
```

**Output**

```json
[
  {"action":"login"},
  {"action":"search","value":"laptop"}
]
```

## Goal

Allow users to perform browser testing using plain English without writing automation scripts.
