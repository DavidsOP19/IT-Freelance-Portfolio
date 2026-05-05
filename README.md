# 💼 IT Freelance Portfolio — Oscar David Palacios Chaparro

> Business Administrator with a technical background in Electronics, demonstrating real-world IT skills through freelance consulting projects for Colombian businesses.

---

## 👨‍💻 About Me

I hold a degree in **Business Administration** and a technical diploma in **Electronics**, which gives me a unique ability to bridge business needs with technical solutions. I have been self-taught in software development, data automation, and business intelligence — applying these skills in real freelance projects for actual clients across different industries in Colombia.

My profile combines **business understanding** with **technical execution** — I don't just build solutions, I understand the business problem behind them.

**Core Technical Skills:**
- Python · Pandas · OpenPyXL · Flask · JavaScript
- Power BI · Power Query · DAX · Excel Advanced · VBA Macros
- SQL · Database Administration
- Zapier · Google Workspace · API Integration · AI Agents
- GitHub · VS Code

**Certifications — Daxus LATAM:**
| Course | Status |
|--------|--------|
| Python Fundamentals | ✅ Completed |
| Advanced Python | ✅ Completed |
| Applications with Artificial Intelligence | ✅ Completed |
| SQL Fundamentals | ✅ Completed |
| Advanced SQL | ✅ Completed |
| Database Administration | ✅ Completed |
| Power Query & Data Modelling | ✅ Completed |
| Excel Advanced with Power Pivot | ✅ Completed |
| Agent Automation | ✅ Completed |

---

## 📁 Freelance Projects

---

### 📋 Project 1 — Balanced Scorecard System (VBA)
**Client:** Restaurante La Popa, Sogamoso, Boyacá  
**Period:** 2021 — Business Administration degree (UPTC)  
**Tools:** Excel · VBA Macros · Balanced Scorecard methodology  
**Result:** 14 KPIs · 4 strategic perspectives · Automated traffic-light indicators  
🔗 [View project](./Balanced-Scorecard-VBA)

---

### 📦 Project 2 — Automated Logistics Delivery Reports
**Client:** Ramírez Eventos y Logística, Sogamoso, Boyacá
**Duration:** 4 weeks
**Tools:** Python · Pandas · OpenPyXL · GitHub · CSV

