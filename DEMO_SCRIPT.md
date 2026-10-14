# SentinelGraph: 3-Minute Demo Video Script & Walkthrough Guide
> **Tailored for Hackathon Judges, Evaluators, and Non-Technical Viewers**  
> **Target Video Runtime:** 2 minutes 45 seconds – 3 minutes 00 seconds  
> **Target Speaking Pace:** 130 – 140 words per minute (confident, clear, conversational)

---

## 🎬 Pre-Recording Checklist & Technical Setup

### 1. Environment & Server Initialization
Before hitting "Record", ensure both backend and frontend services are running and healthy:
- **Terminal 1 (FalkorDB Docker):**
  ```bash
  docker compose up -d
  ```
  *(Note: If Docker is unavailable, SentinelGraph runs automatically in Deterministic Local Topology Mode with 100% interactive fidelity!)*
- **Terminal 2 (FastAPI Backend):**
  ```bash
  cd backend
  python main.py
  ```
  *Verify:* `http://localhost:8000/api/health` returns `200 OK`.
- **Terminal 3 (Next.js Frontend):**
  ```bash
  cd frontend
  npm run dev
  ```
  *Verify:* `http://localhost:3000` loads cleanly.

### 2. Browser & Recording Configuration
- **Browser Window:** Chrome, Edge, or Brave set to **1080p (1920x1080)** resolution with **100% zoom**.
- **Clean Screen:** Hide bookmarks bar (`Ctrl+Shift+B`), close non-essential tabs, and disable desktop notifications.
- **Mouse Cursor:** In OBS or Loom, enable **mouse cursor highlighting** or a subtle yellow halo so viewers can follow your clicks effortlessly.
- **Clean Starting State:**
  - Open `http://localhost:3000/dashboard`.
  - If the status badge already says "QUARANTINE ENFORCED", click the **"Reset Breach Scenario"** button in the top right to return the system to the active breach state.
  - Navigate back to `http://localhost:3000/` (Overview page) to begin the recording.

### 3. Voice & Inflection Guidelines
- **Speak to Business Impact:** Emphasize *what problem is solved* (stopping hackers, protecting customer payment records) rather than getting bogged down in database syntax.
- **Highlight Velocity:** Whenever FalkorDB responds, emphasize phrases like *"single-digit milliseconds"* and *"instant visibility"*.
- **Use Visual Synchronization:** Never speak about a button before pointing to it. Move the cursor smoothly, pause for half a second on key cards, and click with deliberate pacing.

---

## ⏱️ Video Timeline Overview

```
0:00 ─── Hook & The Security Blindspot ─── 0:30
0:30 ─── Page 1: Landing & Architecture Overview ─── 1:00
1:00 ─── Page 2: SOC Command Center & Threat Triage ─── 1:30
1:30 ─── Page 2: 1-Click Autonomous Mitigation ─── 2:00
2:00 ─── Page 3: Graph Analytics Console ─── 2:30
2:30 ─── Conclusion & Hackathon Impact ─── 3:00
```

---

## 🎙️ Master Dual-Column Teleprompter Script

### Scene 1: The Hook & The Security Blindspot (0:00 – 0:30)
* **Goal:** Capture immediate attention by contrasting legacy alert fatigue with real-world connected risk.

| Visual Action & Screen Cue | Spoken Voiceover Script | Delivery & Timing Notes |
| :--- | :--- | :--- |
| **[0:00]** Full screen showing the SentinelGraph hero title on `http://localhost:3000`.<br><br>The cursor rests comfortably on the animated gradient title: *"SentinelGraph: Autonomous Multi-Agent Security SOC"*. | "Every modern company runs on the cloud—interconnecting Kubernetes pods, cloud permissions, and databases. But when a cyberattack strikes, traditional security tools fail at one critical job: **they cannot see the big picture**." | **Tone:** Engaging, authoritative.<br><br>**Pacing:** Steady and deliberate. |
| **[0:15]** Slowly scroll down just enough to reveal the four architecture capability cards.<br><br>Cursor gestures in a wide arc across the screen. | "Security teams get bombarded by hundreds of disconnected alerts every single day. A compromised web server in one room doesn't know it connects to the customer database in another. Tracing how a hacker moves laterally takes human analysts hours or even days—and by then, data is already gone." | **Emphasis:** *"hundreds of disconnected alerts"*.<br><br>[Brief 0.5s pause before pivot]. |
| **[0:24]** Scroll back smoothly to the top hero section. Hover over the pulsing status badge: **"Powered by FalkorDB"**. | "That’s why we built **SentinelGraph**—an autonomous, graph-native Security Operations Center that connects every single dot in real time." | **Tone:** Enthusiastic and confident. |

