[mgt_628_dcf_sandbox_readme.md](https://github.com/user-attachments/files/33908443/mgt_628_dcf_sandbox_readme.md)
# MGT 628 — Sustainability DCF & Sensitivity Analysis Lab
**Global Sustainability Strategy | Professor Ru-Shiun Liou**  
*Interactive 5-Year Capital Budgeting & Adverse Scenario Sandbox*

---

## 📌 Overview
The **Sustainability DCF & Sensitivity Sandbox** is a single-file, interactive web application designed for graduate students in **MGT 628 (Global Sustainability Strategy)**. It translates qualitative sustainability strategies (Milestone 2 & 3 student projects) into rigorous quantitative capital budgeting decisions. 

Grounded in corporate finance and strategic sustainability literature, the lab empowers users to evaluate capital allocation trade-offs, model the impact of unhedged transition risks on the cost of capital, and stress-test pivotal assumptions under severe market or regulatory downturns.

---

## 🧮 Core Financial Methodology (DCF & NPV)

The sandbox evaluates strategic options over a 5-year planning horizon using a standard **Discounted Cash Flow (DCF)** model and the **Present Value Interest Factor of an Annuity (PVIFA)**:

$$\text{PVIFA} = \frac{1 - (1 + r)^{-n}}{r}$$

$$\text{NPV} = -\text{CapEx}_0 + \left( \text{FCF} \times \text{PVIFA} \right)$$

Where:
* $\text{CapEx}_0$ = Initial Capital Expenditure in Year 0
* $\text{FCF}$ = Annual Free Cash Flow (Years $1$ to $5$)
* $r$ = Project Cost of Capital ($\text{WACC}$)
* $n = 5$ years

---

## 🚀 Key Features

* **Student Project Presets:** Instant configuration across 6 distinct student case studies, plus a fully customizable project entry.
* **3-Step Valuation Framework:**
  1. **Numerator (Cash Flows & CapEx):** Quantifies operational cost savings, avoided EPR/regulatory penalties, and commercial/loyalty drivers (Whelan & Douglas, 2021; Koller et al., 2019).
  2. **Denominator (Cost of Capital / WACC):** Models how proactive sustainability hedging reduces systematic transition risk premiums (Bolton et al., 2022; Cornell & Damodaran, 2020).
  3. **Pivotal Assumption Stress Test:** Isolates critical variables and simulates downside cash-flow shocks and WACC stress (Schramade, 2016).
* **Dynamic Visualization:** Built-in interactive **Chart.js** bar chart tracking initial CapEx, Present Value of 5-year cash flows, and Net Present Value (NPV).
* **Journal-Ready Export:** One-click feature to copy formatted Markdown tables and summaries directly for inclusion in academic lab journals and executive memos.
* **Print / PDF Support:** Clean print stylesheets for exporting reports as PDFs.

---

## 📊 Included Project Presets

| # | Project / Company | Focus Area | Unit |
|---|---|---|---|---|
| **1** | **Target Packaging** | Owned-brand circular packaging & EPR fee avoidance | `$\text{M}$` |
| **2** | **Delta Air Lines SAF** | Multi-year sustainable aviation fuel offtake & Scope 3 co-funding | `$\text{M}$` |
| **3** | **Ford Battery Recycling** | Closed-loop EV battery recycling & EU compliance | `$\text{M}$` |
| **4** | **Tampa Bay Markets** | Staged multi-market reusable packaging pilot | `$\text{K}$` |
| **5** | **TPA Airport / HCAA** | Proactive Airside D SAF hydrant & infrastructure readiness | `$\text{M}$` |
| **6** | **Morgan Stanley** | Audited impact-outcome & financed-emissions analytics | `$\text{M}$` |
| **7** | **Custom Project** | User-specified CapEx, cash-flow drivers, and WACC | `$\text{M}$` / `$\text{K}$` |

---

## 🛠️ Technical Architecture & Stack

* **Front-End:** Pure HTML5 / Vanilla JavaScript (Single-File Architecture).
* **Styling:** [Tailwind CSS](https://tailwindcss.com/) (loaded via CDN).
* **Data Visualization:** [Chart.js v4](https://www.chart.js/) (loaded via CDN).
* **Dependencies:** None. Completely client-side and runs entirely within any modern web browser.

---

## ⚙️ How to Use

1. **Open the Application:** Save the HTML code as `index.html` and double-click to open it in any web browser (Chrome, Safari, Edge, Firefox), or host it via GitHub Pages.
2. **Select a Preset:** Click any of the numbered buttons at the top to load baseline parameters for a specific student project.
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
