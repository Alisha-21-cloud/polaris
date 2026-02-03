
# Polaris — Cloud IDE with AI Assistance

![License](https://img.shields.io/badge/license-MIT-green?style=for-the-badge)
![Next.js](https://img.shields.io/badge/Next.js-16-black?style=for-the-badge&logo=next.js)
![React](https://img.shields.io/badge/React-19-61dafb?style=for-the-badge&logo=react)
![TypeScript](https://img.shields.io/badge/TypeScript-Strict-3178c6?style=for-the-badge&logo=typescript)
![Convex](https://img.shields.io/badge/Convex-Realtime_DB-orange?style=for-the-badge)
![AI](https://img.shields.io/badge/AI-Gemini-purple?style=for-the-badge)

Polaris is a **modern, browser-based Cloud IDE** inspired by Cursor, designed to deliver **real-time collaboration**, **AI-assisted development**, and **scalable project management** directly in the browser.

This repository represents a **complete end-to-end engineering workflow**, from authentication and real-time databases to AI-powered code editing and background job orchestration.

---

## ✨ Key Features

- Real-time collaborative code editing
- AI-powered inline code suggestions
- Natural-language code editing (Cmd + K)
- Conversational AI assistant
- Multi-file project workspace
- Optimistic UI with real-time sync
- Scalable backend with background jobs
- Production-ready authentication and error tracking

---

## 🧠 Tech Stack

### Frontend
- Next.js 16 (App Router)
- React 19
- TypeScript
- Tailwind CSS 4
- shadcn/ui + Radix UI

### Editor
- CodeMirror 6
- Custom extensions
- One Dark theme

### Backend & Infra
- Convex (Real-time database)
- Inngest (Background jobs)
- Clerk (Authentication with OAuth)
- Sentry (Monitoring & error tracking)

### AI
- Claude Sonnet (primary)
- Gemini Flash (alternative)

### Execution (Planned)
- WebContainer API
- xterm.js

---

## 🌳 Git Workflow & Branch Strategy

This project follows a **feature-based Git workflow**, where each major system was implemented in an isolated branch and later merged into `main`.

### Implemented Branches

- `setup-ui-theme`
- `auth-clerk-integration`
- `convex-realtime-db`
- `inngest-background-jobs`
- `ai-suggestions-engine`
- `ai-conversation-system`
- `file-explorer-system`
- `editor-codemirror`
- `projects-dashboard`
- `ai-agent-tools`
- `webcontainer-preview`
- `terminal-integration`
- `github-import-export`
- `ai-project-generator`

---

## 📁 Project Structure

```
src/
├── app/
│   ├── api/
│   │   ├── messages/
│   │   ├── suggestion/
│   │   └── quick-edit/
│   └── projects/
├── components/
│   ├── ui/
│   └── ai-elements/
├── features/
│   ├── auth/
│   ├── conversations/
│   ├── editor/
│   ├── preview/
│   └── projects/
├── inngest/
└── lib/

convex/
├── schema.ts
├── projects.ts
├── files.ts
├── conversations.ts
└── system.ts
```

---

## ⚙️ Installation & Setup

### Prerequisites
- Node.js 20+
- npm or pnpm

### Environment Configuration

Create a `.env.local` file:

```env
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

NEXT_PUBLIC_CONVEX_URL=
CONVEX_DEPLOYMENT=
POLARIS_CONVEX_INTERNAL_KEY=

GOOGLE_GENERATIVE_AI_API_KEY=

FIRECRAWL_API_KEY=
SENTRY_DSN=
```

### Run Locally

```bash
npm install
npx convex dev
npm run dev
npx inngest-cli@latest dev
```

Open: `http://localhost:3000`

---

## 🧩 Implemented Capabilities

### Editor
- Syntax highlighting (JS, TS, CSS, HTML, JSON, MD, Python)
- Multi-cursor editing
- Minimap & folding
- Auto-save with debouncing

### AI
- Inline ghost-text suggestions
- Cmd + K quick edits
- Context-aware conversations

### File System
- Create / rename / delete files & folders
- VSCode-style explorer
- Tab-based navigation

### Real-Time
- Optimistic updates
- Instant sync across clients
- Background task handling

---

## 🚧 Planned Enhancements

- AI agent with file system control
- Terminal & live preview
- GitHub repository sync
- AI-generated starter projects
- Conversation history management

---

## 📜 Scripts

```bash
npm run dev
npm run build
npm run start
npm run lint
```

---

## 📄 License

This project is licensed under the **[MIT License](LICENSE)**.


---

## 👤 Author

**Syed Ahmad Alisha**  
AI & ML Engineer | Full-Stack Developer  

---

## ⭐ Acknowledgements

- Cursor — Inspiration
- shadcn/ui
- CodeMirror
- Convex