---

### Scene 2: Page 1 — Landing & Architecture Overview (0:30 – 1:00)
* **Goal:** Demystify the graph engine using simple analogies and demonstrate interactive data seeding.

| Visual Action & Screen Cue | Spoken Voiceover Script | Delivery & Timing Notes |
| :--- | :--- | :--- |
| **[0:30]** Hover mouse over the **"Dynamic Security Topology Snapshot"** section.<br><br>Hover briefly over each counter pill: Active Pods (3), IAM Identities (2), Zero-Day CVEs (2), and Blast Radius Nodes (7). | "Think of SentinelGraph like a live subway map for your entire IT infrastructure. Powered by **FalkorDB**—an ultra-low latency graph engine—we model every server, user identity, and vulnerability as connected points in a live relationship graph." | **Analogy:** *"live subway map"* helps non-technical judges instantly understand graphs. |
| **[0:45]** Move mouse to the purple button: **"Seed Security Graph"** and click it.<br><br>A cyber toast notification slides into the top right corner displaying: *"Security Graph Re-seeded: Initialized 7 nodes and 6 security relationships on sentinel_soc space"*. | "With a single click, our security graph seeds our live production topology: correlating public Kubernetes containers, privileged cloud roles, and active zero-day exploits into an interconnected knowledge web." | **Timing:** Wait 1 second to let the toast notification animate and fade smoothly. |
| **[0:54]** Move cursor down to the primary blue button: **"Launch SOC Dashboard"** and click it. | "Now, let’s step into the shoes of a security engineer and enter the live SOC Command Center." | **Transition:** Click cleanly to trigger navigation to `/dashboard`. |

---

### Scene 3: Page 2 — SOC Command Center & Live Threat Triage (1:00 – 1:30)
* **Goal:** Showcase the live breach scenario, the MITRE attack mapping, and the visual threat trajectory toward the crown jewel.

| Visual Action & Screen Cue | Spoken Voiceover Script | Delivery & Timing Notes |
| :--- | :--- | :--- |
| **[1:00]** Page `/dashboard` loads.<br><br>Highlight the top header: the flashing red status badge reads: **"ACTIVE EXPLOITATION"**.<br><br>Move cursor to Column 1 (Incident Queue). | "We're inside the SOC Command Center, and an active incident has just triggered. On the left, our alert queue flags **Incident 7701**: a critical Remote Code Execution vulnerability with a maximum CVSS score of 9.8." | **Tone:** Urgent and focused.<br><br>**Visual:** Hover over the critical red alert card. |
| **[1:12]** Move mouse to Column 2 (Center Visualizer Canvas).<br><br>Hover over the pulsing red node labeled **`k8s-pod-77`**.<br><br>Trace the connecting arrows from `k8s-pod-77` -> `sa-admin` -> `auth-service` -> to the amber database **`payment-db`**. | "Instead of forcing analysts to read thousands of lines of raw server logs, SentinelGraph renders the attack path visually. Look at the center canvas: an attacker breached our public web pod, and through lateral movement, they are just **two hops away from our crown-jewel customer payment database**!" | **Visual Sync:** Follow the arrow path slowly with the mouse pointer.<br><br>**Emphasis:** *"two hops away from our crown-jewel payment database"*. |
| **[1:24]** Hover over the dashed boundary banner: **"Blast Radius: 4 Nodes (algo.harmonic: 1.83)"**. | "Our graph algorithm calculates the exact blast radius instantly: four critical assets are currently at risk of total compromise." | **Tone:** Demonstrates mathematical precision without getting bogged in formula details. |

---

### Scene 4: Page 2 — 1-Click Autonomous Threat Mitigation (1:30 – 2:00)
* **Goal:** The dramatic climax of the demo—showing autonomous AI agent response and the instantaneous collapse of the attack surface.

