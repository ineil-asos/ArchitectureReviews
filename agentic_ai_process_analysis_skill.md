# Skill: Agentic AI Process Analysis & Report Generation

**Description:** This skill guides the AI to perform a deep-dive "Agentic AI process analysis" on raw corporate workflows (usually from CSV/Excel) and generate a highly polished, interactive, AI Process & Tech Consulting-style assessment report in a single-file HTML format.

## 1. Input Requirements
The user will provide raw data (e.g., a CSV or JSON file) containing a backlog of use cases, processes, or initiatives. The data should ideally contain:
- **Function/Department** (e.g., Finance, Legal)
- **Process Name**
- **Description**
- **Current Effort/Pain Points**

## 2. Analytical Directives
Before generating code, the AI must perform a critical analysis acting as a **Joint Chief AI Governance Officer & Enterprise Solution Architect**:
1. **Disposition & Categorization:** Classify every process into standard categories (e.g., Out-of-the-Box Automation vs. Custom Pro-Code Agentic AI).
2. **Business Value Assessment:** Do not just calculate FTE hours saved. Evaluate the strategic value:
   - *Efficiency:* Paradigm shifts (e.g., sample-based to 100% population testing).
   - *Error Reduction:* Impact of eliminating human bias or omission.
   - *Revenue/Risk:* Quantify the value of mitigating high-value errors or unlocking trapped revenue.
3. **AI Governance & Compliance Guardrails:** For every high-complexity use case, mandate:
   - Is there a Regulated Duty?
   - What level of human oversight is required? (HITL or 4-Eye dual sign-off).
   - Are there Third-Party Data / IPR risks? (Mandate API-only data fences).
   - Map specific Risk Questionnaire Q-IDs directly into the guardrail table (e.g., 'Regulated Duty (Q14)').
4. **Architectural Mitigation Strategy:** Design 4 specific, actionable mitigation strategies per use case (e.g., Cryptographic provenance hashing, Sandboxed execution, Deterministic policy engines).

## 3. Structural Directives (HTML)
Generate a single-file `index.html` with zero external dependencies (aside from Google Fonts and a logo image).
The structure must strictly follow:
1. **Header:** Corporate logo and subtle capability assessment title.
2. **Master Navigation:** Sticky top navigation toggling between "Executive Summary", "Detailed Analysis", and "AI Risk Questionnaire".
3. **Executive Summary View:**
   - Methodology Infographic (01 to 04 steps).
   - High-level Metrics Row.
   - Target State Grid (Clickable cards that open detailed modal deep-dives).
4. **Detailed Analysis View:**
   - Categorized tables displaying all processes, their target tech stack, and architectural rationale.
5. **AI Risk Questionnaire View:**
   - A distinct tab containing a categorized table of AI risk questions mapped to operational buckets (e.g. Data Privacy, Ethics, Autonomy).
6. **Interactive Modals (Deep Dives):**
   - Must contain the Future State Agentic Experience.
   - **Architecture Infographic:** CSS grid flow showing Inputs → Agent Engine → Outputs.
   - **Governance Bar:** Dark-themed bar under the architecture detailing specific gates (🔒 Data Fence, 📋 Audit Trail, 👤 HITL, 👥 4-Eye).
   - **Critical Business Value Grid:** 3-column editorial grid for Effort Savings, Error Reduction, and Governance Notes.
   - **Compliance Guardrails:** Monochromatic table with Red/Amber/Green verdicts. Labels must cross-reference specific Q-IDs and implement an instant, custom JS/CSS tooltip system to show the full question text on hover (bypassing native browser delays).
   - **Mitigation Strategy:** 2-column grid outlining the expert architecture recommendations.

