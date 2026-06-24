# Microgrid Feasibility & Optimization Study for a Desert Community

## 1. Introduction & Project Background
This repository contains a comprehensive technical and economic feasibility study dedicated to finding a reliable electrification solution for an isolated desert location. The target site is **Sidi-Abdelkader**, a remote village situated in the **Timoudi commune (Wilaya of Bechar, Algeria)**. 

Following an on-site field visit to understand local challenges, this study utilizes **HOMER Pro** (Microgrid Analysis Tool) to model, simulate, and determine the absolute optimal hybrid power system architecture.

---

## 2. Mathematical & Geographic Setup
* **Location Coordinates:** 29°24′32.41" N, 01°03′20.31" W
* **Project Lifetime:** 25 Years
* **Economic Parameters:** Modeled with an 8.00% discount rate and a 2.00% inflation rate.

---

## 3. Load Profile Modeling
To ensure realistic operations, the system load was configured with accurate fluctuations rather than a flat consumption curve:
* **Peak Electrical Demand:** 100 kW
* **Average Daily Consumption:** 11.26 kWh/day
* **Realism Adjustments:** A **15% random white noise variability** (daily and hourly) was introduced into HOMER Pro to simulate authentic human activity and unexpected variations.

---

## 4. Meteorological Resource Assessment (NASA Data)
Using multi-decade historical satellite data downloaded from the **NASA Prediction of Worldwide Energy Resource (POWER)** database, the local renewable potentials were analyzed:

### A. Solar Resource (GHI)
* **Annual Average:** Peak horizontal solar resources occur in **June**, yielding an average of **7.75 kWh/m²/day** with a clearness index of **0.680**.
* **Temperature Constraint:** The study highlights that June/July are not the months with the highest solar efficiency. This is due to extreme peak ambient temperatures reaching a monthly average of **35.78°C in July**, which naturally penalizes photovoltaic cell efficiency.

### B. Wind Resource
* **Annual Average Wind Speed:** Measured at **6.05 m/s** at an anemometer height of 50 meters.
* **Seasonal Consistency:** Wind speeds peak during Spring (**6.70 m/s in May**), providing excellent complementary generation when solar panels experience thermal degradation.

---

## 5. System Architecture & Components
The multi-source microgrid was modeled using both alternating current (AC) and direct current (DC) buses:
* **Renewable Sources:** Photovoltaic Panels (PV) and Wind Turbines (G10 Model).
* **Dispatchable Backup:** A Diesel Generator (DC Gen) to safeguard grid security.
* **Energy Storage & Grid:** Lead-Acid (LA) Battery bank, a bi-directional DC/AC Converter, and a Grid connection option.

---

## 6. Simulation Results & Optimal Solution
After evaluating hundreds of search space combinations regarding Net Present Cost (NPC) and Cost of Energy (COE), HOMER Pro generated a categorized list of viable options.
**The Optimal Selected System: Tri-Source Hybrid Configuration (PV + Wind + Grid)**