| Visual Action & Screen Cue | Spoken Voiceover Script | Delivery & Timing Notes |
| :--- | :--- | :--- |
| **[1:30]** Move mouse to Column 3 (Right Column: Autonomous Agent Terminal).<br><br>Scroll down slightly through the Agent Triage Dossier showing MCP tool execution logs. | "On the right is our **Autonomous Agent Swarm**, communicating via the Model Context Protocol. The agent has already audited the graph, verified the attack vector, and staged a precision containment plan." | **Tone:** Confident and innovative.<br><br>**Visual:** Show the live agent audit trail. |
| **[1:42]** Center cursor over the prominent blue button: **"Execute Autonomous Mitigation"**.<br><br>**CLICK THE BUTTON.** | "Now watch what happens when we authorize mitigation—in three, two, one..." | **Pacing:** Build dramatic anticipation before the click. |
| **[1:46]** Keep the camera on the screen as the state mutates in real time:<br><br>1. Top status badge turns green: **"QUARANTINE ENFORCED"**.<br>2. Center pod node turns green with an **"ISOLATED"** shield.<br>3. Blast radius banner changes to: **"Blast Radius: Neutralized (0)"**.<br>4. Terminal updates with audit logs: *Calico NetworkPolicy Applied, IAM sa-admin Revoked*. | "Boom! In less than a second, the attack is stopped dead in its tracks. Our autonomous agents quarantined the compromised pod with a Kubernetes network policy, revoked the stolen administrator role, and collapsed the blast radius from four nodes to **zero**—all without disrupting any other legitimate services in the cluster." | **Tone:** Energetic and triumphant.<br><br>**Visual Cue:** Hover over the green "QUARANTINE ENFORCED" badge and the green pod node. |
| **[1:58]** Move cursor up to the top navigation bar and click **"Graph Analytics"**. | "Next, let's see how security teams can freely explore the graph." | **Transition:** Clean click to `/analytics`. |

---

### Scene 5: Page 3 — Graph Analytics Studio & Plain-English Cypher (2:00 – 2:30)
* **Goal:** Show that non-technical users and analysts can query complex infrastructure using 1-click templates with millisecond execution speeds.

| Visual Action & Screen Cue | Spoken Voiceover Script | Delivery & Timing Notes |
| :--- | :--- | :--- |
| **[2:00]** Page `/analytics` loads.<br><br>Point to the top header banner: live graph counter displaying `Graph: sentinel_soc • Nodes: 7 • Edges: 6`. | "Welcome to the **Graph Analytics Studio**. Historically, asking questions about interconnected infrastructure required mastering complex query languages. SentinelGraph makes it accessible with 1-click security templates." | **Tone:** Informative and empowering. |
| **[2:12]** On the Left Sidebar, click the template: **"Bridge Centrality Scan"** (`algo.betweenness`).<br><br>Watch the Cypher query populate the central editor automatically. Click the **"Run Cypher Query"** button. | "With one click, an analyst can run a Bridge Centrality Scan to detect which microservice acts as the most vulnerable bridge between the internet and internal databases. Powered by FalkorDB's GraphBLAS engine, the query executes in just **four milliseconds**!" | **Visual:** Point to the execution timer badge (`~4ms`) next to the editor.<br><br>**Emphasis:** *"four milliseconds!"* |
| **[2:22]** Toggle between **"Table View"** and **"Raw JSON"** tabs in the result pane. Show the ranked list of services. | "We get clean, tabular intelligence showing that our authentication service is the key bottleneck. Security teams can now proactively harden their architecture before an attacker even discovers it." | **Tone:** Professional, highlighting preventative value. |

---

### Scene 6: Conclusion & Hackathon Impact (2:30 – 3:00)
* **Goal:** End with an unforgettable summary of why graph-native cybersecurity changes the industry.

| Visual Action & Screen Cue | Spoken Voiceover Script | Delivery & Timing Notes |
| :--- | :--- | :--- |
| **[2:30]** Navigate back to the homepage (`/`) or SOC Dashboard (`/dashboard`) showing the green "QUARANTINE ENFORCED" system state.<br><br>Cursor rests near the SentinelGraph logo. | "To summarize: attackers don't think in isolated lists of alerts—they think in graphs. SentinelGraph proves that by pairing the high-speed graph intelligence of **FalkorDB** with autonomous AI agents, we can transform security operations from reactive alert fatigue into proactive, autonomous defense." | **Tone:** Inspiring, visionary, and clear.<br><br>**Key Soundbite:** *"Attackers don't think in lists—they think in graphs."* |
| **[2:48]** Display GitHub repository or team credits slide/footer. | "Thank you for watching SentinelGraph—protecting the connected cloud, one relationship at a time." | **Tone:** Warm closing.<br><br>End video cleanly at **~2:55 – 3:00**. |

