
---
```markdown
#  AI Travel Planner

[![Python](https://img.shields.io/badge/Python-3.10+-blue.svg)](https://python.org)
[![Google Gemini](https://img.shields.io/badge/Google_Gemini-2.5--flash-blueviolet.svg)](https://aistudio.google.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Production_Ready-brightgreen.svg)]()

>  An interactive automated travel curation platform that uses Google Gemini 2.5-Flash JSON configurations to instantly map comprehensive destination guides, build optimized multi-category spending bar charts, extract local cultural guidelines, and output clean markdown trip schedules.

---

##  Table of Contents
- [Overview](#overview)
- [System Architecture](#system-architecture)
- [Key Features](#key-features)
- [Tech Stack](#tech-stack)
- [Jupyter Cell Sequence Blueprint](#jupyter-cell-sequence-blueprint)
- [Installation & Environment Setup](#installation--environment-setup)
- [Project Directory Architecture](#project-directory-architecture)
- [License](#license)

---

##  Overview

The AI Travel Planner tool helps travelers bypass the stress of coordinating multi-day vacations. By running structured JSON contextual inquiries across destination constraints, budget caps, traveler volumes, and specialized styles, it algorithmically maps ideal morning/afternoon/evening schedules, plots local expenditure forecasts, and compiles custom packing checklists.

---

##  System Architecture




User Trip Preferences Input
│
▼
┌────────────────────────────────────────────────────────┐
│         Gemini 2.5-Flash Analytical Engine             │
│  ┌───────────────────────┐ ┌────────────────────────┐  │
│  │ Destination Researcher│ │ Daily Activity Planner │  │
│  └───────────────────────┘ └────────────────────────┘  │
│  ┌───────────────────────┐ ┌────────────────────────┐  │
│  │ Packing Checklist Gen │ │ Cultural Tip Extractor │  │
│  └───────────────────────┘ └────────────────────────┘  │
└──────────────────────────┬─────────────────────────────┘
│
▼
┌────────────────────────────────────────────────────────┐
│         Interactive UI Layout Outputs (Gradio)         │
│  ┌───────────────────────┐ ┌────────────────────────┐  │
│  │ Day-By-Day Itinerary  │ │ Matplotlib Budget Pie  │  │
│  └───────────────────────┘ └────────────────────────┘  │
│  ┌───────────────────────┐ ┌────────────────────────┐  │
│  │ Packing List Panel    │ │ Markdown Document File │  │
│  └───────────────────────┘ └────────────────────────┘  │
└────────────────────────────────────────────────────────┘

```

---

##  Key Features

* **AI Destination Insights Compiler:** Discovers local landmarks, cuisine standouts, transit suggestions, and safety advisories using structured JSON interfaces.
* **Automated Financial Category Balancer:** Automatically groups spending across accommodation, transit, and food, generating visual tracking bar charts saved to `output/`.
* **Adaptive Itinerary Layout Builder:** Splits plans into organized morning, afternoon, and evening slots while matching designated traveler styles and interests.
* **Smart Context Packing Lists:** Generates targeted clothing and accessory guidelines adjusted to the specific duration, season, and climate of your selected city.
* **Clean Markdown Exporter:** Automatically compiles structured schedules and logs them out directly into a clean markdown format file inside `output/`.

---

##  Tech Stack

* **AI Processing Engine:** Google Gemini 2.5-Flash (`google-generativeai`)
* **Visual Presentation Interface:** Gradio Blocks Dashboard Grid (Gradio 6.0+ compatible)
* **Graphical Representation Layer:** Matplotlib Plotting Components
* **Data Processing Models:** Pandas DataFrames & NumPy Matrix Fields
* **Mapping Frameworks:** Folium Map Generators & GeoPy Location Resolvers

---

##  Jupyter Cell Sequence Blueprint

The notebook follows a clear step-by-step modular development loop:

| Cell # | Type | Target Module Context | Technical Core Purpose |
| :--- | :--- | :--- | :--- |
| **Cell 1** |  Markdown | **Project Introduction** | System summary badges, feature indices, and blueprint architectures. |
| **Cell 2** |  Code | **Package Downloads** | Silent environment hydrations (`%pip install`) of GenAI, geopy, and UI frameworks. |
| **Cell 3** |  Code | **Global Initializations** | Standard imports, data classes configuration blueprints, and API settings. |
| **Cell 4** |  Code | **Destination Researcher** | Implements the `DestinationResearcher` tool parsing JSON culture data blocks. |
| **Cell 5** |  Code | **Itinerary Generation** | Implements `ItineraryBuilder` class with bar plotting budget algorithms. |
| **Cell 6** |  Code | **Orchestrator Pipeline Agent** | Defines `AITravelPlannerAgent` orchestrating workflows and file exports. |
| **Cell 7** |  Code | **Verification Demo Run** | Runs system diagnostics using a mock beach vacation scenario framework. |
| **Cell 8** |  Code | **Gradio Interface App** | Mounts individual input metadata configurations panels directly into browser displays. |

---

##  Installation & Environment Setup
```

### 1. Deploy Dependencies Manifest

Create a `requirements.txt` file inside your folder matching the project specifications, then run:

```bash
pip install -r requirements.txt

```

### 2. Setup Gemini Access Token

Get a free API access key directly from [Google AI Studio](https://aistudio.google.com/). Paste your secret key parameter inside **Cell 3** configuration rows:

```python
os.environ["GEMINI_API_KEY"] = "AIzaSyYourSecretKeyStringHere"

```

---

##  Project Directory Architecture

```text
AI_Travel_Planner/
├── notebooks/
│   └── AI_Travel_Planner.ipynb    # Main interactive development notebook workspace
├── output/  
├── .gitignore                     # Git configuration element tracking blocks
├── README.md                      # Comprehensive system documentation (This file)
└── requirements.txt               # Pinned application dependencies manifest

```

---

##  Author

**Divya** — AI/ML Developer |

