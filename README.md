# 🩺 AI Oncology Case-Brief Generator

An automated multi-agent workflow for **[2ndOpinion Desktop](https://2ndopin.io/desktop)** that turns a standard oncology document packet into a **consistent, sourced, decision-ready clinical case brief**.

## 📌 What It Does

The workflow processes:

* Pathology reports
* Imaging reports
* Clinical notes
* Surgery reports
* Laboratory results

Each document type is reviewed by a dedicated specialist agent. The extracted findings are then checked against the original source document before being passed to a synthesis agent.

The final output is a Markdown **Clinical Case Brief** containing:

* Current clinical status
* Diagnosis and pathology
* Biomarkers / molecular findings
* Imaging
* Treatment history
* Relevant laboratory findings
* Clinical timeline
* Missing, uncertain, or contradictory information
* Source document references

A final verification step checks the completed brief against the extracted source evidence and removes or corrects unsupported claims.

## 🚀 How to Use

1. Install **[2ndOpinion Desktop](https://2ndopin.io/desktop)**.
2. Open the **Automations** tab.
3. Download [this repository](https://github.com/al2na/oncology_case_brief_generator/archive/refs/heads/main.zip), unzip it. You will see the automation JSON file `Oncology_case-brief_generator.automation.json`.
5. Input the corresponding clinical PDF reports also in the repository you just downloaded. 
6. Run the automation.
7. Review the generated **Clinical Case Brief**.

## 🧠 Workflow

`Clinical PDFs → Specialist Extraction → Source Verification → Case Synthesis → Final Verification → Clinical Case Brief`

The workflow preserves dates, measurements, uncertainty, and source references. It does not convert planned treatment into completed treatment or silently resolve conflicting information.

## 🔒 Privacy

The automation can be used with cloud-based models or a local AI configuration for more privacy-sensitive workflows.

For demonstrations and testing, synthetic or appropriately de-identified clinical documents are recommended.

## ⚙️ Metadata

* **Format:** `2ndopinion-automation` v1.0
* **Workflow:** `Oncology case-brief generator`
* **Output:** Markdown Clinical Case Brief
* **External Tools:** None

## ⚠️ Disclaimer

This workflow is intended for research, experimentation, workflow prototyping, and clinical decision-support exploration.

Generated summaries must be reviewed against the original medical records by qualified healthcare professionals before clinical use.
