# Product Concept: CareBridge
**The "Zero-Friction" Digital Front Door for Clinical Referrals.**

## Vision
CareBridge is a clinician referral portal that bridges the gap between referring clinicians and our Mission Center. It is architected to sit on top of our existing Salesforce/Five9 stack.

## Technical Components
*   **Frontend:** Next.js / Tailwind CSS (Optimized for Mobile/Tablet "point-and-shoot" insurance uploads).
*   **Backend:** Node.js (TypeScript) on AWS; leveraging **AWS Textract (OCR)** for instant insurance card parsing.
*   **Integrations:** Bi-directional **Salesforce Health Cloud** API for real-time status syncing; **Fivetran/Snowflake** for outcome analytics.

## Key Features
1.  **Continuum Capacity Pulse:** Live availability for Detox, Residential, PHP, IOP, and Sober Living.
2.  **Fast-Track Intake:** capture Name, DOB, and Insurance Photo in under 60 seconds.
3.  **Referral Status Tracker:** A 7-stage funnel (VOB → Assessment → Cleared → Bed Reserved → Admitted).
4.  **Integrated Care Coordination:** Contextual, patient-tethered chat between PCPs and our Mission Center specialists.
5.  **Discharge Loop:** Automated Medication Reconciliation and scheduled follow-up appointments pushed back to the PCP.

## 30-Day Pilot KPIs (Success Metrics)
*   **Referral Velocity:** % increase in net-new clinical referrals.
*   **Conversion Rate:** Lift in lead-to-admission conversion vs. manual channels.
*   **VOB Latency:** Reduction in average hours to verify insurance benefits.
*   **BDO Productivity:** Reduction in administrative hours per lead.

## Key Assumptions
*   **Data Interoperability:** We assume CareBridge functions as a front-end for Salesforce; all records of truth reside in the existing CRM.
*   **Clinical Readiness:** We assume PCPs will adopt the tool if administrative friction (passwords/data entry) is minimized via Doximity SSO and Magic Links.
*   **Lead Intent:** We assume clinical referrals have a higher Lifetime Value (LTV) and longer Length of Stay (LOS) than digital leads.

