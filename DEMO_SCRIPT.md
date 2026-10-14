# SentinelGraph: Master Demo Video Script & Production Walkthrough
> **Tailored for Hackathon Evaluators, Technical Judges, and Executive Audiences**  
> **Total Target Video Runtime:** Exactly **03:30** (3 minutes and 30 seconds / 210 seconds)  
> **Target Speaking Pace:** 135 words per minute (Clear, confident, authoritative narration)  
> **Total Spoken Word Count:** ~475 words (Strictly calibrated to finish at 03:25 – 03:30)

---

## ⏱️ Video Timeline & Structure Overview

```
0:00 ────── 1. Introduction & FalkorDB Architecture (60s / ~135 words) ────── 1:00
1:00 ────── 2. Page 1: Landing / Overview Screen (45s / ~102 words) ───────── 1:45
1:45 ────── 3. Page 2: SOC Dashboard & Autonomous Mitigation (60s / ~138 words) 2:45
2:45 ────── 4. Page 3: Graph Analytics & Production Cloud Close (45s / ~100 words) 3:30
```

---

## 🎬 Pre-Recording Checklist & Technical Setup

### 1. Browser & Display Standards
- **Resolution:** Full HD **1080p (1920x1080)** with browser zoom set strictly to **100%**.
- **Clean Recording Canvas:** Hide the bookmarks bar (`Ctrl+Shift+B` or `Cmd+Shift+B`), close unrelated tabs, and silence all OS notifications.
- **Cursor Visibility:** In OBS Studio, Loom, or Camtasia, enable **mouse cursor click highlighting** (or a subtle glowing halo) so viewers can follow your clicks effortlessly.
- **Target URL:** Live production deployment at [https://sentinel-graph-orcin.vercel.app](https://sentinel-graph-orcin.vercel.app) (or local dev server `http://localhost:3000`).

### 2. Clean Starting State
1. Open the **SOC Dashboard** (`/dashboard`).
2. If the status badge displays green *"QUARANTINE ENFORCED"*, click the **"Reset Breach Scenario"** button in the top right to restore the active breach state.
3. Verify the flashing red status badge reads: **"ACTIVE EXPLOITATION"**.
4. Navigate back to the **Overview Page** (`/`) to begin recording at timestamp `0:00`.

---

## 🎙️ Master Dual-Column Teleprompter Script

---

### Part 1: Introduction & Architecture (0:00 – 1:00 | 60 Seconds)
* **Goal:** Demystify modern cloud risk, introduce SentinelGraph, and explain why FalkorDB's graph-native engine is foundational for autonomous security swarms.
* **Word Count:** 135 words (~60 seconds at 135 wpm).

| Timestamp & Screen Recording Cue | Spoken Voiceover Narration | Delivery, Tone & Inflection Directives |
| :--- | :--- | :--- |
| **[0:00 – 0:15]**<br>Full screen showing the SentinelGraph hero screen.<br><br>The cursor rests comfortably below the animated gradient title: *"SentinelGraph: Autonomous Multi-Agent Security SOC"*.<br><br>Gently scroll down to reveal the four architecture capability cards. | "Modern enterprises operate across distributed cloud environments—connecting container workloads, permissions, and databases. But when attacks occur, traditional security tools create a massive blind spot: they trigger hundreds of disconnected alerts without understanding the big picture." | **Tone:** Engaging, serious, and authoritative.<br><br>**Pacing:** Steady and measured.<br><br>**Emphasis:** *"hundreds of disconnected alerts without understanding the big picture"*. |
| **[0:15 – 0:30]**<br>Slowly scroll back up to the top hero section.<br><br>Hover over the pulsing status badge: **"Powered by FalkorDB"**.<br><br>Cursor circles smoothly around the subtitle mentioning autonomous agent swarms. | "Tracing how an attacker moves laterally across infrastructure still takes security teams hours or days—and by then, critical data is already gone. That's why we created **SentinelGraph**: an autonomous, graph-native Security Operations Center." | **Transition:** Pivot with energy from the problem statement to the solution.<br><br>[Brief 0.5s pause before deep dive]. |
| **[0:30 – 1:00]**<br>Highlight the architecture badges on screen.<br><br>Gesture cursor between the capability cards: *Real-Time Attack Graph Traversal*, *FalkorDB Centrality Algorithms*, and *Autonomous Agent Swarm (MCP)*. | "At its foundation, SentinelGraph uses **FalkorDB**—an ultra-low latency graph database powered by GraphBLAS sparse matrix linear algebra. FalkorDB continuously correlates Kubernetes pods, privileged cloud IAM credentials, and zero-day CVEs into a live security knowledge graph. When combined with autonomous AI agents via the Model Context Protocol, SentinelGraph instantly evaluates multi-hop attack paths and calculates blast radius with sub-ten-millisecond execution speeds." | **Tone:** Technical, confident, and visionary.<br><br>**Key Terminology:** Crisp delivery on *"GraphBLAS sparse matrix linear algebra"*, *"Model Context Protocol"*, and *"sub-ten-millisecond speeds"*. |

---

### Part 2: First Page Walkthrough / Overview (1:00 – 1:45 | 45 Seconds)
* **Goal:** Tour the Landing/Overview interface, explain the navigation structure and status badges, and demonstrate interactive 1-click database seeding.
* **Word Count:** 102 words (~45 seconds at 135 wpm).

| Timestamp & Screen Recording Cue | Spoken Voiceover Narration | Delivery, Tone & Inflection Directives |
| :--- | :--- | :--- |
| **[1:00 – 1:20]**<br>Focus on the top persistent cyber navigation bar.<br><br>Point cursor to the brand logo **"SG • SentinelGraph SOC v0.1"** on the left.<br><br>Hover over the three navigation links: **Overview**, **SOC Dashboard**, and **Graph Analytics**.<br><br>Scroll down slightly to the **Dynamic Security Topology Snapshot**. | "Starting on our Landing and Overview page, the interface immediately establishes complete situational awareness. At the top, our persistent cyber navigation bar gives instant access to Overview, the SOC Dashboard, and Graph Analytics. The hero section highlights our live engine readiness, confirming that our autonomous agent swarms and graph backend are actively synchronized." | **Tone:** Clear, welcoming, and structured.<br><br>**Pacing:** Smooth, synchronizing cursor movement with each mentioned navigation item. |
| **[1:20 – 1:45]**<br>Hover sequentially over the 4 live statistic pills:<br>1. *Active Pods (3)*<br>2. *IAM Identities (2)*<br>3. *Zero-Day CVEs (2)*<br>4. *Blast Radius Nodes (7)*.<br><br>**CLICK** the purple button: **"Seed Security Graph"**.<br><br>Watch the cyber toast notification slide in: *"Security Graph Re-seeded: Initialized 7 nodes and 6 relationships"*. | "Directly below, the Dynamic Security Topology Snapshot displays live infrastructure counters: three active workloads, two IAM identities, two zero-day vulnerabilities, and seven connected assets. With a single click on 'Seed Security Graph', our backend instantly compiles and verifies our entire Kubernetes and cloud topology in FalkorDB. Now, let's step into the SOC Dashboard." | **Action Sync:** Click the button right as you say *"With a single click"*. Allow 1 second for viewers to read the toast notification.<br><br>**Transition:** Click the blue **"Launch SOC Dashboard"** button at 1:44. |

---

### Part 3: Second Page Walkthrough / SOC Dashboard (1:45 – 2:45 | 60 Seconds)
* **Goal:** Showcase the live breach scenario, explain the 3-column command center, demonstrate autonomous agent reasoning, and execute 1-click containment.
* **Word Count:** 138 words (~60 seconds at 135 wpm).

| Timestamp & Screen Recording Cue | Spoken Voiceover Narration | Delivery, Tone & Inflection Directives |
| :--- | :--- | :--- |
| **[1:45 – 2:05]**<br>The `/dashboard` page loads.<br><br>Point to the top header: the flashing red status badge reads: **"ACTIVE EXPLOITATION"**.<br><br>Move cursor to Column 1 (Left: Incident Queue). Hover over **Incident INC-2026-7701** (CVSS 9.8, Remote Code Execution in Ingress Pod). | "Entering the SOC Dashboard, an active breach has triggered. On the left, our threat feed flags Incident 7701: a critical Remote Code Execution exploit scoring a maximum CVSS 9.8." | **Tone:** Urgent, focused, and immersive.<br><br>**Pacing:** Deliberate; draw viewer attention to the severity metrics. |
| **[2:05 – 2:20]**<br>Move mouse to Column 2 (Center: Visualizer Canvas).<br><br>Hover over the red compromised node: `k8s-pod-77`.<br><br>Follow the directional attack arrows:<br>`dev-praveen` ➔ `sa-admin` ➔ `k8s-pod-77` ➔ `auth-service` ➔ amber cylinder `payment-db`.<br><br>Hover over the dashed boundary banner: *"Blast Radius: 4 Nodes (algo.harmonic: 1.83)"*. | "In the center canvas, SentinelGraph visualizes the multi-hop attack trajectory: the attacker breached our ingress pod and is just two hops from our crown-jewel customer payment database. Our FalkorDB harmonic algorithm calculates an active blast radius of four vulnerable assets." | **Visual Sync:** Trace the attack path slowly with your cursor.<br><br>**Vocal Emphasis:** *"two hops from our crown-jewel customer payment database"*. |
| **[2:20 – 2:32]**<br>Move mouse to Column 3 (Right: Autonomous Agent Terminal).<br><br>Scroll through the live MCP traces showing Step 1 (graph query), Step 2 (betweenness bridge detection), and Step 3 (harmonic blast radius). | "On the right, our Autonomous Agent Terminal has already audited the graph using Model Context Protocol tools, mapped the MITRE tactics, and staged a precision mitigation plan." | **Tone:** Professional and technically reassuring. |
| **[2:32 – 2:45]**<br>Hover directly over the blue button: **"Execute Autonomous Mitigation"**.<br><br>**CLICK THE BUTTON AT 2:34.**<br><br>Watch the UI mutate in real time:<br>1. Status flips to green **"QUARANTINE ENFORCED"**.<br>2. Center pod turns green with **"ISOLATED"** shield.<br>3. Blast radius banner displays: **"Neutralized (0)"**.<br>4. Terminal records *Calico NetworkPolicy Applied, IAM Revoked*. | "Watch what happens when I click 'Execute Autonomous Mitigation'. Instantly, the status badge turns green to 'QUARANTINE ENFORCED'. Our agents quarantined the compromised pod, revoked the stolen administrator role, and collapsed the blast radius from four assets to zero—all in milliseconds." | **Pacing:** Build anticipation before the click, then speak with energetic triumph as the state flips to green.<br><br>**Visual Pause:** Linger 1.5 seconds on the green quarantined pod. |

---

### Part 4: Third Page Walkthrough / Graph Analytics & Conclusion (2:45 – 3:30 | 45 Seconds)
* **Goal:** Demonstrate interactive Cypher query execution with sub-10ms GraphBLAS benchmarks, highlight production cloud deployment, and deliver a memorable closing.
* **Word Count:** 100 words (~45 seconds at 135 wpm).

| Timestamp & Screen Recording Cue | Spoken Voiceover Narration | Delivery, Tone & Inflection Directives |
| :--- | :--- | :--- |
| **[2:45 – 3:10]**<br>Click **"Graph Analytics"** in the top navigation bar.<br><br>The `/analytics` page loads.<br><br>On the Left Sidebar, click the template: **"Bridge Centrality Scan"** (`algo.betweenness`).<br><br>Click **"Run Cypher Query"**.<br><br>Point to the execution latency badge: **"~4.0 ms"**.<br><br>Toggle between **"Table View"** and **"Raw JSON"** tabs. | "Moving to the Graph Analytics Studio, security analysts can explore infrastructure relationships using plain-English Cypher templates. With one click, I run a Bridge Centrality Scan using FalkorDB's betweenness algorithm. Executing in just four milliseconds, it pinpoints our authentication service as the critical lateral chokepoint, allowing teams to proactively harden infrastructure before an exploit occurs." | **Tone:** Inspiring, crisp, and analytical.<br><br>**Emphasis:** *"Executing in just four milliseconds"*.<br><br>**Visual:** Show the clean tabular result rows with column headers. |
| **[3:10 – 3:30]**<br>Navigate smoothly back to the overview screen or show the deployed URL bar: `https://sentinel-graph-orcin.vercel.app`.<br><br>Highlight the footer stating: *SentinelGraph Security Operations Center • FalkorDB + MCP Swarm*.<br><br>Cursor rests near the glowing SG brand logo. | "SentinelGraph is fully production-ready: deployed globally on Vercel, powered by a FastAPI backend on Render, and connected to high-availability FalkorDB Cloud. Attackers don't think in isolated alerts—they think in graphs. With SentinelGraph, modern security teams finally do too. Thank you." | **Tone:** Confident, visionary, and decisive.<br><br>**Signature Soundbite:** *"Attackers don't think in isolated alerts—they think in graphs."*<br><br>**Ending:** Warm closing, fade to black at **03:28 – 03:30**. |

---

## 🏆 Hackathon Judge Evaluation Alignment Matrix

Use this matrix to confirm that all Hackathon Track 1 judging criteria are explicitly articulated:

| Rubric Evaluation Item | Timestamp in Video | Exact Visual Cue Shown | Spoken Narration Alignment |
| :--- | :---: | :--- | :--- |
| **1. FalkorDB Deep Integration** | **0:30 & 2:55** | "Powered by FalkorDB" badge, live query latency (`~4ms`), and GraphBLAS specs. | *"Powered by FalkorDB—an ultra-low latency graph database using GraphBLAS sparse matrix linear algebra."* |
| **2. GraphBLAS Algorithms** | **2:15 & 2:55** | Betweenness Centrality (`algo.betweenness`) and Harmonic Centrality (`algo.harmonicCentrality`). | *"Our FalkorDB harmonic algorithm calculates an active blast radius of four vulnerable assets... betweenness pinpoints our bridge service."* |
| **3. Autonomous MCP Agents** | **2:20 – 2:40** | Autonomous Agent Terminal, MCP tool traces (`mcp::k8s`, `mcp::iam`), and reasoning dossier. | *"Our agent swarm communicates via the Model Context Protocol to analyze attack lineage and stage precision containment."* |
| **4. Real-World Business Value** | **2:05 – 2:42** | Multi-hop attack path toward customer financial database (`payment-db`) and 1-click mitigation. | *"The attacker is just two hops from our crown-jewel payment database... collapsed the blast radius from four assets to zero."* |
| **5. Production Cloud Deployment** | **3:10 – 3:25** | Vercel URL bar, live Render API health check, and FalkorDB Cloud connectivity. | *"Deployed globally on Vercel, powered by a FastAPI backend on Render, and connected to high-availability FalkorDB Cloud."* |

---

## 🚨 Live Demo & Fallback Scenario Guide

### Scenario 1: Re-Recording a Second Take
1. If you need to record another take or reset the scenario:
   - Navigate to `/dashboard`.
   - Click the **"Reset Breach Scenario"** button in the top right.
   - The status badge returns to red **"ACTIVE EXPLOITATION"**, pod `k8s-pod-77` returns to its breached state, and the blast radius resets to 4 nodes.
   - Click **"Overview"** in the navbar to begin from `0:00`.

### Scenario 2: Offline / Local Docker Presentation
- SentinelGraph features built-in fallback resilience. If internet connectivity drops, the application continues functioning deterministically with zero UI downtime.

---

## 📝 Speaker's Printable 4-Line Teleprompter Card

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│ SENTINELGRAPH DEMO SCRIPT CHEAT SHEET (TARGET: EXACTLY 03:30)                          │
├────────────────────────────────────────────────────────────────────────────────────────┤
│ 0:00 - 1:00  INTRO: "Siloed alerts create blind spots. FalkorDB + MCP connects them." │
│ 1:00 - 1:45  PAGE 1: Tour Overview, verify live counters, click "Seed Security Graph".│
│ 1:45 - 2:45  PAGE 2: Breach active! Hacker 2 hops from payment-db. Click Contain!     │
│ 2:45 - 3:30  PAGE 3: 4ms Bridge Scan. Live on Vercel + Render. "Attackers think in    │
│                      graphs—now security teams do too."                                │
└────────────────────────────────────────────────────────────────────────────────────────┘
```
