<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="./assets/dark.png">
    <source media="(prefers-color-scheme: light)" srcset="./assets/light.png">
    <img alt="LinkCXO Engineering" src="./assets/light.png" width="720">
  </picture>

  <br />
  <br />

  <h2>LinkCXO Engineering Hub</h2>
  <p><strong>Internal Developer Portal & Engineering Standards</strong></p>

  <p>
    <img src="https://img.shields.io/badge/Access-Private_&_Internal-red?style=flat-square" alt="Private Org" />
    <img src="https://img.shields.io/badge/Team-LinkCXO_Tech-14213D?style=flat-square" alt="LinkCXO Tech Team" />
    <img src="https://img.shields.io/badge/Architecture-Microservices_%26_AI-AA933E?style=flat-square" alt="Architecture" />
    <img src="https://img.shields.io/badge/Deployments-CI%2FCD_Automated-success?style=flat-square" alt="CI/CD" />
  </p>
</div>

---

### 📌 Overview

Welcome to the **LinkCXO Engineering Organization**. This is the centralized home for all private source code, microservices, mobile apps, web portals, AI pipelines, and cloud infrastructure powering the LinkCXO platform.

> 🔒 **Confidentiality Notice:** All code, designs, documentation, and infrastructure configurations within this organization are proprietary to **LinkCxO Global Private Limited**. Access is restricted strictly to authorized engineering team members.

---

### 🗺️ Repository Architecture & Ecosystem

Our codebase is structured across modular service domains. Use this index to locate the relevant projects:

| Domain | Scope & Key Repositories | Core Stack |
| :--- | :--- | :--- |
| **📱 Mobile** | iOS and Android client applications | Flutter / Swift / Kotlin |
| **🌐 Web Platforms** | Executive web portal, administrative consoles, and internal dashboards | Next.js, React, TypeScript, Tailwind |
| **⚙️ Backend Services** | Core REST/gRPC APIs, auth service, messaging, and push notifications | Python (FastAPI), Node.js, Go |
| **🤖 AI & Data Engine** | Recommendation algorithms, NLP extraction pipelines, embeddings & RAG | Python, PyTorch, LangChain, Vector DB |
| **☁️ Infrastructure & DevOps** | Terraform scripts, Docker configurations, Kubernetes manifests, CI/CD | GitHub Actions, Docker, K8s, Cloud |

---

### 📐 Engineering Guidelines & Standards

To ensure software reliability, system stability, and smooth deployments, all team members must follow these core engineering practices:

#### 1. 🌿 Git Branching Strategy

- **`main`** — Production-ready code. Protected branch. Direct pushes are disabled.
- **`staging`** / **`develop`** — Active integration and QA testing environment.
- **Feature Branches** — Branched off `staging` or `develop`:
  - `feat/<ticket-id>-brief-description` (e.g., `feat/CXO-128-push-notifications`)
  - `fix/<ticket-id>-brief-description` (e.g., `fix/CXO-204-auth-token-refresh`)
  - `chore/<ticket-id>-brief-description` (e.g., `chore/CXO-310-update-deps`)
  - `hotfix/<ticket-id>-brief-description` (branched off `main` for critical production patches)

#### 2. 📝 Commit Message Convention

Follow standard [Conventional Commits](https://www.conventionalcommits.org/):

```text
feat(auth): add biometrics login support for mobile clients
fix(chat): resolve websocket reconnect race condition on network drop
refactor(feed): optimize query execution plan for executive timeline
chore(deps): bump next.js to 14.x
```

#### 3. 🔍 Pull Requests & Code Reviews

- **PR Requirements:**
  - Clear summary of changes with linked Jira / Linear ticket ID.
  - Screenshots / API payloads for UI or schema updates.
  - Steps for QA / reviewer to verify locally or on staging.
- **Review Rules:**
  - Every PR requires **at least 1 peer approval** before merging.
  - All automated CI tests, linters, and security checks must pass.
  - Use **Squash and Merge** to maintain a clean git commit history.

#### 4. 🔐 Secrets & Security Management

- **NEVER** commit `.env` files, API keys, certificates, or database credentials.
- Use our internal secrets manager or GitHub Organization Secrets for environment configuration.
- Review our [Internal Security Policy](SECURITY.md) for vulnerability disclosure and secret rotation protocols.

---

### 💻 Primary Technology Stack

```
Frontend & Mobile       Backend & APIs          Data & Caching          DevOps & Cloud
─────────────────       ──────────────          ──────────────          ──────────────
• Next.js / React       • Python (FastAPI)      • PostgreSQL            • Docker / K8s
• TypeScript            • Node.js / TypeScript  • Redis                 • GitHub Actions
• TailwindCSS           • Go                    • Vector Search         • AWS / GCP
• Flutter               • gRPC / REST           • Apache Kafka          • Terraform
```

---

### 🚀 Developer Onboarding Checklist

New to the LinkCXO engineering team? Follow these steps to get set up:

1. [ ] **GitHub Setup:** Enable Two-Factor Authentication (2FA) and add your work SSH key.
2. [ ] **Team Access:** Request repository access from your engineering lead via GitHub Teams.
3. [ ] **Local Environment:** Install standard toolchains (Docker, Node.js LTS, Python 3.11+, Git).
4. [ ] **Secrets & Config:** Obtain development environment variables from the internal secrets store.
5. [ ] **Branching & PRs:** Verify you can clone, build, run tests locally, and submit a draft PR.

---

### 🛠️ Internal Team Resources

| Resource | Description | Destination |
| :--- | :--- | :--- |
| 📊 **Monitoring & Logs** | Application telemetry, error tracking, and system metrics | Grafana / CloudWatch |
| 🎫 **Issue Tracking** | Sprint boards, backlog, bug tracking, and roadmaps | Project Management Portal |
| 📚 **Technical Specs** | Architecture decision records (ADRs) and API documentation | Internal Engineering Wiki |
| 💬 **Engineering Chat** | Daily standups, technical discussions, and deployment alerts | Internal Team Channels |

---

<div align="center">
  <sub>LinkCXO Engineering • Internal Team Reference • Proprietary & Confidential</sub>
</div>
