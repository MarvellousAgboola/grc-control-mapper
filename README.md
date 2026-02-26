# 🛡️ ISO 27001:2022 Multi-Framework Control Mapper

> An interactive web tool that maps all **93 ISO 27001:2022 Annex A controls** to **NIST CSF 2.0**, **SOC 2 TSC**, and **PCI-DSS v4.0** — built by Victor Agboola, for GRC analysts.

---

## 🔴 Live Demo

👉 **[Try it here →]**

---

## 📌 The Problem This Solves

GRC analysts routinely work across multiple compliance frameworks simultaneously. A single engagement might require mapping ISO 27001 controls to SOC 2 for a SaaS client, NIST CSF for a US federal contractor, and PCI-DSS for a payments company — all at the same time.

**The traditional approach:**
- Multiple browser tabs open across framework documentation
- Manual spreadsheet cross-referencing
- Hours lost per engagement to lookup work
- High risk of mapping errors and omissions

**This tool eliminates that entirely.**

---

## ✨ Features

| Feature | Description |
|---|---|
| 🔍 **Real-Time Search** | Search by control ID (e.g. `A.8.5`), keyword (e.g. `encryption`), domain, or framework reference (e.g. `CC6.1`) |
| 📂 **Domain Filter** | Narrow to Organizational, People, Physical, or Technological controls instantly |
| 🏷️ **Framework Filter** | One-click filter to show only controls mapped to NIST CSF, SOC 2, or PCI-DSS |
| 🔽 **Expand for Detail** | Click any control row to reveal the full mapping rationale and implementation guidance per framework |
| 📊 **Full Annex A Coverage** | All 93 ISO 27001:2022 controls including all new 2022 additions |
| 🌐 **Zero Dependencies** | Single HTML file — no server, no login, no data sent anywhere. Runs entirely in the browser |
| 🎨 **Professional UI** | Dark-themed, responsive design built for professional portfolio presentation |

---

## 🗺️ Frameworks Covered

### 🟢 ISO 27001:2022 (Source Framework)
All 93 Annex A controls across 4 domains:
- **A.5** — Organizational Controls (37 controls)
- **A.6** — People Controls (8 controls)
- **A.7** — Physical Controls (7 controls)
- **A.8** — Technological Controls (34 controls + supporting)

New 2022 controls included: Threat Intelligence (A.5.7), Cloud Services Security (A.5.23), Data Masking (A.8.11), Data Leakage Prevention (A.8.12), Web Filtering (A.8.23), and more.

### 🔵 NIST CSF 2.0 (Target Framework)
Mapped to the 6 NIST CSF 2.0 Functions:
- **GV** — Govern
- **ID** — Identify
- **PR** — Protect
- **DE** — Detect
- **RS** — Respond
- **RC** — Recover

### 🟣 SOC 2 TSC (Target Framework)
Mapped to Trust Services Criteria:
- **CC1–CC9** — Common Criteria (Security)
- **A1** — Availability
- **P1–P4** — Privacy (where applicable)

### 🟡 PCI-DSS v4.0 (Target Framework)
Mapped to all 12 PCI-DSS requirements where applicable, with specific sub-requirement references.

---

## 🚀 How to Use

### Option 1 — Use the Live Tool
Click the live demo link above. No installation needed.

### Option 2 — Run Locally
```bash
# Clone the repository
git clone https://github.com/your-username/grc-control-mapper.git

# Navigate to the folder
cd grc-control-mapper

# Open in your browser
open control-mapper.html
# or just double-click the file
```

### Option 3 — Deploy Your Own Copy (GitHub Pages)
```bash
# Fork this repo, then:
# 1. Go to your repo → Settings → Pages
# 2. Set Source to: Deploy from a branch
# 3. Select: main branch / root folder
# 4. Click Save — your live URL will appear in ~60 seconds
```

---

## 💼 Real-World Use Cases

### Use Case 1 — SOC 2 Audit Preparation
**Scenario:** Your organization is ISO 27001 certified and undergoing a SOC 2 Type II audit. You need to map existing controls to SOC 2 criteria.

