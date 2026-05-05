# Balanced Scorecard System — Restaurante La Popa

**Client:** Restaurante La Popa, Sogamoso, Boyacá, Colombia
**Period:** 2021 — Business Administration degree project (UPTC)
**Tools:** Excel · VBA Macros · Balanced Scorecard methodology

---

## Problem

Restaurante La Popa had no structured system to monitor business
performance. Management decisions were based on intuition with no
measurable indicators, no strategic alignment, and no visibility
over key operational and financial metrics.

## Approach

Before building the system, a full stakeholder analysis was conducted:
- Client interview to identify the restaurant's value proposition
- Definition of strategic objectives across 4 perspectives
- Research and design of 14 KPIs tailored to the client's context
- No pre-built template was used — indicators were built from scratch
  based on the client's operational reality

## Solution

Built a complete Balanced Scorecard management system in Excel with
VBA macros, structured across 4 strategic perspectives:

- **Financial** — Profitability, operational margin, net margin
- **Customers** — Satisfaction, retention, brand awareness
- **Internal Processes** — Service time, innovation, returns
- **Learning & Growth** — Training, employee satisfaction, safety

**Key features:**
- 14 KPIs with individual formulas and measurement frequency
- Automated traffic-light indicators (green/yellow/red) triggered
  by performance thresholds using VBA conditional logic
- Strategic map linking objectives across all 4 perspectives
- SWOT matrix with derived strategic initiatives
- VBA macro activated on file open for system initialisation
- Navigation menu linking all sheets

## System Architecture

CMI_Restaurante_La_POPA/
├── HOME          # Navigation menu + welcome macro
├── DOFA          # SWOT matrix
├── MAPA ESTRATÉGICO  # Strategic map
├── CMI           # Main dashboard with 14 KPIs + traffic lights
├── Persp. Financiera
├── Persp. Clientes
├── Persp. Procesos Internos
└── Persp. Aprendizaje & Crecimiento

## Results

- Management went from intuition-based to indicator-based decisions
- Full strategic visibility across financial, customer, process,
  and learning dimensions
- Replicable system adaptable to other SMEs in the restaurant sector

## Stack

`Excel` `VBA Macros` `Balanced Scorecard` `Kaplan & Norton methodology`

## Evidence

- `bsc-01-welcome-macro.png` — VBA macro activated on file open
- `bsc-02-cmi-completo.png` — Full dashboard with 14 KPIs and traffic lights
- `bsc-03-mapa-estrategico.png` — Strategic map across 4 perspectives
- `bsc-04-vba-code.png` — VBA code in editor
