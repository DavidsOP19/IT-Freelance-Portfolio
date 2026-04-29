# 💼 IT Freelance Portfolio — Oscar David Palacios Chaparro

> Business Administrator with a technical background in Electronics, demonstrating real-world IT skills through freelance consulting projects for Colombian businesses.

---

## 👨‍💻 About Me

I hold a degree in **Business Administration** and a technical diploma in **Electronics**, which gives me a unique ability to bridge business needs with technical solutions. I have been self-taught in software development, data automation, and business intelligence — applying these skills in real freelance projects for actual clients across different industries in Colombia.

My profile combines **business understanding** with **technical execution** — I don't just build solutions, I understand the business problem behind them.

**Core Technical Skills:**
- Python · Pandas · OpenPyXL · Flask · JavaScript
- Power BI · Power Query · DAX · Excel Advanced
- SQL · Database Administration
- Zapier · Google Workspace · API Integration · AI Agents
- GitHub · VS Code · Claude Code

**Certifications — Daxus LATAM:**
| Course | Status |
|--------|--------|
| Python Fundamentals | ✅ Completed |
| Advanced Python | ✅ Completed |
| Applications with Artificial Intelligence | ✅ Completed |
| SQL Fundamentals | ✅ Completed |
| Advanced SQL | ✅ Completed |
| Database Administration | ✅ Completed |
| Mastering Power Query and Data Modeling | 🔄 88% |
| Agent Automation | 🔄 84% |
| Dashboard Design | 🔄 58% |

---

## 📁 Freelance Projects

---

### 🤖 Project 1 — Appointment Automation System
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
- `zapier-01-google-form.png` — Live Google Form (Published)
- `zapier-02-google-sheets-datos.png` — Google Sheets with real appointment data
- `zapier-03-flujo-completo.png` — Complete Zapier workflow (both Zaps ON)
- `zapier-04-email-configuracion.png` — Email configuration with dynamic variables

---

### 📦 Project 2 — Automated Logistics Delivery Reports
**Client:** Logistics / Transport Company
**Duration:** 4 weeks
**Tools:** Python · Pandas · OpenPyXL · GitHub · CSV

