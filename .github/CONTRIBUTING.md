# 🚀 Contributing to ZenFlow-Distraction-Free-Reading-Browser-Extension

Thank you for considering contributing to the ZenFlow Browser Extension! We welcome all contributions, from bug reports and feature requests to code submissions.

## 1. Our Philosophy

ZenFlow aims to be a distraction-free sanctuary for readers. Contributions should align with our core principles:

*   **Simplicity:** Keep features focused and intuitive.
*   **Performance:** Ensure the extension is lightweight and fast.
*   **User Focus:** Prioritize enhancements that improve the reading experience.
*   **Maintainability:** Write clean, well-documented, and testable code.

## 2. Getting Started

### 2.1. Prerequisites

Before you start, ensure you have the following installed:

*   **Node.js:** Version 18 or higher.
*   **npm** or **yarn** or **pnpm** (we recommend pnpm for efficiency).
*   **Git**.

### 2.2. Setup

Follow these steps to set up a development environment:

1.  **Clone the repository:**
    bash
    git clone https://github.com/chirag127/ZenFlow-Distraction-Free-Reading-Browser-Extension.git
    cd ZenFlow-Distraction-Free-Reading-Browser-Extension
    

2.  **Install dependencies:**
    bash
    # Using npm
    npm install
    
    # Using yarn
    # yarn install
    
    # Using pnpm
    # pnpm install
    

3.  **Build the extension (development mode):**
    bash
    # Using npm
    npm run dev
    
    # Using yarn
    # yarn dev
    
    # Using pnpm
    # pnpm dev
    
    This command will typically start a development server and watch for changes.

4.  **Load the extension in your browser:**
    *   **Chrome/Edge:** Go to `chrome://extensions` (or `edge://extensions`), enable Developer Mode, and click "Load unpacked" to load the `dist` folder (or the appropriate build output directory).
    *   **Firefox:** Go to `about:debugging#/runtime/this-firefox`, click "Load Temporary Add-on", and select the `manifest.json` file from the root of the project or the build output.

## 3. Contribution Workflow

We follow a standard GitHub pull request workflow:

1.  **Fork the repository:** Create your own fork of the `chirag127/ZenFlow-Distraction-Free-Reading-Browser-Extension` repository.
2.  **Create a new branch:** For your feature or bug fix, create a descriptive branch (e.g., `feature/new-reading-style`, `fix/unwanted-element-removal`).
    bash
    git checkout -b feature/your-feature-name
    
3.  **Make your changes:** Write your code, ensuring it follows the project's coding standards and includes relevant tests.
4.  **Test your changes:** Run the tests to ensure everything is working as expected.
    bash
    # Using npm
    npm test
    
    # Using yarn
    # yarn test
    
    # Using pnpm
    # pnpm test
    
5.  **Commit your changes:** Use conventional commits for your commit messages.
    bash
    git commit -m "feat: Add new minimalist theme"
    
6.  **Push to your fork:** Push your branch to your forked repository.
    bash
    git push origin feature/your-feature-name
    
7.  **Open a Pull Request:** Open a pull request from your branch on your fork to the `main` branch of the `chirag127/ZenFlow-Distraction-Free-Reading-Browser-Extension` repository.

## 4. Coding Standards

*   **Language:** TypeScript (Strict Mode is enabled).
*   **Formatting & Linting:** We use **Biome** for code formatting and linting. Ensure your code is formatted correctly before committing.
    bash
    # Using npm
    npm run lint
    npm run format
    
    # Using yarn
    # yarn lint
    # yarn format
    
    # Using pnpm
    # pnpm lint
    # pnpm format
    
*   **Frameworks:** React, Vite, Tailwind CSS v4.
*   **Architecture:** Feature-Sliced Design (FSD) principles are encouraged for organizing code.
*   **Testing:** Write unit tests using **Vitest** and end-to-end tests using **Playwright**. Aim for comprehensive test coverage.

## 5. Reporting Bugs

If you encounter a bug, please open an issue in the GitHub repository. Provide as much detail as possible:

*   **Browser and Version:**
*   **Extension Version:**
*   **Operating System:**
*   **Clear Steps to Reproduce:**
*   **Expected Behavior:**
*   **Actual Behavior:**
*   **Screenshots or Videos (if applicable):**

## 6. Feature Requests

Have an idea for a new feature? We'd love to hear it! Please open an issue and describe your idea. Clearly explain the problem it solves and how it would benefit users.

## 7. Code of Conduct

This project adheres to a Code of Conduct. By participating, you are expected to uphold this code. Please refer to the `CODE_OF_CONDUCT.md` file for details.

## 8. Questions?

If you have any questions about contributing, feel free to open an issue or reach out to the maintainer.

**Thank you for your contribution to ZenFlow!**
