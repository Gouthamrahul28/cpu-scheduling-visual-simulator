# CPU Scheduling Visual Simulator

[![Live Demo](https://img.shields.io/badge/demo-online-brightgreen.svg)](https://gouthamrahul28.github.io/cpu-scheduling-visual-simulator/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

An interactive, zero-dependency web-based **CPU Scheduling Visual Simulator** designed for Operating Systems lab courses, viva preparation, and self-study.

🔗 **Live Link / Demo**: [https://gouthamrahul28.github.io/cpu-scheduling-visual-simulator/](https://gouthamrahul28.github.io/cpu-scheduling-visual-simulator/)

---

## 🚀 Features

- **5 CPU Scheduling Algorithms**:
  1. **FCFS** (First Come First Served) – Non-preemptive
  2. **SJF** (Shortest Job First) – Non-preemptive
  3. **Round Robin** (RR) – Preemptive with customizable time quantum
  4. **SRTF** (Shortest Remaining Time First) – Preemptive SJF
  5. **MLFQ** (Multi-Level Feedback Queue) – 3 priority queues (quanta: 2, 4, 8)
- **Interactive Gantt Chart**:
  - Color-coded process blocks with exact start and finish timestamps
  - CPU idle period detection and display
  - Interactive step-by-step highlighting (`Highlight next step`) that syncs with the operation log
- **Automated Performance Metrics**:
  - Completion Time ($CT$)
  - Turnaround Time ($TAT = CT - AT$)
  - Waiting Time ($WT = TAT - BT$)
  - Average Turnaround Time and Average Waiting Time
- **Real-Time Operation Log**:
  - Granular trace of every arrival, CPU dispatch, preemption, quantum expiry, and process termination
- **OS Lab Companion & Viva Guide**:
  - Tabbed laboratory reference covering:
    - **AIM & Procedure**
    - **Pseudocode & Logic**
    - **Standard C Program (FCFS)**
    - **Sample Input / Output verification**
    - **Frequently Asked Viva Questions (FAQ)**

---

## 💻 Quick Start / Local Setup

No build tools or server dependencies required!

### Option 1: Direct File
Simply clone the repository and double-click `index.html` in any browser:
```bash
git clone https://github.com/Gouthamrahul28/cpu-scheduling-visual-simulator.git
cd cpu-scheduling-visual-simulator
# Open index.html in your default browser
start index.html     # On Windows
open index.html      # On macOS
xdg-open index.html  # On Linux
```

### Option 2: Local HTTP Server (Optional)
```bash
npx serve .
# or
python -m http.server 8000
```

---

## 📊 Scheduling Formula Reference

| Metric | Formula | Description |
|---|---|---|
| **Turnaround Time (TAT)** | $TAT = CT - AT$ | Total time from process arrival to final completion |
| **Waiting Time (WT)** | $WT = TAT - BT$ | Total time the process spent waiting in the ready queue |
| **Response Time (RT)** | $RT = \text{First CPU Time} - AT$ | Time from arrival until first CPU allocation |

---

## 📜 License
Distributed under the MIT License. Feel free to use for academic, laboratory, and educational purposes.
