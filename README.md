Here is the finalized documentation in **GitHub Flavored Markdown (GFM)**. You can copy and paste this directly into your `README.md` file.

***

# CareBridge: Scaling Admissions Volume for a Deerfield Portfolio Company
> **A strategic product concept to increase admissions volume across 11 national addiction treatment centerscenters.**

## Executive Summary
A Deerfield portfolio company is looking to increase its admissions volume across their 11 treatment addiction centers. The comopany has seen a decline in patient call volume over the last 24 months, in a setting of increased competition, growing demand for homecare services, and changes in how patients are seeking treatment with a shift towards digital channels. In order to achieve their growth target, they will need to  pivot their channel strategy toward high-intent clinical referrals (PCPs and therapists). This project introduces **CareBridge**, a digital portal designed to capture this market by building communication, trust, and long-term relationships with clinical care proivders.

---

## Problem Statement
Admissions volume is low primarily due to a decline in patient calls, in a climate of increased competition and growing demand for homecare services. This is an **upper-funnel channel problem**: the portfolio is over-reliant on stagnant ER leads and lacks a frictionless digital pathway to capture the growing referral demand from PCPs and therapists.

## Research
To understand the challenges, I conducted a deep dive into company operations:
*   **Strategic Overview:** [Interview with Sarah Chen (Chief of Staff)](./research/sarah_chen_interview.md) – Focused on the 75% BDO-led admission goal.
*   **Frontline Research:** [Staff Insights (Call Center & BDOs)](./research/staff_insights.md) – Identified 24-hour insurance latency and manual data entry as primary drivers of lead drop-off.

---

## Deliverable 1: Ranked Pain Points

| Priority | Category | Pain Point | Business Impact |
| :--- | :--- | :--- | :--- |
| **P0** | Demand Gen | **Inadequate Channel Diversification** | **Critical:** Over-reliance on ER referrals; failure to capture high-intent PCP/Therapist demand. |
| **P1** | Personnel | **Staffing Instability** | **High:** High turnover and 3- to 6-month staffing onboarding times disrupt provider relationships and lead to delays and errors during the intake process. |
| **P2** | Operations | **Insurance (VOB) Latency** | **High:** 24–48 hour wait times cause high-intent patients to drop off or call competitors. |
| **P3** | Operations | **Data Fragmentation** | **Med:** Manual use of PDFs/Excel outside of Salesforce causes miscommunication and intake delays. |

---

## Deliverable 2: Solution Ideas

### 1. CareBridge Referral Portal (P0/P2)
A lightweight portal where PCPs and therapists can submit a referral in under 60 seconds.

### 2. Clinical Education & Feedback (P0)
A CME-accredited program for clinicians regarding early intervention and post-rehab management. Includes an automated feedback loop that sends recovery milestones (with consent) back to the referring physician to prove treatment efficacy and build thought leadership.

### 3. Mentorship & Scenario-Based Onboarding (P1)
A 90-day mentorship program paired with interactive, role-specific training modules. This reduces the staff "competency ramp-up" time from months to weeks, stabilizing the Mission Center infrastructure to support increased referral volume.

---

## 🚀 Deliverable 3: Product Concept — CareBridge
**The Solution:** A HIPAA-compliant interface that bridges the referring physician, the Business Development Officer (BDO), and the Mission Center.

*   **[Interactive Prototype: View Live Demo]([https://your-live-demo-link.vercel.app](https://v0.app/chat/care-bridge-ui-shZ16yHAVKM?ref=L36LBK))**
*   **Access Code:** `Deerfield2025`

### Key Features:
*   **Continuum Capacity:** Live availability status for Detox, Residential, PHP, IOP, and Sober Living.
*   **Fast-Track Intake:** 60-second referral form with integrated Insurance OCR for instant VOB initiation.
*   **Referral Status Overview:** Real-time transparency into the clinical funnel (VOB → Assessment → Cleared → Admitted).
*   **Continuity Loop:** Digital discharge summaries and scheduled follow-up appointments pushed back to the PCP to close the care cycle.

---

## 🛠️ Technical Components & Assumptions

### Technical Logic
*   **Frontend:** Next.js / Tailwind CSS; optimized for mobile "point-and-shoot" insurance uploads.
*   **Backend:** Node.js (TypeScript) on AWS; utilizing AWS Textract for Insurance OCR.
*   **Integrations:** Bi-directional **Salesforce Health Cloud** API for real-time CRM sync; **Fivetran** for clinical outcome analytics.

### Key Assumptions
1.  **Lead Intent:** Clinical referrals (PCPs/Therapists) have higher intent and longer length-of-stay (LOS) than digital leads, justifying the investment in a dedicated channel.
2.  **Thin Client:** CareBridge acts as the "Face" while Salesforce/Five9 remains the "Brain" (System of Record). No duplicative database is required.
3.  **Data Interoperability:** All 11 centers utilize EMR/CRM systems that support standard API integrations for real-time syncing.

---

## 📈 Next Steps: 90-Day Roadmap
*   **Phase 1 (Days 1-30):** Pilot CareBridge with Top 5 PCPs at 2 high-potential centers; launch scenario-based staff training to stabilize the Mission Center.
*   **Phase 2 (Days 30-60):** Integrate Salesforce Webhooks for automated status updates; reduce VOB latency via AI-OCR.
*   **Phase 3 (Days 60-90):** Scale portal to all 11 centers; launch the Knowledge Hub to deepen clinical partnerships and drive long-term referral loyalty.

---
**Contact:** [Anne Merritt]
