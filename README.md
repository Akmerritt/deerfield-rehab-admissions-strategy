# Project Admissions: Scaling Volume for the Deerfield Portfolio
> **A strategic product concept to reverse a 24-month admissions decline across 11 national centers.**

## 🎯 Executive Summary
Admissions volume across our 11-center portfolio has declined over the last 24 months. To hit the Board’s target of 75% BDO-led admissions, we must pivot our channel strategy toward high-intent clinical referrals (PCPs and therapists). This project introduces **CareBridge**, a digital portal designed to capture this market by eliminating administrative friction and building long-term clinical trust.

---

## 🚩 Problem Statement
Admissions volume is low primarily due to a decline in patient calls, in a climate of increased competition and growing demand for homecare services. This is an **upper-funnel channel problem**: the portfolio is over-reliant on stagnant ER leads and lacks a frictionless digital pathway to capture the growing referral demand from PCPs and therapists.

## 🔍 Research & Discovery
To understand the challenges, I conducted a deep dive into company operations:
*   **Strategic Overview:** [Interview with Sarah Chen (Chief of Staff)](./research/sarah_chen_interview.md) – Focused on the 75% BDO-led admission goal.
*   **Frontline Research:** [Staff Insights (Call Center & BDOs)](./research/staff_insights.md) – Identified 24-hour insurance latency and manual data entry as primary drivers of lead drop-off.
*   **Analysis:** [Ranked Pain Points](./research/pain_points.md) – Prioritization of P0 (Channel Diversification) and P1 (Staffing Stability).

---

## 🚩 Primary Pain Points

| Priority | Category | Pain Point | Strategic Impact |
| :--- | :--- | :--- | :--- |
| **P0** | Demand Gen | **Inadequate Channel Diversification** | Over-reliance on ER referrals; failure to capture high-intent PCP demand. |
| **P1** | Personnel | **Staffing Instability** | High turnover and 3-month onboarding times disrupt provider relationships. |
| **P2** | Operations | **Insurance (VOB) Latency** | 24–48 hour wait times cause high-intent clinical leads to call competitors. |

---

## 💡 Solution: CareBridge
**The Solution:** A HIPAA-compliant interface that bridges the referring physician, the Business Development Officer (BDO), and the Mission Center. [Read full strategy here](./strategy/solutions.md).

### 🚀 [Interactive Prototype: View Live Demo](https://your-live-demo-link.vercel.app)
*   **Access Code:** `Deerfield2025`
*   **Design Principle:** "Zero-Friction" clinical intake (Doximity SSO, Magic Links, No-Password access).

### Key Features:
*   **Continuum Capacity Pulse:** Live vacancy status for Detox, Residential, PHP, IOP, and Sober Living.
*   **Fast-Track Intake:** 60-second referral form with integrated **Insurance OCR** for instant VOB initiation.
*   **Real-Time Tracker:** Real-time transparency into the 7-stage clinical funnel (VOB → Clearance → Bed Reserved).
*   **Coordination Chat:** Patient-tethered secure messaging between PCPs and Mission Center specialists.
*   **Discharge Loop:** Automated Medication Reconciliation and follow-up scheduling pushed back to the PCP.

---

## 🛠️ Technical Logic & Assumptions
*   **Infrastructure:** **"Thin Client" Architecture**. CareBridge acts as the "Face" while Salesforce/Five9 remains the "Brain" (System of Record). No duplicative database is required.
*   **Integrations:** Bi-directional Salesforce Health Cloud API; AWS Textract for AI-powered insurance parsing; Fivetran for clinical outcome analytics.
*   **Assumptions:** We assume clinical referrals have a higher Lifetime Value (LTV) and longer Length of Stay (LOS) than digital leads. [View all assumptions](./concept/carebridge_concept.md).

---

## 📈 Measuring Success: 30-Day Pilot KPIs
To validate the ROI of the CareBridge pilot, we will track four critical performance indicators:
1.  **Referral Velocity:** % increase in net-new clinical referrals.
2.  **Conversion Rate:** Lift in lead-to-admission conversion vs. manual channels.
3.  **VOB Latency:** Reduction in average hours to verify insurance benefits.
4.  **BDO Productivity:** Reduction in administrative hours per lead.

---

## 🗓️ 90-Day Roadmap
*   **Phase 1 (Days 1-30):** Pilot CareBridge with Top 5 PCPs at 2 high-potential centers; launch scenario-based staff training.
*   **Phase 2 (Days 30-60):** Integrate Salesforce Webhooks for automated status updates; reduce VOB latency via AI-OCR.
*   **Phase 3 (Days 60-90):** Scale portal to all 11 centers; launch the Knowledge Hub to deepen clinical partnerships.

---
**Contact:** Anne Merritt | [anne.merritt@yale.edu](mailto:anne.merritt@yale.edu)
