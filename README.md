# React AdBlock Chrome Extension 🛡️

A modern, high-performance ad blocker built for Google Chrome. This extension demonstrates the implementation of **Manifest V3** privacy standards, using network-level filtering to block advertisements and trackers before they even reach the browser.

## 🚀 Key Features
* **Network-Level Blocking:** Leverages the `declarativeNetRequest` API to block ads at the request level, ensuring minimal impact on browser performance.
* **Static Rule Sets:** Includes pre-configured rules for blocking common analytics and tracking domains (e.g., Google Analytics, DoubleClick).
* **Manifest V3 Compliant:** Fully optimized for the latest Chrome Extension security and performance architecture.
* **React & TypeScript:** A clean, type-safe codebase providing a modern development experience.
* **Webpack Build Pipeline:** Custom Webpack configuration for bundling React components, content scripts, and background workers.

## 🛠 Tech Stack
* **Framework:** React.
* **Language:** TypeScript.
* **Build Tool:** Webpack 5.
* **Chrome APIs:** `declarativeNetRequest`, `storage`, `tabs`.

## 📦 Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/oleksandrivanyshyn/extension-chrome-react-adblock.git
    ```
2.  **Install dependencies:**
    ```bash
    npm install
    ```
3.  **Build the extension:**
    ```bash
    npm run build
    ```
4.  **Load into Chrome:**
    * Open `chrome://extensions/`.
    * Enable **Developer mode**.
    * Click **Load unpacked**.
    * Select the `dist` folder from your local project directory.

## 📖 Project Structure
* **src/static/rules.json:** Contains the declarative filtering rules for ad blocking.
* **src/background/background.ts:** Manages extension-level events and ruleset updates.
* **src/static/manifest.json:** Defines the permissions and core configuration of the extension.