## 4. Design Aesthetics & CSS (Premium AI Process & Tech Consulting style)
The CSS must adhere to a premium editorial design system:
- **Typography:** Google Font `Inter`. Weights restricted to 300 (light), 400 (regular), 600 (semibold). Generous line-height (`1.6` or `1.7`).
- **Whitespace:** Extremely generous padding (`padding: 56px 64px` for modals).
- **Color Palette:**
  - Background: Off-white `#FAFAFA`
  - Text: Deep Slate `#1A1A2E` and Muted `#4A5568`
  - Accents: Restrained. Use Cognizant Blue `#0033A0`, Amber `#B45309`, Green `#065F46`, Purple `#5B21B6`.
- **UI Elements:**
  - Flat borders (`1px solid #E2E8F0`) instead of heavy box-shadows.
  - Section dividers should use thin, elegant accent lines (`border-top: 2px solid`).
  - Use typographic hierarchy (uppercase tracking: `letter-spacing: .1em`) for micro-copy and labels.
- **Print Layout:** Include strict `@media print` rules.
  - Hide all navigation and body background elements.
  - Force `.modal-content` to display block, removing shadows and fixed positioning.
  - Use `page-break-inside: avoid` on grids and infographics.
  - Ensure colors print perfectly with `-webkit-print-color-adjust: exact`.

## 5. Execution Workflow
1. Parse the user's data.
2. Run the Governance & Business Value analysis in memory.
3. Output the fully formed HTML structure containing the generated analysis injected directly into the premium CSS template.
4. Provide the user with a local server command (`python3 -m http.server 8000`) to view the file without `file://` CORS issues.

## 6. Corporate AI Risk Questionnaire Baseline
Use the following 22-question framework to assess risk and generate the Q-ID tooltips:

**1. Prohibited & High-Risk Applications**
- **Q1:** Does the project involve the AI system to be used for access to, evaluating eligibility and/or enjoyment of essential private / public services and benefits?
- **Q2:** Does the project involve the AI system to be used as a safety component of a product or the AI system is itself a product regulated by safety regulations?
- **Q3:** Does the project involve the AI system to be used for critical infrastructure?
- **Q4:** Does the project involve the AI system to be used for employment, workers' management or access to self-employment?
- **Q5:** Does the project involve the AI system to be used for migration, asylum and border control management, administration of justice, democratic processes or law enforcement?
- **Q8:** Is there a risk of the project involving AI practices that have been categorized as "prohibited"?
- **Q9:** Is the proposed AI solution used in a system where human health and safety is paramount?

**2. Data Privacy & Sensitivity**
- **Q6:** Does the project involve the use of sensitive personal information (eg biometric data, health data, financial data)?
- **Q7:** Does the project involve the AI system using emotion recognition with the purpose to identify or infer emotions or intentions of natural persons?

**3. Ethics, Rights & Societal Impact**
- **Q10:** Does the proposed AI solution relate to, or could it impact environmental matters beyond the incidental impacts of operating the model itself?
- **Q11:** Could the proposed AI solution be used to create and spread information which may have a material impact on democracy?
- **Q12:** Could the proposed AI solution impact the fundamental rights of individuals?

**4. Operational Autonomy & Accountability**
- **Q13:** Does the proposed AI solution operate as part of the core systems of any business?
- **Q14:** Does the proposed AI solution fulfil any regulated duty?
- **Q15:** During deployment would the proposed AI solution make and/or implement decisions autonomously?

**5. Ecosystem & Third-Party Exposure**
- **Q16:** Is Cognizant itself providing data for use in or with the AI?
- **Q17:** Will the proposed AI solution be used by third party members of the public?
- **Q18:** Will the solution's functionality or output(s) be relied on by anyone other than the client and its group affiliates?
- **Q22:** Does the solution extract or use third party content without prior license, including data scraping from online sources?

**6. Financial & Process Risk**
- **Q19:** Does the solution determine values or prices for assets or services?
- **Q20:** Does the solution perform a high volume of tasks or transactions where an error could cause significant losses or tasks to put right?
- **Q21:** Does the solution perform a role or function that the client has identified as high sensitivity or risk?
