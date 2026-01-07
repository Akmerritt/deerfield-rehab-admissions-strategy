# Product Concept: CareBridge
**The "Zero-Friction" Digital Front Door for Clinical Referrals.**

## Vision
CareBridge is a clinician referral portal that bridges the gap between referring clinicians and our Mission Center. It is architected to sit on top of our existing Salesforce/Five9 stack.

## Overview
**CareBridge** is a high-trust, HIPAA-compliant digital platform designed to provide PCPs and therapists with a transparent, efficient referral path for patients seeking treatment for substance use disorders. 

This product directly addresses **Pain Point P0: Inadequate Referral Diversification**. By providing a frictionless "zero-login" referral path, we aim to scale our clinical referral pipeline and grow admissions volume. We will pilot this product at 1-2 high-potential centers before a broader rollout.

### Primary Objectives
*   **Efficient Handoffs:** Streamline the transition from primary care to specialized addiction treatment.
*   **Real-Time Bed Visibility:** Provide live information about bed availability to prevent referral drop-off.
*   **Enhanced Care Coordination:** Ensure high-touch discharge planning through close collaboration with referring providers.

## Design Principles
*   **Clean & Clinical:** Professional Medical UI with vast white space to reduce cognitive load.
*   **High Trust:** Slate Gray accents and Medical Blue (#0056b3) primary branding.
*   **Zero-Friction:** Minimal clicks, Doximity SSO, and "Magic-Link" authenticated access.

## Key Components
*   **Secure Referral Form:** HIPAA/42-CFR compliant intake with insurance card photo upload.
*   **Real-Time Patient Tracker:** Lifecycle management showing patient progress from VOB to Discharge.
*   **Bed Availability Dashboard:** Live capacity indicators for Detox, Residential, and Dual-Diagnosis.
*   **Quality Metrics:** Transparency into completion rates and readmission data.
*   **Doximity SSO:** Verified physician interface for rapid authentication.

## Full-Continuum Lifecycle Management
CareBridge is designed to manage the patient across the entire 12-month recovery journey, moving beyond the "Initial Admission" model to a "Longitudinal Care" model.

*   **ASAM-Aligned Intake:** Standardized referral levels (4.0 through 1.0) to ensure patients are placed in the clinically appropriate level of care from day one.
*   **Continuum Pulse Header:** Real-time capacity tracking across all service lines, including Detox, Residential, PHP, IOP, and Sober Living.
*   **Visual Step-Down Roadmap:** A "Subway Map" visualization within each patient profile that tracks the projected transition dates between clinical intensities, providing PCPs with a 90-day view of the recovery plan.
*   **Gapless Transitions:** Integrated Sober Living and Aftercare tracking to ensure that the handoff from clinical treatment to community reintegration is managed without a "Black Hole" period of non-communication.

## Interactive Prototype
A live, functional preview of the CareBridge interface is available for review.

*   **URL:** https://v0.app/chat/care-bridge-ui-shZ16yHAVKM?ref=L36LBK
*   **Access code:** Deerfield2025
*   **Note:** This is a sandboxed environment using synthetic data.

## Technical Components
*   **Frontend:** Next.js / Tailwind CSS (Optimized for Mobile/Tablet "point-and-shoot" insurance uploads).
*   **Backend:** Node.js (TypeScript) on AWS; leveraging **AWS Textract (OCR)** for instant insurance card parsing.
*   **Integrations:** Bi-directional **Salesforce Health Cloud** API for real-time status syncing; **Fivetran/Snowflake** for outcome analytics.
*   **Compliance and security:** HIPAA/42-CFR compliant with end-to-end encryption for all PHI (Protected Health Information) and automated consent-to-release management for sensitive SUD records. 

## Key Features
1.  **Continuum Capacity Pulse:** Live availability for Detox, Residential, PHP, IOP, and Sober Living.
2.  **Fast-Track Intake:** Capture Patient Name, DOB, and Insurance Photo in under 60 seconds.
3.  **Referral Status Tracker:** A 7-stage funnel (Contacting patient → VOB → Clinical Assessment → Medically Cleared → Bed Reserved → Admitted → Discharged).
4.  **Integrated Care Coordination:** Contextual, patient-tethered chat between PCPs and our Mission Center specialists.
5.  **Discharge Loop:** Automated Medication Reconciliation and scheduled follow-up appointments pushed back to the PCP.

## 30-Day Pilot KPIs (Success Metrics)

| KPI | Metric | Strategic Purpose |
| :--- | :--- | :--- |
| **1. Referral Velocity** | % Increase in net-new clinical referrals. | **Solves P0:** Proves we are successfully diversifying channels and capturing PCP/Therapist demand. |
| **2. Admission Conversion** | Lift in lead-to-admission rate vs. traditional channels. | **Proves Quality:** Validates the assumption that clinical leads have higher "intent to admit" than digital leads. |
| **3. VOB Latency** | Reduction in avg. hours to verify insurance benefits. | **Solves P2:** Targets a reduction from **24–48 hours down to <2 hours** via AI-OCR automation. |
| **4. BDO Productivity** | Reduction in administrative hours per lead. | **Solves P1/P4:** Measures how much time BDOs save on paperwork, allowing them more "boots-on-the-ground" time. |
| **5. Platform Adoption** | Repeat usage rate of participating PCPs. | **Proves Trust:** Measures "stickiness"—if a doctor uses it twice in 30 days, the Knowledge Hub and Discharge Loop are working. |

---

## Key Assumptions
*   **Data Interoperability:** We assume CareBridge functions as a front-end for Salesforce; all records of truth reside in the existing CRM.
*   **Clinical Readiness:** We assume PCPs will adopt the tool if administrative friction (passwords/data entry) is minimized via Doximity SSO and Magic Links.
*   **Lead Intent:** We assume clinical referrals have a higher Lifetime Value (LTV) and longer Length of Stay (LOS) than digital leads.

