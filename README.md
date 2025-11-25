# ISO 27001 Compliance Automation Engine (Python)

Automated compliance mapping engine that analyzes ISO 27001 Annex A controls, maps them to evidence, evaluates gaps, assigns risk-weighted compliance scores, and generates professional Excel + PDF reports.

This project demonstrates:
- ✔ Security Consulting mindset  
- ✔ ISO 27001 Annex A understanding  
- ✔ Python automation skills  
- ✔ NLP for policy–control matching  
- ✔ Evidence validation + compliance scoring  
- ✔ Excel dashboards + PDF reporting  
- ✔ Full CLI automation pipeline  

---

## 🚀 Features

### 🔍 1. Ingestion
Loads:
- ISO 27001 Annex A controls (JSON)
- Asset inventory (CSV)
- Policies (TXT)
- Evidence index (JSON)
- Risk register (CSV)

### 🧠 2. Automated Mapping
- Rule-based control → evidence mapping  
- NLP (difflib similarity) to match policy text to control descriptions  
- Generates `mappings.csv`

### 🛡️ 3. Evidence Checking
- Verifies policy presence  
- Verifies evidence type availability (config, asset inventory, etc.)  
- Identifies missing items  
- Generates:
  - `results.json`
  - `gaps.csv`

### 📊 4. Compliance Scoring
- Compliance state: **Compliant / Partially Compliant / Not Compliant**  
- Risk-weighted scoring based on control impact  
- Computes:
  - Compliance %
  - Weighted Compliance %

### 📈 5. Excel Dashboard
Generates `report.xlsx` with:
- Summary sheet  
- Controls sheet  
- Mappings sheet  
- Gaps sheet  
- Charts sheet:
  - Compliance bar chart  
  - Weighted compliance bar chart  

### 📝 6. PDF Report
Generates a clean 1-page `summary.pdf`:
- Summary table  
- Header, footer, timestamps  
- Perfect for screenshots / auditors  

### 🖥️ 7. CLI Tool (One command automation)
Run entire pipeline:

```bash
python src/cli.py run-all
