# Python Logistics Automation — Ramírez Eventos y Logística

**Client:** Ramírez Eventos y Logística, Sogamoso, Boyacá, Colombia
**Period:** January 2024
**Stack:** Python · Pandas · OpenPyXL · GitHub
**Repository:** [Automatizacion-entregas](https://github.com/DavidsOP19/Automatizacion-entregas)

---

## Problem

The company had no standardised system for logistics reporting.
Data was inconsistent — routes named differently by each employee,
no traceability, and no structured capture format.
Generating a weekly report required 3 to 4 hours of manual work.

## Systems Analysis

Before writing any code, a full systems analysis was conducted:
- Identified data quality problems caused by inconsistent nomenclature
- Designed a standardised data capture format with fixed columns and closed value lists
- Eliminated dirty data at the source before processing

## Solution

Built a Python automation script using Pandas and OpenPyXL that:
- Reads raw CSV delivery data
- Consolidates and processes records automatically
- Generates a structured Excel report with multiple sheets:
  - Executive Summary
  - Full Data
  - By Region
  - By Driver

## Results

- Report generation reduced from **3–4 hours to under 1 minute**
- Standardised data capture across the operation
- Replicable and scalable for fleet growth

## Stack

`Python` `Pandas` `OpenPyXL` `CSV` `GitHub`

## Source Code

Full source code available at:
[github.com/DavidsOP19/Automatizacion-entregas](https://github.com/DavidsOP19/Automatizacion-entregas)