**How to use:** Search `CC6.1` in the tool → instantly see every ISO 27001 control that satisfies that criterion, with rationale. Present this mapping to auditors as evidence of control equivalence.

---

### Use Case 2 — PCI-DSS Gap Analysis
**Scenario:** A client processes card payments and needs to understand what PCI-DSS coverage their ISO 27001 certification already provides.

**How to use:** Click the **PCI-DSS** filter button → review all 70+ controls with PCI mappings → identify controls with `—` (not mapped) as gap areas requiring dedicated PCI controls.

---

### Use Case 3 — Multi-Framework Executive Reporting
**Scenario:** The board wants a single view of the organization's compliance posture across all active frameworks.

**How to use:** Expand any high-priority control (e.g. `A.8.5 Secure Authentication`) → screenshot the expanded view showing NIST, SOC 2, and PCI coverage in one panel → include in board report.

---

### Use Case 4 — Vendor / Third-Party Assessment
**Scenario:** A prospect asks whether you're compliant with NIST CSF before signing a contract. You're ISO certified but not formally NIST assessed.

**How to use:** Filter by **NIST CSF** → export or screenshot the full mapping → show the prospect the direct equivalence between your ISO controls and their NIST requirements.

---

### Use Case 5 — Zero Trust Architecture Review
**Scenario:** You're advising on a Zero Trust implementation and need to identify which ISO controls apply.

**How to use:** Search `access` or `authentication` → controls A.5.15, A.5.16, A.5.17, A.8.2, A.8.3, A.8.5 appear immediately with their NIST identity-related mappings (PR.AA series).

---

## 📁 Repository Structure

```
grc-control-mapper/
│
├── control-mapper.html        # The complete application (single file)
├── README.md                  # This file
└── portfolio-one-pager.pdf    # Portfolio summary for job applications
```

---

## 🧠 How It Was Built

This tool was developed using **AI-assisted GRC analysis** — a modern workflow where domain expertise drives the output and AI accelerates the execution.

**The process:**
1. Framework research — ISO 27001:2022, NIST CSF 2.0, SOC 2 TSC, and PCI-DSS v4.0 official documentation
2. Control mapping logic — each ISO control was analyzed against the other three frameworks based on intent, scope, and implementation requirements
3. AI-assisted development — Claude (Anthropic) was used to accelerate the coding of the interactive interface
4. GRC review — all mappings were validated against official guidance and cross-referenced for accuracy

> This project demonstrates how GRC professionals can use AI as a force multiplier — not to replace expertise, but to deliver more value, faster.

---

## 📋 Mapping Methodology

Each ISO 27001:2022 control is mapped based on:

- **Control intent alignment** — does the ISO control address the same security objective as the target framework requirement?
- **Implementation overlap** — would implementing the ISO control satisfy or partially satisfy the target requirement?
- **Official guidance cross-reference** — mappings are anchored to published guidance from NIST, AICPA, and PCI SSC where available

Controls marked `—` in a framework column indicate no direct mapping exists and dedicated controls should be considered for that framework.

---

## ⚠️ Disclaimer

This tool is intended as a **reference aid** to support GRC professionals. Framework mappings are based on professional judgment and publicly available guidance. They should not be used as a substitute for formal compliance assessment, qualified auditor review, or official certification programs.

Always validate mappings against the latest published versions of each framework standard.

---

## 🤝 Contributing

Spotted an incorrect mapping? Want to add a new framework? Contributions are welcome.

1. Fork the repository
2. Create a feature branch: `git checkout -b fix/control-A.8.5-mapping`
3. Make your changes in `control-mapper.html`
4. Submit a pull request with a description of the change and your source reference

---

## 📜 License

MIT License — free to use, modify, and distribute with attribution.

---

## 👤 Author

Built by **Victor Agboola** specializing in multi-framework compliance, risk management, and AI-augmented security operations.

Connect on LinkedIn: https://www.linkedin.com/in/agboolavictor/

---

If this tool saved you time, drop a ⭐ on the repo it helps others find it.
