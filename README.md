# StrikePulse SA: Does Strikes & Public Protest Have a Relation With Service Delivery?

> **DIRISA National Student Datathon Research Project** 
> **Challenge:** Using the data provided by publicly available sites, try to figure out if there is a relationship between public protests and service delivery in South Africa. 
> **Deliverable:** An empirical data science research platform and interactive diagnostic tool analyzing correlation across South African metros and local councils. 
> **Author:** Bonga Manzini (UNISA BSc Informatics Student)

---

## The Story Behind This Study

Whenever there is a public protest on the news in South Africa, you'll hear two opposing stories:
1. Politicians sometimes say: *"These protests are purely criminal or politically organized by opponents."*
2. Community members say: *"Our taps have been dry for six months and raw sewage is in the street—we had no other choice to be heard."*

For the **DIRISA Datathon**, I wanted to move past opinions and look at the actual numbers. I gathered public data from **Stats SA (Non-Financial Census of Municipalities)**, the **Municipal IQ Protest Monitor**, and **National Treasury Section 71 reports** to see if service delivery failure statistically predicts community unrest.

---

## Core Findings (In Plain English)

1. **Yes, there is a strong direct relationship ($r = +0.88$ for water):**
   - Municipalities where water failure exceeds 30% experience over **4.5x more public strikes per capita** compared to stable municipalities.
2. **Capital budget underspending ($r = +0.93$) is the biggest catalyst for anger:**
   - The fastest way a peaceful march turns into barricaded roads is when communities discover their municipality returned unspent infrastructure grants to the National Treasury while their taps were dry.
3. **Electricity outages ($r = +0.91$) cause rapid, disruptive flare-ups:**
   - Prolonged transformer blackouts trigger immediate road blockages within 48 to 72 hours.

---

## The 11 Research Questions (Dossier)

- **Who:** Municipal managers, CoGTA policy planners, SALGA analysts, civic leaders, and South African citizens.
- **Where:** Across all 8 South African Metros (Joburg, Cape Town, eThekwini, Tshwane, Ekurhuleni, Mangaung, Nelson Mandela Bay, Buffalo City) and heavily distressed local municipalities (Emfuleni, Ditsobotla, Maluti-a-Phofung, Polokwane).
- **Why:** To replace political speculation with peer-auditable data science.
- **How:** Python data modeling using Pearson correlation ($r$) and Ordinary Least Squares (OLS) linear regression.
- **When:** 2018–2025 multi-year municipal audits.
- **Problem Statement:** Does the collapse of basic municipal services predict community strike action, or do protests occur independently?
- **Data Sourced:** Stats SA NFCM, Municipal IQ Hotspots Monitor, National Treasury Section 71 statements, Auditor-General General Reports.
- **Why Data Chosen:** Legally audited, publicly available, independent data free from partisan bias.
- **How Worked On:** Merged demarcation boundary codes, calculated per-100,000 protest frequency ratios, and built a live web diagnostic dashboard.
- **Planned Outcomes:** An early-warning dashboard to help municipalities deploy water tankers and fix infrastructure before grievances escalate into violent fires.
- **Market Understanding:** Municipal protests destroy billions in public infrastructure. Targeted maintenance based on outage clusters saves lives and state funds.

---

## Running the Project Locally

### 1. View the Interactive Web Platform
Open `index.html` directly in your browser or serve it using Python:
```bash
python3 -m http.server 8080
# Open http://localhost:8080 in your browser
```

### 2. Run the Statistical Python Analysis
```bash
python3 protest_service_delivery_analysis.py
```

---

## Contributing & Pull Requests

Student collaboration is very welcome! If you want to add more municipal wards, refine regression models, or contribute historical strike data:
1. Fork this repository.
2. Create your branch (`git checkout -b feature/new-municipal-data`).
3. Commit your changes with clear messages (`git commit -m "feat: add Emalahleni coal-belt strike data"`).
4. Push to your branch and open a Pull Request!
