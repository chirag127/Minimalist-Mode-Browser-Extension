# MinimalistView: Content Focus Browser Extension


![MinimalistView Hero Banner](https://raw.githubusercontent.com/chirag127/MinimalistView-Content-Focus-Browser-Extension/main/.github/assets/banner.png)


<div align="center">

[
![Build Status](https://img.shields.io/github/actions/workflow/status/chirag127/MinimalistView-Content-Focus-Browser-Extension/ci.yml?branch=main&style=flat-square&logo=githubactions&logoColor=white)
](https://github.com/chirag127/MinimalistView-Content-Focus-Browser-Extension/actions/workflows/ci.yml)
[
![Code Coverage](https://img.shields.io/codecov/c/github/chirag127/MinimalistView-Content-Focus-Browser-Extension?style=flat-square&logo=codecov&logoColor=white)
](https://app.codecov.io/gh/chirag127/MinimalistView-Content-Focus-Browser-Extension)
[
![Tech Stack](https://img.shields.io/badge/Tech-TypeScript%20%7C%20WXT%20%7C%20Vite-blue?style=flat-square&logo=typescript)
](https://wxt.dev/)
[
![Linter & Formatter: Biome](https://img.shields.io/badge/Linter%20&%20Formatter-Biome-blueviolet?style=flat-square&logo=biome)
](https://biomejs.dev/)
[
![License: CC BY-NC 4.0](https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg?style=flat-square)
](https://creativecommons.org/licenses/by-nc/4.0/)
[
![GitHub Stars](https://img.shields.io/github/stars/chirag127/MinimalistView-Content-Focus-Browser-Extension?style=flat-square&logo=github&logoColor=white)
](https://github.com/chirag127/MinimalistView-Content-Focus-Browser-Extension/stargazers)

</div>

> **Enhance focus by minimizing UI elements and distractions on web pages. A clean, minimalist browser extension for a distraction-free browsing experience.**

This tool declutters your digital workspace by intelligently hiding non-essential elements like sidebars, headers, and pop-ups, allowing you to concentrate solely on the content that matters.

<div align="center">
<a href="https://github.com/chirag127/MinimalistView-Content-Focus-Browser-Extension/stargazers"> <img src="https://img.shields.io/static/v1?label=%E2%AD%90&message=Star this Repo&style=social&logo=github" alt="Star the repo"></a>
</div>

---

## 🏛️ Architecture Overview

This project adheres to the **Feature-Sliced Design (FSD)** methodology, promoting a scalable and maintainable codebase. The structure isolates business logic into self-contained features, ensuring low coupling and high cohesion.

sh
. # Root
├── .github/          # CI/CD, templates, and assets
├── .vscode/          # VSCode settings for consistent development
├── entrypoints/      # Extension entry points (popup, background, content)
│   ├── background.ts # Background service worker
│   ├── content.ts    # Content script for page manipulation
│   └── popup/        # Popup UI files (HTML, TSX)
├── features/         # Business logic modules (e.g., element-hiding, domain-rules)
│   └── element-hider/
│       ├── lib/      # Business logic and utility functions
│       └── model/    # Data models and types
├── shared/           # Reusable code across the application
│   ├── api/          # External API clients (e.g., storage API)
│   ├── config/       # Global configuration
│   └── ui/           # Shared UI components (e.g., buttons, toggles)
├── public/           # Static assets (icons, manifest.json)
└── package.json      # Project dependencies and scripts


---

## 📋 Table of Contents

- [Key Features](#-key-features)
- [🤖 AI Agent Directives](#-ai-agent-directives)
- [🚀 Getting Started](#-getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [🛠️ Development Scripts](#️-development-scripts)
- [📜 Core Principles](#-core-principles)
- [🤝 Contributing](#-contributing)
- [🔐 Security Policy](#-security-policy)
- [📄 License](#-license)

---

## ✨ Key Features

- **One-Click Cleaning:** Instantly remove distracting elements from any webpage.
- **Customizable Rules:** Define per-domain rules to specify which elements to hide or keep.
- **Minimalist UI:** A clean and intuitive popup interface for managing settings.
- **High Performance:** Optimized content scripts ensure minimal impact on browser performance.
- **Cross-Browser Support:** Built with WXT for compatibility with Chrome, Firefox, and Edge.

---

## 🤖 AI Agent Directives

<details>
<summary><strong>SYSTEM: APEX TECHNICAL AUTHORITY (DECEMBER 2025 EDITION)</strong></summary>

### 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards.
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

### 2. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
This repository, `MinimalistView-Content-Focus-Browser-Extension`, is a modern web extension.

*   **PRIMARY SCENARIO: WEB / EXTENSION (TypeScript)**
    *   **Framework:** **WXT** (`wxt.dev`) is the primary framework for building a robust, cross-browser extension.
    *   **Build Tool:** **Vite** is used under the hood by WXT for lightning-fast HMR and optimized builds.
    *   **Language:** **TypeScript (Strict Mode)** is mandatory for all code to ensure type safety and maintainability.
    *   **Styling:** **TailwindCSS v4** for utility-first CSS.
    *   **Linting & Formatting:** **Biome** is the single source of truth for code quality. All code MUST pass `npx @biomejs/biome check --apply` before merging.
    *   **Architecture:** Adheres strictly to **Feature-Sliced Design (FSD)**. All new functionality must be encapsulated within `features/`, `shared/`, or `entrypoints/` slices.

*   **VERIFICATION & TESTING PROTOCOL**
    *   **Unit & Integration Tests:** **Vitest** is the designated framework. Coverage must be maintained at or above 90%.
    *   **End-to-End (E2E) Tests:** **Playwright** is used to simulate user interactions and validate extension behavior in a real browser environment.
    *   **CI/CD Pipeline:** The `.github/workflows/ci.yml` pipeline automates linting, testing, and build verification on every pull request.

</details>

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v20.x or higher)
- [pnpm](https://pnpm.io/) (v9.x or higher)

### Installation

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/MinimalistView-Content-Focus-Browser-Extension.git
    cd MinimalistView-Content-Focus-Browser-Extension
    

2.  **Install dependencies:**
    bash
    pnpm install
    

3.  **Run the development server:**
    bash
    pnpm dev
    

4.  **Load the extension in your browser:**
    - Open your browser's extension management page.
    - Enable "Developer Mode".
    - Click "Load unpacked" and select the `dist` directory.

---

## 🛠️ Development Scripts

| Command         | Description                                        |
| --------------- | -------------------------------------------------- |
| `pnpm dev`      | Starts the development server with HMR.            |
| `pnpm build`    | Compiles and bundles the extension for production. |
| `pnpm test`     | Runs all unit and integration tests with Vitest.   |
| `pnpm test:e2e` | Runs all end-to-end tests with Playwright.         |
| `pnpm lint`     | Checks code for linting and formatting issues.     |
| `pnpm format`   | Automatically formats the entire codebase.         |

---

## 📜 Core Principles

-   **SOLID:** Code is structured following SOLID principles for maintainability and scalability.
-   **DRY (Don't Repeat Yourself):** Reusable logic is abstracted into shared modules.
-   **YAGNI (You Ain't Gonna Need It):** Features are built to solve current problems, avoiding premature optimization.

---

## 🤝 Contributing

Contributions are welcome! Please read the [CONTRIBUTING.md](./.github/CONTRIBUTING.md) file for guidelines on how to submit pull requests, report issues, and suggest enhancements.

## 🔐 Security Policy

The security of this project is taken seriously. Please refer to our [SECURITY.md](./.github/SECURITY.md) file for information on how to report security vulnerabilities.

## 📄 License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License**.

See the [LICENSE](./LICENSE) file for more details.