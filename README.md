# CityMind — An Urban Intelligence System

An AI-powered urban simulation built for the AI-2002 course at FAST NUCES.
A 20×20 city grid is populated using Constraint Satisfaction, connected with 
a minimum-cost road network, and simulated with ambulance placement, 
emergency routing, and crime risk prediction.

## Five AI Modules

| Challenge | Algorithm | What it does |
|---|---|---|
| City Layout | CSP + Backtracking + AC-3 | Places hospitals, schools, industrial zones on a grid under hard planning rules |

| Road Network | Kruskal's MST + UCS | Builds minimum-cost roads with a guaranteed backup route between Hospital and Depot |

| Ambulance Placement | Genetic Algorithm | Evolves optimal placement of 3 ambulances to minimise worst-case response time |

| Emergency Routing | A* Search | Routes a medical team to rescue civilians, re-routing in real time when roads flood |

| Crime Prediction | K-Means + Decision Tree | Clusters neighbourhoods and predicts High/Medium/Low crime risk, feeding back into routing costs |

## How to Run

```bash
pip install pygame
python main.py
```

## Controls

| Button | Action |
|---|---|
| Start / Pause | Run simulation automatically (one step per second) |

| Next Step | Advance one step manually |

| Reset | Start fresh with a new city layout |

| Show Roads | Toggle road network overlay |

| Show Coverage | Toggle ambulance coverage overlay |

| Show Heatmap | Toggle crime risk heatmap |

## Tech Stack

- Python 3.9+
- Pygame (UI only)
- All AI algorithms implemented from scratch — no sklearn, no numpy

## Authors

- Haris Said (24I-0527)
- Anoosha Ahsan (24I-0831)

FAST NUCES Islamabad — AI-2002 Semester Project, 2026