🔗 **Full repository:** [github.com/DavidsOP19/Automatizacion-entregas](https://github.com/DavidsOP19/Automatizacion-entregas)

#### Problem
The company recorded daily deliveries in separate Excel sheets by driver and route. Every week, the supervisor manually consolidated data into a general report — a process taking 3-4 hours, prone to errors, with no real-time visibility on route performance or failed delivery alerts.

#### Solution
Python script that fully automates weekly report generation:
1. Reads CSV files with delivery records
2. Consolidates and cleans data using Pandas
3. Calculates KPIs: total deliveries, success rate, failed deliveries by route
4. Automatically generates a formatted Excel report (.xlsx) with 4 sheets
5. Runs with a single command in under 1 minute

```python
delivery_rate = round((delivered / total_orders) * 100, 1)
avg_days = round(df[df["status"] == "Entregado"]["delivery_time_days"].mean(), 1)

region_summary = df.groupby("region").agg(
    total=("order_id", "count"),
    entregados=("status", lambda x: (x == "Entregado").sum()),
    retrasados=("status", lambda x: (x == "Retrasado").sum()),
    tiempo_promedio=("delivery_time_days", "mean")
).round(1).reset_index()
```

#### Results
- ✅ Report generation time: from 3–4 hours to under 1 minute
- ✅ 4-sheet Excel output: Summary, Data, By Region, By Driver
- ✅ Zero manual consolidation errors
- ✅ Full GitHub repository with documentation

#### Evidence
- `python-01-reporte-excel.png` — Generated Excel report
- `python-02-datos-csv.png` — Source CSV data
- `python-03-codigo-script.png` — Python script code
- `python-04-terminal-ejecucion.png` — Script running in terminal

---

### 🤖 Project 3 — Appointment Automation System
**Client:** Consultorio Estar Natural (Natural Medicine Clinic)
**Duration:** 3 weeks
**Tools:** Google Forms · Google Sheets · Zapier · Gmail

#### Problem
The clinic managed appointments completely manually — patients called by phone, staff wrote in paper or Excel with no automation, and reminders were sent one by one via WhatsApp. This generated an absenteeism rate above 30%, wasted staff time, and made follow-up difficult.

#### Solution
End-to-end automation workflow using no-code tools:
1. Google Form for appointment booking (name, phone, date, time, reason)
2. Google Sheets as central appointment database
3. **Zap 1 — Confirmation:** Trigger on new Google Sheets row → automatic confirmation email to patient via Gmail
4. **Zap 2 — Reminder:** Daily schedule trigger → lookup tomorrow's appointments → send reminder email 24 hours before

#### Results
- ✅ 40% reduction in absenteeism in the first month
- ✅ Staff saved ~2 hours/day previously spent on manual reminders
- ✅ Clinic moved from paper management to a fully digital system at zero software cost
- ✅ 2 active Zaps running in production

#### Evidence
- `zapier-01-google-form.png` — Live Google Form
- `zapier-02-google-sheets-datos.png` — Google Sheets with appointment data
- `zapier-03-flujo-completo.png` — Complete Zapier workflow (both Zaps ON)
- `zapier-04-email-configuracion.png` — Email configuration with dynamic variables

---

### 📊 Project 4 — Sales & Inventory Dashboards in Power BI
**Duration:** 3 weeks per client
**Tools:** Power BI Desktop · Power Query · DAX · Excel

---

#### 4A — La Ruana de Mi Pueblo
**Client:** Artisanal ruana store, Nobsa, Boyacá
**Period:** October 2025 – February 2026

##### Problem
No visibility over product rotation, seasonal patterns, or restocking needs across 19 products and 5 categories. Purchasing decisions were made by intuition.

##### Solution
Interactive Power BI dashboard connected to structured Excel data via Power Query:
- **3 data tables:** Sales (200 records), Products (19 items), Categories (5)
- **DAX Measures:**

- Total Ventas = SUMX(Ventas, Ventas[cantidad] * Ventas[precio_unitario_COP])
Margen Bruto = DIVIDE(Total Ventas - Total Costo, Total Ventas)
Total Unidades = SUM(Ventas[cantidad])

##### Results
- ✅ 20% of products identified as generating 80% of revenue
- ✅ Weekly analysis reduced from 2 hours to 10 minutes
- ✅ Critical stock alerts implemented for 3 key products

---

#### 4B — Lizzmore
**Client:** Children and adult clothing store, Sogamoso, Boyacá
**Period:** January 2025 – March 2026

##### Problem
No visibility over seasonal sales patterns, top-performing categories, or channel performance across 30 products and 6 categories.

##### Solution
Power BI dashboard adapted to fashion retail with 15 months of data:
- **3 data tables:** Sales (350 records), Products (30 items), Categories (6)
- **Channel analysis:** Instagram, WhatsApp Business, Physical Store, Marketplace

##### Results
- ✅ Children's clothing segment (0–12 years) = 32% of total revenue
- ✅ Peak sales months identified: May and December
- ✅ Client shifted from intuition-based to data-driven decisions
- ✅ 350 transactions analysed across 15 months

---

## 🌐 Additional Project — Parce AU

Web application built to help Colombians navigate life in Australia.

**Live:** [parceau.onrender.com](https://parceau.onrender.com)
**Repository:** [github.com/DavidsOP19/Parce-AU](https://github.com/DavidsOP19/Parce-AU)

**Stack:** Python · Flask · Jinja2 · Bootstrap 5 · Vanilla JavaScript · JSON

| Module | Description |
|--------|-------------|
| 🕐 Hour Calculator | Track work hours and monitor fortnightly limits |
| 💰 Financial Tracker | Income, expenses, balance and daily budget |
| ✅ Arrival Checklist | Tasks before and after arriving in Australia |
| 💬 English Templates | Ready-to-copy messages for common situations |
| 📞 Emergency Numbers | Fair Work, Lifeline, and key contacts |
| 🚌 Public Transport | Cards and tips by city |
| ⚖️ Immigration Lawyers | Directory by city with bilingual support |

---

## 📬 Contact

**Email:** oscarpalacios08821@gmail.com  
**GitHub:** [github.com/DavidsOP19](https://github.com/DavidsOP19)

---

*All freelance projects include client certification letters available upon request.*
