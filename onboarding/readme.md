# Interact Onboarding Documentation

## **1. Getting Started**

1. Choose your focus

   * **Backend development** – Recommended OS: **Linux** or **macOS**.
     If you’re using Windows, install **WSL2 (Windows Subsystem for Linux)** to run the backend.
   * **Frontend development** – Any OS is fine.
2. Choose your environment

   * **Local development** – Run both backend and frontend on `localhost`.
   * **Server development** – Requires **OpenSSL** for SSL certificate handling.

---

## 2. Required Tools & Their Purpose

| Tool / Software | Description | Used For |
| -- | -- | -- |
| **Visual Studio Code** | Code editor | Writing backend and frontend code |
| **Docker Desktop** | Docker container management | Running the database and subservices |
| **Node.js (v20)** | JavaScript runtime | Running the backend server locally |
| **MongoDB Docker** | MongoDB image for Docker | Running the database in a container |
| **MongoDB Compass** | GUI for MongoDB | Managing and viewing database data     |
| **Git** | Version control | Managing code changes & collaboration  |
| **OpenSSL** *(optional)* | SSL certificate management  | Running backend on a server with HTTPS |
| **Bruno** | API testing tool | Testing backend API routes |

---

## 3. Installation Steps

1. Install Visual Studio Code
   [Download here](https://code.visualstudio.com/)

2. Install Docker Desktop for your OS
   [Download here](https://www.docker.com/products/docker-desktop/)

3. Install Node.js (version 20)
   [Download here](https://nodejs.org/en/download)

   * Alternatively, use **nvm (Node Version Manager)** to manage multiple Node.js versions.

4. Install MongoDB Docker image
   [View on Docker Hub](https://hub.docker.com/_/mongo)

5. Install MongoDB Compass
   [Download here](https://www.mongodb.com/products/tools/compass)

6. Install Git

   * [Download here](https://git-scm.com/downloads)
   * Or on Linux:

     ```bash
     sudo apt-get install git
     ```

7. **(Optional)** Install OpenSSL

   * On macOS: Preinstalled
   * On Linux:

     ```bash
     sudo apt-get install openssl
     ```

8. **Install Bruno** (API testing tool)
   [Download here](https://www.usebruno.com)

---

## **4. Next Steps**

* **Clone the repository**

  ```bash
  git clone <repository_url>
  cd <repository_folder>
  ```

* **Set up environment variables** – Follow `.env.example` and create your `.env` file.

* **Start Docker containers**

  ```bash
  docker-compose up -d
  ```

* **Run the backend locally**

  ```bash
  npm install
  npm run dev
  ```

* **Run the frontend** – Follow frontend setup documentation in `/frontend`.

---

This version is **clearer, formatted for readability, and beginner-friendly**.

If you want, I can also make a **quick-start “one-page” onboarding sheet** so a new developer can be up and running in under 10 minutes. That would make onboarding even smoother.
