# Volunteer Shift Scheduling Optimizer

**Saudi Red Crescent Authority – Madinah Volunteer Affairs Department**
**Internal Use Only**

<p align="center">
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Algorithm-Deterministic%20Greedy-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Backend-Python 3.x-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Frontend-HTML%20%7C%20CSS%20%7C%20JS-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/UI-PyWebView-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Excel Export-Yes-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Confidential-Internal Only-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Volunteers-500%2B-brightgreen?style=for-the-badge" />
</p>

---

## Overview

This project is a purpose-built scheduling system for the
**Saudi Red Crescent Authority – Madinah Volunteer Department**, designed to modernize EMS volunteer shift management in one of the most demanding operational environments in the world.

With **≈500 volunteers** serving inside **Al-Masjid An-Nabawi**, scheduling isn’t just paperwork — it’s a time-intensive task that requires fairness, accuracy, and speed.

This system replaces the old manual, fully random process with a **deterministic, preference-aware workflow**, making planning efficient, consistent, and fair.

---

## The Problem It Solves

Before this system:

* ❌ Schedules were created **fully manually**
* ❌ Assignments were **random**, ignoring volunteer availability and preferences
* ❌ Shift distribution may become unintentionally **unbalanced**
* ❌ Supervisors spent **hours** arranging and rearranging names
* ❌ Managing **≈500 volunteers** was exhausting
* ❌ Last-minute adjustments added more strain

The previous system **worked**, but as the volunteer pool grew, it became grueling and inefficient.
This project brings **structure, fairness, and automation** to a workflow that had been chaotic and labor-intensive.

---

## Why It Matters

Inside **Al-Masjid An-Nabawi**, particularly during **Ramadan** and **Hajj**:

* Volunteer counts surge past **500 active members**
* Peak crowds reaches almost **1.5 million worshippers**
* Daily operational tempo is extremely high
* Schedules must be created **quickly and fairly**

By automating scheduling:

* ⚡ Schedules are generated instantly
* 🎯 Volunteer availability and preferences are respected
* 📊 Shifts are distributed fairly and consistently
* 🧭 Hundreds of volunteers are handled without slowing down
* 💼 Hours of repetitive manual work are eliminated
* 🧠 Supervisor workload is significantly reduced

This system **optimizes the workflow**, not because the old system was unsafe, but because it was too exhausting to maintain at scale.

---

## Key Features

### 🔹 Deterministic Greedy Scheduling

* Fair, consistent assignments every time
* Same inputs → same outputs

### 🔹 Load Balancing

* Volunteers with fewer shifts are prioritized automatically

### 🔹 Preference-Aware Assignments

* Assignments respect volunteer availability and preferences

### 🔹 Excel Export

* Clean, styled `.xlsx` files
* Shift coloring (Morning/Evening)
* Role separation
* Weekly summaries
* Legend row
* logo embedding
* Safe export even if logo is missing

### 🔹 Modern Desktop UI

* Built with **HTML, CSS, JavaScript**, displayed via **PyWebView**
* Non-blocking modals and inline notifications
* Safe reset flows
* File path prompts and keyboard shortcuts

### 🔹 State Persistence

* Saves current schedule and UI state in JSON
* Safe reset without accidental data loss

---

## Tech Stack

**Backend:** Python 3.x, Pandas, NumPy, OpenPyXL, PyBidView, ExcelListWriter
**Frontend:** HTML, CSS, JavaScript, PyWebView
**Data Layer:** JSON persistence, Excel export

---

## High-Level Architecture

```
┌────────────────────┐
│  HTML / CSS / JS   │  ← UI Layer (Frontend)
└─────────┬──────────┘
          │ PyWebView Bridge
┌─────────▼──────────┐
│   Python Backend    │  ← Scheduling engine
│  (Deterministic     │
│   Greedy Algorithm) │
└─────────┬──────────┘
          │
┌─────────▼──────────┐
│ Excel Export System │  ← Styled .xlsx output
└─────────────────────┘
```

---

## Workflow

1. Input volunteer availability & preferences
2. Run the scheduling algorithm
3. Display results in the UI
4. Export to Excel for review and deployment

---

## Repository Purpose

This repository exists to document the system
> ⚠️ **The operational code is intentionally withheld** for confidentiality.
> Only the README and documentation are included.

---

🔹 Development Notes

This project was developed using a heavily AI-assisted workflow, combined with hands-on coding by me.
Core parts of the system were written manually, while AI tools were used throughout development to help generate, refine, debug, refactor, and document code. The overall structure, feature set, and operational logic were guided by real-world volunteer and EMS requirements, with AI acting as an accelerator rather than a replacement.
The final stage focused on code cleanup, readability, and adding comments/notes, with AI support to improve maintainability.

---

## Confidentiality Notice

This project is for **internal use** within the
**Saudi Red Crescent Authority – Madinah Branch**.
