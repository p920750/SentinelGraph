# SentinelGraph: Multi-Agent Security SOC
> **WeMakeDevs Hackathon — Track 1 (Graph-Native Security & Multi-Agent Systems)**

SentinelGraph is an autonomous graph-native Security Operations Center (SOC) intelligence platform. By modeling network telemetry, processes, cloud identities, and CVEs inside **FalkorDB**, SentinelGraph empowers specialized AI agents (via the **Model Context Protocol - MCP**) to correlate alerts, map multi-hop attack paths, calculate blast radius, and trigger rapid automated remediation.

---

## 📁 Repository Structure

```
SentinelGraph/
├── docker-compose.yml       # FalkorDB graph database (port 6379)
├── .gitignore               # Root gitignore for Python, Node, & Next.js
├── DEMO_SCRIPT.md           # 3-minute video recording script & presentation guide
├── backend/
│   ├── .env.example         # Template environment configuration
│   ├── .env                 # Active environment config (credentials, host, port)
│   ├── database.py          # Centralized FalkorDB connection factory (Local + Cloud)
│   ├── main.py              # FastAPI server, GraphBLAS algorithms & MCP agent endpoints
│   ├── requirements.txt     # fastapi, uvicorn, falkordb, pydantic, mcp
│   ├── seed.py              # Multi-hop security topology database seeder
│   └── test_audit.py        # 9-point verification audit test suite
└── frontend/
    ├── .env.example         # Frontend template environment config
    ├── .env                 # Active frontend config (NEXT_PUBLIC_API_URL=http://localhost:8000)
    ├── package.json         # Next.js 14, Tailwind CSS, TypeScript, Lucide
    ├── tsconfig.json        # TypeScript configuration
    ├── tailwind.config.ts   # Custom dark cyber SOC theme
    └── src/
        ├── components/
        │   └── Header.tsx   # Responsive cyber navigation header & mobile drawer
        └── app/
            ├── layout.tsx   # Global SOC root layout
            ├── globals.css  # Dark cyber SOC design system
            ├── page.tsx     # Page 1: Landing & System Overview
            ├── dashboard/
            │   └── page.tsx # Page 2: SOC Dashboard (Alerts & Agent Dossier)
            └── analytics/
                └── page.tsx # Page 3: Graph Analytics & Cypher Console
```

---

## 🚀 Quick Start Guide

### 1. Spin up FalkorDB Graph Database
Run the root Docker Compose configuration (or connect to a cloud FalkorDB instance):
```bash
docker compose up -d
```
- **FalkorDB Redis Protocol:** `localhost:6379`

---

### 2. Run Backend (FastAPI + MCP)
```bash
cd backend
python -m venv venv
# On Windows:
.\venv\Scripts\activate
# On Linux/macOS:
source venv/bin/activate

pip install -r requirements.txt

# Seed the FalkorDB security graph:
python seed.py

# Run verification test audit:
python test_audit.py

# Launch FastAPI server:
python main.py
```
- **Backend API:** `http://localhost:8000`
- **Swagger Docs:** `http://localhost:8000/docs`
- **Health Check:** `http://localhost:8000/api/health`

---

### 3. Run Frontend (Next.js App Router)
```bash
cd frontend
npm install
npm run dev
```
- **Frontend App:** `http://localhost:3000`
  - **Overview Page:** `http://localhost:3000/`
  - **SOC Dashboard:** `http://localhost:3000/dashboard`
  - **Graph Analytics:** `http://localhost:3000/analytics`
