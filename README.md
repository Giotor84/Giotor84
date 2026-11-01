### Gioacchino Tortorici — AI su documenti legali e finanziari in ambienti chiusi

Porto l'AI generativa dove i dati non possono uscire: servicer NPL, SPV, banche e studi di recupero crediti.
Costruisco l'intera catena (acquisizione dei documenti, OCR, estrazione con modelli locali o in cloud privato,
verifica, dashboard) e misuro quanto funziona, anche quando non funziona.

#### Come iniziare

| passo | cosa | durata | che cosa ottenete |
|---|---|---|---|
| **Diagnostica** | un piccolo campione dei vostri documenti, per esempio 10 fascicoli | 2 settimane | errori, casi "da verificare" e tempi misurati, senza impegno a proseguire |
| **Pilota** | un campione più ampio, con un campione di confronto fissato prima di far girare il sistema | 6–8 settimane dall'accesso all'ambiente, secondo il prodotto | report di accuratezza, che mostra anche gli errori, e decisione |
| **Licenza annuale** | prodotto e supporto | annuale | il costo del pilota è scalato dal primo canone se firmate entro 6 mesi |

Tariffa fissa concordata prima dell'avvio. Il lavoro avviene nella vostra infrastruttura o nel vostro account AWS
senza internet, sotto NDA.

**Contatto:** gioacchino.tortorici@gmail.com. Indicate azienda, caso d'uso e volumi indicativi; nessun dato
riservato nel primo messaggio.

---

#### Commercial products (on-premises & air-gapped cloud, available under NDA)

| product | buyer & problem solved | deployment |
|---|---|---|
| **ZT Legal Analysis** | **NPL servicers, banks, SPVs, recovery law firms**: turns credit-recovery dossiers of hundreds of PDFs (native + scanned deeds) into a draft legal report and actionability checklist for lawyer review; amounts, prescription deadlines and chain-of-title guardrails computed in Python | Local GPU or air-gapped AWS (SageMaker + Bedrock) |
| **ZT Orienta** | **Litigation heads & NPL portfolio managers**: extracts structured rulings, norms and debtor exceptions from your private corpus of Italian court decisions, with human review gate and offline forum/section orientation dashboards | Air-gapped AWS or private cloud + offline HTML/Excel |
| **ZT Call Analytics** | **Debt-collection call centers & servicers**: transcribes collection calls with speaker separation, flags promises to pay (amount + ISO date) and compliance issues with verbatim quotes for supervisor review; accuracy measured on your own sample during the pilot | Air-gapped SageMaker + Bedrock or on-prem GPU |

#### Public repositories

| project | what | license |
|---|---|---|
| [**zt-anchor**](https://github.com/Giotor84/zt-anchor) | Document AI that can say "I don't know": verbatim anchoring, abstention, frozen-holdout evaluation, Italian contract lint ([live demo](https://giotor84.github.io/zt-anchor/)) | PolyForm Small Business + commercial |
| [**zt-airgap**](https://github.com/Giotor84/zt-airgap) | Tested template for LLM pipelines on SageMaker with no internet: verified releases via S3, Bedrock via proxy, numbers in Python | Apache-2.0 |
| [**zt-legal-analysis-core**](https://github.com/Giotor84/zt-legal-analysis-core) | Source-available core of ZT Legal Analysis: OCR cascade, resumable checkpoints, rolling synthesis for case files larger than the context, YAML decision rules, LLM adapters | PolyForm Small Business + commercial |
| [**zt-legal-graph**](https://github.com/Giotor84/zt-legal-graph) | Components of a local pipeline for drafting creditor-side replies in Italian civil cases, with claims anchored to a statute graph built from Normattiva | PolyForm Small Business + commercial |
| [**zt-backtest**](https://github.com/Giotor84/zt-backtest) | Honest forecast evaluation: blind windows, baselines to beat, conformal bands | MIT |
| [**zt-whisper-guard**](https://github.com/Giotor84/zt-whisper-guard) | Stops Whisper from inventing text on noisy phone audio | MIT |
| [**zt-memory**](https://github.com/Giotor84/zt-memory) | Local code-context engine + MCP server: makes local and air-gapped LLMs useful on real codebases (right file in context 93–100% vs 21–29% with whole files) | Apache-2.0 |
| [**zt-local-llm-kit**](https://github.com/Giotor84/zt-local-llm-kit) | One-command local coding agent on Windows + safety guards for small models | MIT |
| [**zt-hw-price**](https://github.com/Giotor84/zt-hw-price) | Landed-cost price tracker for local-AI hardware, with tok/s estimates | MIT |

---

#### What I have built in production (client work, described without confidential details)

- **Legal intelligence on case law**: thousands of Italian court decisions turned into a searchable graph of
  rulings, statutes and exceptions; extraction with a private-cloud LLM, human approval before publication,
  offline dashboards for executives and lawyers.
- **From case file to legal report**: OCR cascade and per-document-type extraction over files of hundreds of
  PDFs (mortgages, guarantees, enforcement deeds), producing a narrative report and an action checklist.
- **Call analytics for collections**: on-device transcription with anti-hallucination filters, compliance and
  promise-to-pay scoring, KPI dashboards; plus an offline real-time call translator (no audio leaves the PC).
- **Document acquisition and automation**: supervised document acquisition, legacy terminal automation,
  public-auction extraction with code-side validation.
- **Portfolio analytics**: recovery-rate and collections forecasting with blind-window backtests,
  segmentation by next best action, settlement NPV tools.

Stack: Python · llama.cpp / GGUF · Amazon Bedrock & SageMaker (air-gapped) · Ollama · Whisper · tree-sitter ·
SQLite FTS5 · Playwright · MCP.

---

#### Work with me

- **Diagnostic and pilot** on your own documents or call recordings, at a fixed fee agreed upfront: inside your infrastructure or air-gapped AWS account, under NDA, with the evaluation sample and success criteria fixed before the system runs. The pilot fee is credited toward the first annual license if signed within 6 months.
- **Commercial annual licenses** (at or above the PolyForm Small Business threshold of 100 people or 1M USD revenue) for [zt-anchor](https://github.com/Giotor84/zt-anchor/blob/main/COMMERCIAL.md), [zt-legal-analysis-core](https://github.com/Giotor84/zt-legal-analysis-core/blob/main/COMMERCIAL.md) and [zt-legal-graph](https://github.com/Giotor84/zt-legal-graph/blob/main/COMMERCIAL.md), with a free 90-day internal evaluation.
- **Contact**: gioacchino.tortorici@gmail.com. Please indicate company, use case and approximate volume (never send confidential data in the first message).
