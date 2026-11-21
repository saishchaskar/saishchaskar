# Hi, I'm Saish Chaskar 👋

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0e76a8?style=for-the-badge&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/saish-chaskar/) [![Twitter](https://img.shields.io/badge/-Twitter-00acee?style=for-the-badge&logo=Twitter&logoColor=white)](https://twitter.com/SaishChaskar) [![Instagram](https://img.shields.io/badge/-Instagram-e4405f?style=for-the-badge&logo=Instagram&logoColor=white)](https://www.instagram.com/saishchaskar/?igshid=OGQ5ZDc2ODk2ZA%3D%3D)

### Full-Stack Software Engineer · GCP Certified Cloud Architect

> *Building reliable web platforms, backend data services, and observable infrastructure.*

---

## About Me

I’m a **Software Development Engineer** working across the full stack—from browser interfaces and backend APIs to bare-metal observability. Currently, I build software for warehouse automation and live sortation systems at **Unbox Robotics**.

Working close to production hardware has shaped how I write code: writing a feature is only part of the job; making sure it behaves predictably under load and tells you when something breaks is what makes it dependable.

- **Backend & Real-Time Systems:** Build low-latency APIs (**<100ms**) and event-driven services processing **30–40K+ events/day** across **Java (Spring Boot)**, **Python**, **Node.js**, and **PostgreSQL**.
- **Cloud & Infrastructure:** **GCP Professional Cloud Architect** focused on cloud-native architectures, automated CI/CD pipelines, and practical **RAG / MCP** workflows.
- **Observability & Reliability:** Deploy and tune bare-metal monitoring stacks using **Grafana**, **Prometheus**, **Loki**, and **OpenTelemetry** to trace bottlenecks and prevent production incidents.
- **Currently Exploring:** Distributed System Design, **Apache Kafka**, and **Terraform (IaC)**.
- **Selected Builds:** End-to-end systems including **AgroConnect**, **ResumeMetrics**, and **PetroConnect**.
- **Developer Community:** Regular attendee and builder at **GDG Pune**, **Cloud Native Pune**, and **JS Pune** meetups, and hackathons like **MumbaiHacks**.

---

## Architecture & Engineering Workflows

### 1. Real-Time Backend & Bare-Metal Observability Flow

```mermaid
flowchart LR
    A[Warehouse Hardware & Client UIs<br/>React · Live Sortation] -->|<100ms APIs| B[Backend Services<br/>Java Spring Boot · Python · Node.js]
    B -->|30–40K+ events/day| C[(PostgreSQL<br/>Transactional State)]
    B -->|Traces & Metrics| D[OpenTelemetry]
    D --> E[Prometheus<br/>Metrics]
    D --> F[Loki<br/>Log Aggregation]
    E --> G[Grafana Dashboards<br/>Alerting & Bottleneck Tracing]
    F --> G
```

### 2. Cloud-Native, CI/CD & RAG / MCP Workflow

```mermaid
flowchart LR
    A[Git Push / PR] --> B[Automated CI/CD Pipeline]
    B --> C[GCP Cloud-Native Services<br/>Professional Cloud Architect]
    C --> D[RAG / MCP Workflows<br/>Context & Retrieval]
    C -.->|Exploring| E[Apache Kafka & Terraform IaC]
```

### 3. Hybrid Edge-AI & Guardrailed RAG Flow (AgroConnect PWA)

```mermaid
flowchart LR
    A[Farmer Camera<br/>22 Indic Languages] --> B[Quality & Blur Check]
    B --> C[On-Device TFLite<br/>MobileNetV3 INT8 <15MB · <300ms]
    C -->|Offline| D[Local Crop & Disease Diagnosis]
    C -->|Online Sync| E[Spring Boot / FastAPI Gateway]
    E --> F[Vector Search<br/>ChromaDB · ICAR & PPQS Manuals]
    F -->|Similarity >= 0.7| G[Gemini 2.0 Flash<br/>JSON Advisory + Redis Cache]
    F -->|Similarity < 0.7| H[Safe KVK Officer Fallback]
    G --> I[AI4Bharat IndicTrans2<br/>Localized Farmer UI]
    H --> I
```

### 4. Async Resume Scoring & ATS Intake Pipeline (ResumeMetrics)

```mermaid
flowchart LR
    A[React Client / ATS Portal<br/>Firebase Hosting · Bearer API] -->|Resumable Upload up to 1 GiB ZIP| B[Private GCS Bucket]
    B --> C[Cloud Run Job<br/>ZIP Validation & Fan-Out]
    C --> D[Cloud Tasks Queue<br/>OIDC-Verified Workers]
    D --> E[Flask API on Cloud Run<br/>Sentence Transformers 75% + Term Match 25%]
    E --> F[(Firestore<br/>Ranked Scores & Evidence Excerpts)]
    F --> G[Live Polling UI & CSV/Excel Export]
```

### 5. Shift Accounting, Carry-Forward & Analytics Flow (PetroConnect)

```mermaid
flowchart LR
    A[React + TypeScript Dashboard<br/>Ant Design · Debounced Auto-Save] -->|BCrypt Session & REST| B[Spring Boot 3 API<br/>DSR · Station Config · Analytics]
    B -->|Flyway Migrations| C[(PostgreSQL JSONB<br/>Flexible DU/Nozzle & DSR Payloads)]
    C -->|Auto Carry-Forward| D[Next Shift Opening Readings<br/>& Completed-Shift Locking]
    B --> E[Monthly Consolidated PDF<br/>& Recharts Fuel-Mix Analytics]
```

---

## Project Highlights

| Project | Highlights & Architecture | Core Stack | Repository |
| :--- | :--- | :--- | :--- |
| **AgroConnect PWA** | Offline-first AgriTech platform for **450+ Indian crop diseases & pests** combining on-device **TFLite (<300ms)** inference with a **guardrailed RAG** pipeline (similarity ≥ 0.70 + KVK fallback) and **22 Indic languages**. | Angular 18 · Java 21 · Spring Boot · TFLite · Gemini 2.0 Flash · ChromaDB · Redis · IndicTrans2 | [agroconnect-pwa](https://github.com/saishchaskar/agroconnect-pwa) · [AgroConnect-dev](https://github.com/saishchaskar/AgroConnect-dev) |
| **ResumeMetrics** | Cloud-native resume screening workspace & ATS integration API supporting **1 GiB ZIP** direct-to-GCS uploads, **Cloud Run Job** fan-out, **Cloud Tasks** async scoring (**75% semantic + 25% keyword**), and CSV/Excel exports. | React · Tailwind · Flask · Sentence Transformers · Cloud Run · Cloud Tasks · GCS · Firestore · Firebase | [resume-metrics](https://github.com/saishchaskar/resume-metrics) |
| **PetroConnect** | Full-stack petrol-station management platform for **Day/Night Daily Sales Reports (DSRs)**, automatic nozzle reading carry-forward, cash/UPI/credit reconciliation, tanker/dip inventory, and monthly PDF & Recharts analytics. | React 18 · TypeScript · Ant Design · Java 21 · Spring Boot 3 · PostgreSQL (JSONB) · Flyway · Docker | [petro-connect-manager](https://github.com/saishchaskar/petro-connect-manager) · [petro-connect-dashboard](https://github.com/saishchaskar/petro-connect-dashboard) |
| **AgroConnect (Android)** | Earlier native Android implementation delivering **data.gov.in (OGD)** market prices, weather updates, and Firebase authentication. | Java · Android Studio (MVVM) · Firebase | [Shetkari](https://github.com/saishchaskar/Shetkari) |

---

![saishchaskar's Streak](https://streak-stats.demolab.com/?user=saishchaskar&theme=transparent&hide_border=true&stroke=0000&background=00000000&ring=0e76a8&fire=0e76a8&currStreakLabel=0e76a8)