---

## 🏆 Hackathon Judge Evaluation Alignment Matrix

Use this matrix during video editing and verbal delivery to ensure all judging rubric categories are explicitly hit:

| Track 1 Evaluation Criteria | Where It Appears in the Video | What the Judge Sees on Screen | Key Audio Talking Point |
| :--- | :--- | :--- | :--- |
| **1. FalkorDB Integration** | **0:30 & 2:15** | "Powered by FalkorDB" badge, live health check, and `sentinel_soc` graph space. | *"Powered by FalkorDB—an ultra-low latency graph engine that models your infrastructure like a live subway map."* |
| **2. GraphBLAS Algorithms** | **1:24 & 2:15** | Betweenness Centrality (`algo.betweenness`), Harmonic Centrality (`algo.harmonicCentrality`), and MaxFlow. | *"Calculates exact blast radius using harmonic centrality, executing queries in just four milliseconds."* |
| **3. Autonomous AI Agents (MCP)** | **1:30 – 1:55** | Autonomous Agent Swarm Terminal, explainable Cypher audit trails, and tool calls (`mcp::k8s`, `mcp::iam`). | *"Our autonomous agent swarm communicates via the Model Context Protocol to analyze attack lineage and stage precision containment."* |
| **4. Real-World Business Value** | **1:12 – 1:50** | Visual attack path from breached public Pod -> lateral bridge -> Crown Jewel Payment Database. | *"Collapsed the blast radius from four nodes to zero before customer payment data could be stolen."* |
| **5. Production UX & Polish** | **Throughout (0:00 – 3:00)** | Responsive dark cyber theme, animated visualizer canvas, live tabular result grids, and zero layout shift. | Seamless navigation across Overview, SOC Command Center, and Analytics Studio. |

---

## 🚨 Live Demo & Offline Emergency Fallback Guide

If presenting SentinelGraph live to judges (via Zoom, Google Meet, or an in-person stage) where internet or local Docker services might fluctuate, follow these fail-safe protocols:

### Fallback Scenario 1: Docker / FalkorDB Service Disconnects
- **Built-in Resilience:** SentinelGraph includes an automatic fallback system. If Docker stops, the backend immediately switches to **Local Topology Mode** (`Local Mode Ready`).
- **Talking Point:** *"Notice the health badge displays 'Local Mode Ready'. SentinelGraph is engineered with zero-downtime resilience, maintaining deterministic graph evaluation even during infrastructure failover."*
- **Action:** Continue clicking through the demo exactly as scripted—all algorithms, triage dossiers, and containment triggers will continue functioning deterministically!

### Fallback Scenario 2: Resetting the Scenario for a Second Take
- If you need to re-record or run the demo again for another judge:
  1. Go to `/dashboard`.
  2. Click the **"Reset Breach Scenario"** button in the top right.
  3. The status flips back to red **"ACTIVE EXPLOITATION"**, pod `k8s-pod-77` returns to its breached red state, and the blast radius resets to 4 nodes.
  4. You are instantly ready for another demonstration!

---

## 📝 Speaker's Quick Cheat Sheet (Printable Card)

```
┌────────────────────────────────────────────────────────────────────────┐
│ SENTINELGRAPH DEMO CHEAT SHEET (TARGET: 2:45)                          │
├────────────────────────────────────────────────────────────────────────┤
│ 0:00 - 0:30  HOOK: "Modern attacks cross silos; alert fatigue is real." │
│ 0:30 - 1:00  PAGE 1: FalkorDB is a subway map; click "Seed Graph".    │
│ 1:00 - 1:30  PAGE 2: Breach alert! Hacker is 2 hops from payment-db.   │
│ 1:30 - 2:00  MITIGATION: Click "Execute Autonomous Mitigation". Boom! │
│ 2:00 - 2:30  PAGE 3: Bridge Centrality scan runs in 4 milliseconds.    │
│ 2:30 - 3:00  CLOSE: "Attackers think in graphs. SentinelGraph does too."│
└────────────────────────────────────────────────────────────────────────┘
```
