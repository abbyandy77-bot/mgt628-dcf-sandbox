# MGT 628 — Sustainability DCF & Sensitivity Analysis Lab
**Global Sustainability Strategy | Professor Ru-Shiun Liou**  
*Interactive 5-Year Capital Budgeting & Adverse Scenario Sandbox*

---

## 📌 Overview
The **Sustainability DCF & Sensitivity Sandbox** is a single-file, interactive web application designed for graduate students in **MGT 628 (Global Sustainability Strategy)**. It translates qualitative sustainability strategies into rigorous quantitative capital budgeting decisions. 

Grounded in corporate finance and strategic sustainability literature, the lab empowers users to evaluate capital allocation trade-offs, model the impact of unhedged transition risks on the cost of capital, and stress-test pivotal assumptions under severe market or regulatory downturns.

---

## 🚀 Key Features

* **Case Study Presets:** Instant configuration across 6 distinct corporate sustainability case studies, plus a fully customizable project entry.
* **3-Step Valuation Framework:**
  1. **Numerator (Cash Flows & CapEx):** Quantifies operational cost savings, avoided EPR/regulatory penalties, and commercial/loyalty drivers (Whelan & Douglas, 2021; Koller et al., 2019).
  2. **Denominator (Cost of Capital / WACC):** Models how proactive sustainability hedging reduces systematic transition risk premiums (Bolton et al., 2022; Cornell & Damodaran, 2020).
  3. **Pivotal Assumption Stress Test:** Isolates critical variables and simulates downside cash-flow shocks and WACC stress (Schramade, 2016).
* **Dynamic Visualization:** Built-in interactive **Chart.js** bar chart tracking initial CapEx, Present Value of 5-year cash flows, and Net Present Value (NPV).
* **Journal-Ready Export:** One-click feature to copy formatted Markdown tables and summaries directly for inclusion in academic lab journals and executive memos.
* **Print / PDF Support:** Clean print layout for exporting reports as PDFs.

---

## 📊 Included Project Presets

| # | Project / Company | Strategic Focus Area | Unit |
|---|---|---|---|
| **1** | **Target Packaging** | Owned-brand circular packaging redesign & state EPR fee avoidance | `$M` |
| **2** | **Delta Air Lines SAF** | Multi-year sustainable aviation fuel (SAF) offtake & Scope 3 co-funding | `$M` |
| **3** | **Ford Battery Recycling** | Closed-loop EV battery recycling & EU regulatory compliance | `$M` |
| **4** | **Tampa Bay Markets** | Staged multi-market reusable packaging & waste-prevention pilot | `$K` |
| **5** | **TPA Airport / HCAA** | Proactive Airside D SAF hydrant & blending infrastructure readiness | `$M` |
| **6** | **Morgan Stanley** | Audited impact-outcome & financed-emissions analytics platform | `$M` |
| **7** | **Custom Project** | User-specified CapEx, ROSI cash-flow drivers, and WACC | `$M` / `$K` |

---

## 🧮 Core Financial Formulas

The sandbox calculates the **5-Year Present Value Interest Factor of Annuity (PVIFA)** and **Net Present Value (NPV)** using:

$$\text{PVIFA} = \frac{1 - (1 + r)^{-n}}{r}$$

$$\text{NPV} = -\text{CapEx}_0 + \left(\text{Annual FCF} \times \text{PVIFA}\right)$$

$$\text{Break-Even Annual FCF} = \frac{\text{CapEx}_0}{\text{PVIFA}_{\text{stressed}}}$$

*(Where $r$ is the project WACC and $n = 5$ years).*

---

## 🛠️ Technical Architecture & Stack

* **Front-End:** Pure HTML5 / Vanilla JavaScript (Single-File Architecture).
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (via CDN).
* **Data Visualization:** [Chart.js v4](https://www.chart.js/) (via CDN).
* **Dependencies:** None. Runs entirely client-side in any modern web browser.

---

## ⚙️ How to Use

1. **Open the Application:** Save the HTML file as `index.html` and open it in any web browser (or deploy via GitHub Pages).
2. **Select a Preset:** Click any of the numbered preset buttons at the top to load baseline parameters for a specific case study.
3. **Adjust Parameters (Steps 1 & 2):** Modify CapEx, cash flow drivers, or WACC values to observe real-time changes in NPV and PVIFA.
4. **Stress Test (Step 3):** Use the cash flow shock slider and WACC stress adjustment to run adverse scenarios, or click **"Simulate Adverse Case"** for pre-configured stress levels.
5. **Export Data:** Click **"Copy Markdown Table for Journal"** to paste your findings directly into your documentation, or click **"Print / Save PDF"** to archive the report.

---

## 📚 Theoretical & Academic Foundations
* **Whelan, T., & Douglas, C. (2021):** *Return on Sustainability Investment (ROSI).* NYU Stern Center for Sustainable Business.
* **Koller, T., Goedhart, M., & Wessels, D. (2019):** *Valuation: Measuring and Managing the Value of Companies.* Wiley.
* **Bolton, P., & Kacperczyk, M. (2022):** *Global Pricing of Carbon Transition Risk.* Journal of Finance.
* **Cornell, B., & Damodaran, A. (2020):** *Valuing ESG: Doing Good or Sound Corporate Finance?* Journal of Impact and ESG Investing.
* **Schramade, W. (2016):** *Integrating Sustainability into Valuation Models.* Journal of Applied Corporate Finance.
