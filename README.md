# Voder — AI-Powered Web IDE & Coding Workspace

> **Developed by Bhuvan**

Voder is a restrained, browser-based coding IDE and interactive playground featuring Python asynchronous input execution, Java console programs with `Scanner(System.in)`, live sandboxed HTML/CSS/JS and React previews, and dual AI assistance (built-in Voder AI and Gemini Cloud AI).

---

## Features

- **Pre-Project Home Dashboard (`/app`)**: Clean, distraction-free dashboard on startup. No sample project is forced into the editor until you create or open one.
- **Interactive Python 3.11 Execution**:
  - Non-blocking asynchronous stdin queue.
  - Supports sequential `input()` calls directly in the in-app terminal without browser `window.prompt()`.
  - Built-in 9-case automated Python stdin verification test suite.
- **Java SE Console Runner**:
  - Write multi-file Java classes (`Main.java`, `Student.java`).
  - Supports interactive `Scanner(System.in)` terminal input.
- **Live Sandboxed Web & React Preview**:
  - Multi-file bundling for HTML, CSS, JavaScript, and React (JSX/TSX).
  - Resolves relative module imports in-browser.
  - Desktop, tablet, and mobile viewport simulation.
  - Console forwarding directly to the bottom IDE console drawer.
- **AI Coding Assistant & Diff Approval Engine**:
  - **Voder AI (Built-in)**: Zero-download, instantly ready coding engine.
  - **Gemini Cloud AI**: Optional cloud provider integration with configurable API keys.
  - Granular context control: Checkbox selection of exactly which project files are shared.
  - Side-by-side diff review with one-click **Accept & Apply**, **Reject**, and **Undo Last AI Edit**.
- **Curated 1,020-Example Dataset Explorer**:
  - Validated coding tasks across 10 categories with train/validation/test splits.
  - One-click loading of dataset solutions directly into the editor.
- **ZIP Export & Project Persistence**:
  - Full project import and export as `.zip` or `.json` archives.
  - Local persistence across sessions.

---

## Tech Stack

- **Frontend**: React 18, TypeScript, Vite, Tailwind CSS
- **Icons**: Lucide React
- **Runtime Sandbox**: Babel Standalone (in-browser transpilation for React & TypeScript)
- **Deployment**: Vercel SPA (configured via `vercel.json`)

---

## Project Structure

```text
voder/
├── index.html
├── package.json
├── tsconfig.json
├── vite.config.ts
├── vercel.json
├── README.md
└── src/
    ├── main.tsx
    └── App.tsx
