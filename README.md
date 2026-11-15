# ⚡ VoltRelay Energy: Growth vs. Quality Analysis

**An End-to-End Data Analytics Project for the Gradient Learnings Hackathon
for detail pls open .ipynb file we give our best **

## 📌 Project Overview
VoltRelay Energy is a simulated battery-swapping network for electric 2W and 3W vehicles. While the network experienced rapid revenue growth (+83.7%) over 18 months, service failures spiked, margins eroded, and rider retention plummeted. 

**The Core Objective:** Analyze 3.8 million swap events to uncover the root causes of service failures and churn, and provide a data-driven operating budget strategy.

## 🎯 Key Findings (Executive Summary)
1. **The 3W Bottleneck:** 3W vehicles fail at **10.34%** (2x the 2W rate) due to stockouts.
2. **The Kyron Disaster:** Kyron batteries degrade **35.46%** (2x faster than competitors), destroying range and profitability.
3. **The Margin Paradox:** PEAK pricing yields a massive **₹32.98/swap**, while Fleet Partners are a volume trap yielding only **₹6.15/swap** (with the largest partner operating at a loss).
4. **The Churn Cliff:** If a rider experiences >10% cumulative failures, their lifetime value drops by 50%. The 3W segment is sitting right on this cliff.

---

## 📂 Project Structure & Methodology
**The Jupyter Notebook (`.ipynb`) is the foundational source of truth for this entire project.** All other deliverables (PPT, Report, Dashboard) were derived directly from the code and insights generated in the notebook.

### 1. The Core: Jupyter Notebook (`VoltRelay_Analysis.ipynb`)
The notebook follows a strict, judge-defensible flow:
*   **Data Loading & Cleaning:** Handled the firmware timestamp bug (+5.5 hrs), excluded test stations, removed offline duplicates, and validated a 100% successful merge across 5 tables.
*   **Unit Economics Model:** Built a custom Contribution Margin model (Revenue - Energy Cost - Battery Wear - Station Rent).
*   **Core Analysis (Q1-Q6):** Addressed all 6 organizer questions using Pandas, Matplotlib, and Seaborn.
*   **Deep Dives:** Added 4 bonus analyses (Expansion Waves, Support Ticket NLP, Anomaly Detection, Fleet Partner Value).
*   **Output:** Generated 6 high-resolution charts (`chart_q1.png` to `chart_q6.png`) which are reused in all other deliverables.

### 2. Power BI Dashboard (`VoltRelay_Dashboard.pbix`)
An interactive 1-page executive dashboard built using pre-aggregated data (exported via the Notebook) to ensure fast loading and interactive slicing (e.g., filter by city or vehicle type).

### 3. Presentation (`VoltRelay_Hackathon_PPT_Final.pptx`)
A 9-slide premium deck designed for a 3-minute pitch to leadership. Focuses on the "So What?" and the Budget Decision.

### 4. Analysis Report (`VoltRelay_Analysis_Report_Final.docx`)
A comprehensive 12+ page consulting-style report detailing the methodology, code logic, deep-dives, and priority-ordered recommendations (P1 to P5).

---

## 🛠 Tech Stack
*   **Core Analysis:** Python 3 (Pandas, NumPy, Matplotlib, Seaborn)
*   **Environment:** Google Colab
*   **Business Intelligence:** Power BI Desktop
*   **Documentation:** `python-pptx` & `python-docx` (for programmatic formatting)

---

## 🚀 How to Run the Notebook
1. Open `VoltRelay_Analysis.ipynb` in Google Colab.
2. Mount your Google Drive (the dataset `swap_events.csv` and other CSVs must be in `/content/drive/MyDrive/`).
3. Click **"Runtime -> Restart and Run All"**. 
4. The notebook will clean the data, generate KPIs, and output 6 charts locally.

---

## 🏆 Final Recommendations (The Budget Decision)
Based on the evidence, VoltRelay should:
*   ✅ **APPROVE:** 3W Battery Inventory (Phase out Kyron), Gen1 to Gen3 Charger Retrofits, Network-wide PEAK Pricing.
*   ❌ **REJECT:** Building new stations (Wave3) and Exclusive Fleet Partner contracts.

---

## 📝 AI Disclosure
AI tools were used for brainstorming analytical questions, debugging Pandas code, and refining business insights. All data processing, merging, statistical logic, and narrative construction are original. No pre-built analysis or external datasets were used — all insights are derived solely from the organizers' provided data.

**Team:** deep_insights | **Analyst:** Rishabh Shukla
**Event:** Gradient Learnings Data Analytics Hackathon (Nov 2026)
