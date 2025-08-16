# Interact Onboarding Documentation

## 1. Overview

Currently, Interact contributors will be focusing on **frontend development**.
The backend and microservices are currently hosted in **production** and require additional security steps that aren’t part of this onboarding.

When a **development backend** is ready, this guide will be updated with backend onboarding instructions. If you want to contribute to the backend, please contact Daniel Kravec directly at [daniel@dkravec.net](mailto:daniel@dkravec.net)

---

## 2. Common Setup

### Required Tools

| Tool | Purpose | Link |
| -- | -- | -- |
| **Visual Studio Code** | Code editor | [Download](https://code.visualstudio.com/) |
| **Live Server extension** | Local development server for HTML/JS/CSS | [Install from VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) |
| **Git** | Version control | [Download](https://git-scm.com/downloads) | 

---
## 3. Releases
For each release, you must follow the instructions in [releases](./releases.md) to prepare any given repository for the release.

---

## 4. Frontend Quick Start

1. **Clone the Repository**
    * Navigate to a folder for repositories, ex: `~/git, ~/dev, ~/repos`
    ```bash
    mkdir social-novapro
    cd social-novapro
    git clone https://github.com/social-novapro/social-frontend-plain
    ```

2. Open the Frontend Repository in VS Code
    * Navigate to the `social-frontend-plain/html` folder in VS Code.
    * You must open the `html` folder, not the root of the repository, as the HTML files are located there.

3. Set API Environment
    * Open the file `config.js` in the html folder.
    * Confirm that line 3 is set to prod: `"current" : "prod",` (set by default)
    * Create API Tokens, follow [Get Started](../readme.md#2-get-started) to create your developer and application tokens.
    * Copy the devtoken, and apptoken, and place it into the config file: 
    ```javascript
    var headers = {
        'Content-Type': 'application/json',
        "devtoken" : "XXX-XXX-XXX-XXX-XXX",
        "apptoken" : "XXX-XXX-XXX-XXX-XXX"
    }
    ```
    * Replace the XXX-XXX-XXX-XXX with your own developer and application tokens.

4. Start Live Server
    * Right-click the `index.html` file.
    * Select **"Open with Live Server"**.
    * The app will open in your browser at:
    ```
    http://127.0.0.1:5500/
    ```
    * You can login with your Interact account or create a new one.

5. Develop
    * Any changes you save will automatically refresh in the browser.

---

## 5. API Usage Notes
* The frontend is connected to the **production API** by default.
* Some endpoints may require authentication or tokens.
* Do **not** submit real or sensitive data during frontend development.

---

## 6. Backend Onboarding (Coming Soon)

Backend onboarding will be added when a **development backend environment** is available.
Planned improvements:

* A full development ready backend instance, with all microservices.
* An seperate endpoint for backend contributors to test their changes with real data.
    * Such as, DB, AI, and media services.
    * This will also allow developers to not worry about setting up their own backend instances.
* Shared development tokens for contributors.