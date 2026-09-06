<div align="center">

# 🍽️ Restaurant Booking Agent & ✈️ Travel Agent

### An Intelligent Agent Design Project (PEAS Framework)

![Python](https://img.shields.io/badge/Python-3.10-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Colab](https://img.shields.io/badge/Google%20Colab-Ready-F9AB00?style=for-the-badge&logo=googlecolab&logoColor=white)
![Status](https://img.shields.io/badge/Status-Completed-4CAF50?style=for-the-badge)
![License](https://img.shields.io/badge/License-Academic-blue?style=for-the-badge)

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=2B6CB0&center=true&vCenter=true&width=600&lines=Restaurant+Agent+%F0%9F%8D%B4;Travel+Agent+%E2%9C%88%EF%B8%8F;Built+with+PEAS+Framework;Rule-Based+Intelligent+Agents" alt="Typing SVG" />

</div>

---

## 📌 Overview

This repository contains the complete submission for the **Intelligent Agent Design** assignment. It includes:

- 📄 A full **PDF report** documenting the **Restaurant Booking Agent** — problem formulation, textual & graphical representation, PEAS evaluation, and environmental properties.
- 🐍 A working **Python implementation** of a **Travel Agent** — a rule-based flight booking assistant, built and tested in Google Colab.

<div align="center">

```
┌─────────────────────────────────────────────┐
│   USER  ───▶  AGENT  ───▶  ENVIRONMENT       │
│     ▲                          │             │
│     └──────────  RESPONSE  ◀───┘             │
└─────────────────────────────────────────────┘
```

</div>

---

## 🗂️ Repository Structure

```
📦 restaurant-travel-agents-project
 ┣ 📄 AI_Agent_Report.pdf      → Restaurant Agent: full report (PEAS + flowchart)
 ┣ 📓 travel_agent.ipynb       → Travel Agent: Colab notebook (Python code)
 ┗ 📘 README.md                → You are here
```

---

## 🍴 Agent 1 — Restaurant Booking Agent

> Documented in **`AI_Agent_Report.pdf`**

<table>
<tr><td width="50%" valign="top">

### 🧩 Problem
Booking a table usually means calling ahead or waiting in line. This agent lets a user enter a cuisine/area and books a table automatically.

### 🧠 PEAS Breakdown
| Element | Description |
|---|---|
| 🎯 Performance | Accuracy, speed, successful booking |
| 🌍 Environment | Restaurants, cuisines, ratings, tables |
| 🖥️ Actuators | Display list, confirm booking |
| 👁️ Sensors | User input (cuisine, choice) |

</td><td width="50%" valign="top">

### 🌐 Environment Properties
- 🔸 Partially Observable
- 🔸 Deterministic
- 🔸 Sequential
- 🔸 Static
- 🔸 Discrete
- 🔸 Single-agent

### 📊 Flowchart
See **Figure** in the PDF report for the complete visual flow (START → Search → IF/ELSE → Booking → END).

</td></tr>
</table>

---

## ✈️ Agent 2 — Travel Agent (Flight Booking)

> Implemented in **`travel_agent.ipynb`** — run entirely in Google Colab

```python
def travel_agent():
    print("START")
    departure = input("Enter departure city: ")
    destination = input("Enter destination city: ")
    matches = search_flights(departure, destination)

    if len(matches) == 0:
        print("No flights available")
        print("STOP")
        return
    else:
        display_flights(matches)
        # ... user selects & books a flight
    print("END")
```

<div align="center">

| ✅ Feature | Description |
|:---:|:---|
| 🔍 Search | Matches flights by departure & destination |
| 📋 Display | Shows flight ID + price |
| 🎟️ Book | Confirms booking on selected flight ID |
| ⚠️ Handles | Gracefully manages "no flights found" case |

</div>

### ▶️ How to Run
1. Open the notebook in **Google Colab**
2. Run all cells
3. Enter a departure & destination city when prompted
4. Choose a flight ID from the list to complete booking

---

## 🛠️ Tech Stack

![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/-Jupyter-F37626?style=flat-square&logo=jupyter&logoColor=white)
![GitHub](https://img.shields.io/badge/-GitHub-181717?style=flat-square&logo=github&logoColor=white)
![PDF](https://img.shields.io/badge/-PDF-EC1C24?style=flat-square&logo=adobeacrobatreader&logoColor=white)

---

## 👩‍🎓 Student Info

| Field | Detail |
|---|---|
| **Name** | Huma Shahab |
| **Class** | BS 6A |
| **Section** | A |
| **Seat No** | 23122023 |
| **Date** | 6 Sep 2026 |

---

<div align="center">

⭐ **Thanks for checking out this project!** ⭐ 👋

</div>
