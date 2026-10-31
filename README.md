### Hi, I'm Gioacchino 👋

I bring generative AI into **closed, regulated environments** — banks, credit servicers, law firms — where data
cannot leave the building, personal data must stay protected, and a wrong field has legal consequences.
I build the whole chain: document acquisition, OCR, extraction with local or private-cloud LLMs, verification,
dashboards for management. And I measure honestly how well it works, including when it does not.

🇮🇹 *Porto l'AI generativa in ambienti chiusi e regolamentati (banche, servicer NPL, studi legali): dati che non
escono, privacy protetta, risultati misurati.*

---

#### Open source & source-available

| project | what | license |
|---|---|---|
| [**zt-memory**](https://github.com/Giotor84/zt-memory) | Local code-context engine + MCP server: makes local and air-gapped LLMs useful on real codebases (right file in context 93–100% vs 21–29% with whole files) | Apache-2.0 |
| [**zt-anchor**](https://github.com/Giotor84/zt-anchor) | Document AI that can say "I don't know": verbatim anchoring, abstention, frozen-holdout evaluation, Italian contract lint | PolyForm Small Business + commercial |
| [**zt-whisper-guard**](https://github.com/Giotor84/zt-whisper-guard) | Stops Whisper from inventing text on noisy phone audio | MIT |
| [**zt-local-llm-kit**](https://github.com/Giotor84/zt-local-llm-kit) | One-command local coding agent on Windows + safety guards for small models | MIT |
| [**zt-hw-price**](https://github.com/Giotor84/zt-hw-price) | Landed-cost price tracker for local-AI hardware, with tok/s estimates | MIT |
| [**zt-legal-graph**](https://github.com/Giotor84/zt-legal-graph) | Local pipeline that drafts creditor-side replies in Italian civil cases, every claim anchored to a statute graph built from Normattiva | PolyForm Small Business + commercial |
| [**zt-call-translator**](https://github.com/Giotor84/zt-call-translator) | Real-time call translation for phone operators that never leaves the PC | PolyForm Small Business + commercial |
| [**zt-airgap**](https://github.com/Giotor84/zt-airgap) | Tested template for LLM pipelines on SageMaker with no internet: verified releases via S3, Bedrock via proxy, numbers in Python | Apache-2.0 |
| [**zt-backtest**](https://github.com/Giotor84/zt-backtest) | Honest forecast evaluation: blind windows, baselines to beat, conformal bands | MIT |
| [**zt-legal-analysis-core**](https://github.com/Giotor84/zt-legal-analysis-core) | Open core of ZT Legal Analysis: OCR cascade, resumable checkpoints, rolling synthesis for case files larger than the context, YAML decision rules, LLM adapters | PolyForm Small Business + commercial |

#### Commercial products (on-premises & air-gapped cloud — 4-week paid pilots & annual licenses)

| product | buyer & problem solved | deployment |
|---|---|---|
| **ZT Legal Analysis** | **NPL servicers, banks, SPVs, recovery law firms** — turns credit-recovery dossiers of hundreds of PDFs (native + scanned deeds) into a verified legal report and actionability checklist; amounts, prescription deadlines and chain-of-title guardrails computed in Python | Local GPU or air-gapped AWS (SageMaker + Bedrock) |
| **ZT Orienta** | **Litigation heads & NPL portfolio managers** — extracts structured rulings, norms and debtor exceptions from your private corpus of Italian court decisions, with human review gate and offline forum/section orientation dashboards | Air-gapped AWS or private cloud + offline HTML/Excel |
| **ZT Call Analytics** | **Debt-collection call centers & servicers** — transcribes and audits 100% of collection calls: speaker separation, verified Promise-to-Pay (amount + ISO date), compliance alerts anchored to verbatim quotes, contactability and team coaching | Air-gapped SageMaker + Bedrock or on-prem GPU |

---

#### What I have built in production (client work, described without confidential details)

- **Legal intelligence on case law** — thousands of Italian court decisions turned into a searchable graph of
  rulings, statutes and exceptions; extraction with a private-cloud LLM, human approval before publication,
  offline dashboards for executives and lawyers.
- **From case file to legal report** — OCR cascade and per-document-type extraction over files of hundreds of
  PDFs (mortgages, guarantees, enforcement deeds), producing a narrative report and an action checklist.
- **Call analytics for collections** — on-device transcription with anti-hallucination filters, compliance and
  promise-to-pay scoring, KPI dashboards; plus an offline real-time call translator (no audio leaves the PC).
- **Acquisition and RPA** — portal downloaders with manual login/MFA and minimal footprint, legacy terminal
  automation, public-auction extraction with code-side validation.
- **Portfolio analytics** — recovery-rate and collections forecasting with blind-window backtests,
  segmentation by next best action, settlement NPV tools.

Stack: Python · llama.cpp / GGUF · Amazon Bedrock & SageMaker (air-gapped) · Ollama · Whisper · tree-sitter ·
SQLite FTS5 · Playwright · MCP.

---

#### Work with me

- **4-week paid pilots** on your own documents or call recordings (inside your infrastructure or air-gapped AWS account, under NDA, with frozen-holdout evaluation agreed upfront — pilot fee credited toward the first annual license).
- **Commercial annual licenses** (above the PolyForm Small Business threshold of 100 people / 1M USD revenue) for [zt-anchor](https://github.com/Giotor84/zt-anchor/blob/main/COMMERCIAL.md), [zt-legal-analysis-core](https://github.com/Giotor84/zt-legal-analysis-core/blob/main/COMMERCIAL.md), [zt-legal-graph](https://github.com/Giotor84/zt-legal-graph/blob/main/COMMERCIAL.md) and [zt-call-translator](https://github.com/Giotor84/zt-call-translator/blob/main/COMMERCIAL.md).
- **Direct B2B contact** (private inquiries under NDA, no public GitHub thread required): email **gioacchino.tortorici@gmail.com** or use the contact on my [GitHub profile](https://github.com/Giotor84) — please indicate company, use case and approximate volume (never send confidential data in the first message).