🔗 **Full repository:** [github.com/DavidsOP19/Automatizacion-entregas](https://github.com/DavidsOP19/Automatizacion-entregas)

#### Problem
The company recorded daily deliveries in separate Excel sheets by driver and route. Every week, the supervisor manually consolidated data into a general report — a process taking 3-4 hours, prone to errors, with no real-time visibility on route performance or failed delivery alerts.

#### Solution
Python script that fully automates weekly report generation:
1. Reads CSV files with delivery records (date, driver, route, status, client)
2. Consolidates and cleans data using Pandas
3. Calculates KPIs: total deliveries, success rate, failed deliveries by route
4. Automatically generates a formatted Excel report (.xlsx) with 4 sheets
5. Runs with a single command and produces the report in under 30 seconds
6. Code versioned and documented on GitHub

```python
# Key metrics calculated automatically
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
- ✅ Report generation time: from 3-4 hours to under 1 minute
- ✅ 68% delivery success rate tracked automatically
- ✅ 4-sheet Excel output: Summary, Data, By Region, By Driver
- ✅ Zero manual consolidation errors
- ✅ Full GitHub repository with documentation

#### Evidence
- `python-01-reporte-excel.png` — Generated Excel report with 4 sheets
- `python-02-datos-csv.png` — Source CSV data in VS Code
- `python-03-codigo-script.png` — Python script code
- `python-04-terminal-ejecucion.png` — Script running in terminal with output

---

### 📊 Project 3 — Sales & Inventory Dashboard in Power BI
**Duration:** 3 weeks per client
**Tools:** Power BI Desktop · Power Query · DAX · Excel

Same BI solution architecture successfully applied to **two different Colombian businesses**, demonstrating adaptability and reusability of technical solutions.

---

#### 3A — La Ruana de Mi Pueblo
**Client:** Artisanal wool ruana shop — Nobsa, Boyacá, Colombia
**Period:** October 2025 – March 2026

##### Problem
The owner tracked sales and inventory in unstructured Excel sheets updated manually. No quick way to identify which products rotated most, which seasons concentrated sales, or when to restock. Purchasing decisions were made by intuition, generating excess stock in some products and shortages in the most demanded ones.

##### Solution
Interactive Power BI dashboard connected to structured Excel data via Power Query:
- **3 data tables:** Sales (200 records), Products (19 items), Categories (5)
- **DAX Measures:**
```
Total Ventas = SUMX(Ventas, Ventas[cantidad] * Ventas[precio_unitario_COP])
Margen Bruto = DIVIDE(Total Ventas - Total Costo, Total Ventas)
Total Unidades = SUM(Ventas[cantidad])
```

##### Dashboard Features
- 📈 Line chart — Monthly revenue (Oct 2025 – Mar 2026)
- 📊 Bar chart — Top 10 products by revenue
- 🍩 Donut chart — Sales by category (5 categories)
- 📋 Table — Critical stock inventory with minimum stock alerts
- 🎛️ Interactive slicers — Date range + Category filter

##### Results
- ✅ Owner identified that 20% of products generate 80% of revenue
- ✅ Weekly analysis time reduced from 2 hours to 10 minutes
- ✅ 3 critical stock products identified before causing lost sales
- ✅ December Christmas peak and cold season (Oct-Nov) clearly visible

##### Real Market Prices (Boyacá, Colombia 2025-2026)
| Category | Price Range (COP) |
|----------|------------------|
| Traditional Ruanas | $140,000 – $190,000 |
| Executive Ruanas | $265,000 – $420,000 |
| Children's Line | $90,000 – $115,000 |
| Wool Accessories | $42,000 – $230,000 |
| Special Edition | $345,000 – $490,000 |

---

#### 3B — Lizzmore
**Client:** Baby (0-12 years) and adult clothing store, Colombia
**Period:** January 2025 – March 2026 (15 months)

##### Problem
No visibility on seasonal sales patterns, top-performing categories, or inventory health across 30+ products and 6 categories. No data-driven insight into which lines (baby vs adult) generated the most revenue or which months drove peak sales.

##### Solution
Same Power BI architecture adapted to fashion retail with 15 months of data:
- **3 data tables:** Sales (350 records), Products (30 items), Categories (6)
- **Seasonal peaks:** May (Mother's Day) and December (Christmas)
- **Channel analysis:** Instagram, WhatsApp Business, Physical Store, Marketplace

##### Dashboard Features
- 📈 Line chart — Full year 2025 + Q1 2026 revenue trend
- 📊 Bar chart — Top products across 6 categories
- 🍩 Donut chart — Revenue by category
- 📋 Table — Stock control for 30 products
- 🎛️ Interactive slicers — Date range + Category filter

##### Results
- ✅ Baby clothing (0-12m) = 32% of total revenue — top category identified
- ✅ May and December peak months clearly visible in trend
- ✅ Instagram = strongest sales channel in fashion periods
- ✅ 350 transactions analyzed across 15 months

##### Real Market Prices (Colombia 2025-2026)
| Category | Price Range (COP) |
|----------|------------------|
| Baby 0-12m | $52,000 – $125,000 |
| Kids 1-4 years | $68,000 – $115,000 |
| Kids 5-12 years | $72,000 – $125,000 |
| Women | $55,000 – $162,000 |
| Men | $62,000 – $172,000 |
| Accessories | $22,000 – $38,000 |

---

## 🌐 Additional Project — Parce AU

Web application built to help Colombian immigrants navigate life in Australia.

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

**Technical highlights:**
- Monolithic Flask app — no login or external database required
- User data stored locally in browser (localStorage)
- Bootstrap 5 included locally — works fully offline
- Deployed on Render — production ready

---

## 📬 Contact

**Email:** oscarpalacios08821@gmail.com
**GitHub:** [github.com/DavidsOP19](https://github.com/DavidsOP19)

---

*All freelance projects include client certification letters available upon request.*
*Portfolio built as part of IT Master's degree application — Torrens University Australia.*
