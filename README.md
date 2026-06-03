# glad-mhg-onboarding
Tier system for Glad-MHG
# GLAD MHG Clinical Site Onboarding Portal

Welcome to the official repository for the **GLAD MHG Site Onboarding Framework**. This interactive portal is an operational tool designed for clinical collection sites and lab coordinators to identify their processing infrastructure capabilities, evaluate their study Tier, and access standardized logistics protocols destined for King's College London (KCL).

## 📊 Framework Overview

The study operates on a progressive, 3-tier sample collection system modeled directly from the structured laboratory matrix outlined in **image_dabb77.png**. Each successive tier reflects an escalation in required laboratory equipment, sample processing complexity, and technical staff oversight.

### 📋 Tier Classifications

* **Tier 1 (Basic Collection):** Sites are limited strictly to phlebotomy. No local centrifugation, processing, or long-term storage is performed.
* **Tier 2 (Intermediate Processing):** Sites execute standard phlebotomy, sample centrifugation, aliquoting (e.g., plasma/serum separation), and local cold-chain preservation.
* **Tier 3 (Advanced Processing):** Sites execute all standard processing alongside specialized Peripheral Blood Mononuclear Cell (PBMC) isolation protocols prior to sample dispatch.

---

## 📦 Logistical Pipelines & Shipping Workflows

To optimize sample integrity and budget cost-efficiencies, logistics pathways are strictly defined by a site's operational tier:

1. **The Postal Pathway (Tier 1 Only):** Because Tier 1 sites do not centrifuge or freeze samples locally, specimens must remain ambient. Ambient collections must be securely packed into pre-paid, clinical-grade **Royal Mail SafeBox** containers and dispatched directly to KCL on the same day as venipuncture.
2. **The Cold-Chain Pathway (Tiers 2 & 3):** Tier 2 and Tier 3 sites process and freeze derivatives locally. Rather than ad-hoc shipping, samples accumulate in site freezers. Once a designated batch threshold is reached (minimum 10 samples accumulated), a specialized medical courier is scheduled to transport the batch over to KCL on **dry ice**.

---

## 🛠️ Repository & Web Architecture

This onboarding app is designed as a **completely self-contained, single-file static application (`index.html`)** styled dynamically using Tailwind CSS. 

* **No Server Dependencies:** The application runs completely client-side in the user's browser.
* **Data Privacy Compliance:** Because the application does not utilize a backend database or external tracking APIs, **no sensitive patient or institutional site metadata is stored, transmitted, or logged** anywhere across the web. It functions purely as an educational routing tool.

---

## 🚀 Deployment Instructions (GitHub Pages)

To serve this website externally to clinical networks using GitHub Pages, follow these configurations:

1. In this repository, click on the **Settings** tab located on the top navigation bar.
2. From the left sidebar, navigate down to the **Code and automation** header and select **Pages**.
3. Under the **Build and deployment** section, verify **Source** is toggled to *Deploy from a branch*.
4. Change the deployment branch from *None* to **`main`** (or `master`), keeping the root directory path as `/ (root)`.
5. Click **Save**. 

Within 1–2 minutes, GitHub will compile your environment and host your tool live at: 
`https://<your-github-username>.github.io/glad-mhg-onboarding/`
