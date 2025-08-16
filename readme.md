# Interact API Documentation
Started by Daniel Kravec, on April 26, 2022

Interact was started on July 23, 2021

Base API URL ``https://interact-api.novapro.net/``

---
### 1. Information

Interact is online and accessible at [interact.novapro.net](https://interact.novapro.net)

You are able to use the API in a limited fashion. Most documentation is not up to date, you can reverse engineer the API by using the main [Interact](https://interact.novapro.net) frontend.

For each release, you must follow the instructions in [releases](./releases.md) to prepare any given repository for the release.

For onboarding documentation, see [onboarding](./onboarding/readme.md). This will help you get started with the frontend (and backend in the future) development of Interact.

---

### 2. Get Started

Create developer account and application token
1) Open [Interact](https://interact.novapro.net)
2) Login / Create an Interact account
3) Open settings /?settings
4) Scroll down to "Developer"
5) Press "Show Dev Settings"
6) Click "Sign up for a developer account."
7) Create an app token
8) press "Hide Developer Settings"
9) Press "Show Dev Settings"
10) Look for "Generate New App Token"
11) Type inside "Application Name" the name of your app
12) Press "Generate Token"

To copy your developer token
1) Open [Interact](https://interact.novapro.net)
2) Login / Create an Interact accoun
3) Open settings
4) Scroll down to "Developer"
5) Press "Show Dev Settings"
6) Locate "Developer Account"
7) Press "Copy Token" under "Dev Account Created"
8) Save this token in a safe location for future use, this is "devtoken"

To copy your application token
1) Open [Interact](https://interact.novapro.net)
2) Login / Create an Interact account
3) Open settings
4) Scroll down to "Developer"
5) Press "Show Dev Settings"
6) Locate "App Token" OR "App Tokens"
6) Press "Copy Token" above "API Uses"
7) Save this token in a safe location for future use, this is "appoken"


---
### 3. API Versions

| API Version | Active | Routes | Schemas |
| -- | -- | -- | -- |
| 1 | true | [Routes](./v1/readme.md) | [Schemas](./v1/schemas/readme.md) |