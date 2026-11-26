<div align="center">

<p><strong>✦ ✦ ✦ &nbsp; PROJECT SYNOPSIS &nbsp; ✦ ✦ ✦</strong></p>

# 🧠 GRAPH NEURAL NETWORK-BASED FINANCIAL FRAUD DETECTION AND INVESTIGATION ENGINE

### GLA UNIVERSITY
**Department of Computer Engineering & Applications**  
**B.Tech - Computer Science and Engineering**  
**(AI / ML and IoT)**

---

## 📘 PROJECT SYNOPSIS

# Graph Neural Network-Based Financial Fraud Detection and Suspicious Transaction Investigation Engine

*A graph-based approach for identifying suspicious transaction patterns, tracing connected activity, and presenting evidence for human review*

| 📌 Field | Details |
|:--|:--|
| **Project team** | Suraksha Squad (T55) |
| **Team Member 1** | Shubhansh Gupta - UR: 2315510204 |
| **Team Member 2** | Rachit Gupta - UR: 2315510159 |
| **Team Member 3** | Saksham Gupta - UR: 2315510180 |
| **Version / Date** | Version 0.1 / 10 October 2026 |

**GLA University**  
17km Stone, NH-19, Mathura-Delhi Road, Chaumuhan, Mathura - 281406, Uttar Pradesh, India

<p><strong>📘 21-PAGE ACADEMIC SYNOPSIS &nbsp; • &nbsp; VERSION 0.1</strong></p>

</div>

---

## 🧭 Contents

<details open>
<summary><strong>📑 Show / hide table of contents</strong></summary>

- [Project Synopsis](#project-synopsis-graph-neural-network-based-financial-fraud-detection-and-suspicious-transaction-investigation-engine)
- [0. Cover and Document Control](#-0-cover-and-document-control)
- [1. Overview](#-1-overview)
- [2. Scope and Control](#-2-scope-and-control)
- [3. Stakeholders and RACI](#-3-stakeholders-and-raci)
- [4. Team and Roles](#-4-team-and-roles)
- [5. Weekwise Plan and Assignments](#-5-weekwise-plan-and-assignments)
- [6. Users and User Experience](#-6-users-and-user-experience)
- [7. Existing Approaches and Project Positioning](#-7-existing-approaches-and-project-positioning)
- [8. Objectives and Success Metrics](#-8-objectives-and-success-metrics)
- [9. Key Features](#-9-key-features)
- [10. System Architecture](#-10-system-architecture)
- [11. Data Design](#-11-data-design)
- [12. Technical Workflow Diagrams](#-12-technical-workflow-diagrams)
- [13. Quality: Non-Functional Requirements and Testing](#-13-quality-non-functional-requirements-and-testing)
- [14. Security and Compliance](#-14-security-and-compliance)
- [15. Delivery and Operations](#-15-delivery-and-operations)
- [16. Risks and Mitigations](#-16-risks-and-mitigations)
- [17. Evaluation Strategy and Success Metrics](#-17-evaluation-strategy-and-success-metrics)
- [18. Appendices](#-18-appendices)

</details>

---

# 📄 Project Synopsis: Graph Neural Network-Based Financial Fraud Detection and Suspicious Transaction Investigation Engine

This synopsis proposes a prototype that represents customers, accounts, devices, merchants and transactions as a connected graph. A Graph Neural Network will learn from both transaction attributes and neighbouring relationships. The system will then rank suspicious activity, retrieve relevant transaction chains or subgraphs, and prepare an evidence bundle for an investigator.

---

# 🗂️ 0. Cover and Document Control

| Field | Details |
|:--|:--|
| Project title | Graph Neural Network-Based Financial Fraud Detection and Suspicious Transaction Investigation Engine |
| Team name and ID | Suraksha Squad (T55) |
| Institute / programme | GLA University / B.Tech CSE (AI/ML and IoT) |
| Document version | V0.1 |
| Date | 10 October 2026 |
| Document status | Project synopsis for academic review |

### 🗂️ Revision History

| Version | Date | Author | Change |
|:--|:--|:--|:--|
| v0.1 | 10 Oct 2026 | Suraksha Squad | Initial synopsis covering graph construction, GNN-based detection, investigation evidence and prototype evaluation. |

---

# 🔎 1. Overview

## 🔍 1.1 Problem Statement

Financial fraud can be difficult to identify when a transaction is examined on its own. A payment may appear normal by amount and timing, while its sender, receiver, device or surrounding transactions form a more concerning pattern. Traditional transaction-level models can miss these relationships when the network context is not represented directly. The project will develop a graph-based detection system in which customers, accounts, devices, merchants and transactions are represented as connected entities. A Graph Neural Network will be used to learn from their features and relationships. The system will assign risk scores, identify suspicious subgraphs or transaction chains, and generate interpretable evidence for each alert.

## 🎯 1.2 Goal

The goal is to build an end-to-end academic prototype that turns financial transaction records into a graph, applies a trained GNN to rank suspicious activity, and gives an analyst enough source-linked evidence to review an alert without relying on an unexplained model score.

## 🚫 1.3 Non-Goals

- The prototype will not make final legal findings or declare a customer guilty of fraud.
- It will not automatically freeze accounts, block payments or replace a bank’s compliance team.
- It will not connect to live banking networks or collect real customer data for the initial demonstration.
- It will not guarantee that every fraud case is detected; performance will depend on data quality, labels and the tested scenarios.
- Large-scale, multi-bank deployment and production-grade real-time streaming are outside the first release.

## 💡 1.4 Value Proposition

The main value of the proposed system is that it combines detection with investigation. The GNN can use relationships that are difficult to capture in a flat transaction table, while graph traversal can show how the flagged activity is connected to other records. The investigator receives a risk-ranked alert, a relevant portion of the graph, a chronological transaction chain where available, and a list of factual indicators that can be checked against source data. The prototype will also compare graph-based performance with conventional models so that the contribution of the graph can be assessed rather than assumed.

---

# 🧩 2. Scope and Control

## ✅ 2.1 In-Scope

- Import and validate transaction, account, customer, device and merchant data from CSV files or a controlled database.
- Build a typed, attributed graph and preserve the transaction IDs and timestamps required for evidence tracing.
- Create historical transaction and graph-structure features without using information from the future.
- Train a transaction-level heterogeneous GNN and compare it with conventional machine-learning baselines.
- Assign a risk score and configurable risk band to each scored transaction.
- Detect selected patterns such as rapid onward transfers, fan-in/fan-out behaviour, cycles and shared-entity relationships.
- Retrieve bounded transaction paths and suspicious subgraphs, subject to defined hop and time limits.
- Generate evidence bundles containing source-linked transactions, relationships, rule triggers and model metadata.
- Provide a web dashboard for reviewing alerts, exploring graphs, viewing timelines and updating investigation cases.
- Evaluate detection, chain retrieval, evidence traceability and system reliability on controlled test data.

## 🚫 2.2 Out-of-Scope

- Direct connection to production banking systems, payment gateways or regulatory reporting systems.
- Automated adverse action against customers without authorised human review.
- A full Know Your Customer (KYC), sanctions-screening or customer identity verification platform.
- A guarantee of real-world fraud detection performance based only on synthetic data.
- Nationwide deployment, multiple-bank tenancy, high-availability clusters and enterprise-scale streaming in the first version.
- Complex natural-language investigation chat, automated filing of Suspicious Transaction Reports, or legal decision-making.

## 🧩 2.3 Assumptions

- A synthetic banking dataset such as IBM AMLSim will be used as the initial data source; its known patterns will be useful for controlled tests [1].
- Where customer, device or merchant relations are absent, additional records may be generated for demonstration, and they will be clearly marked as synthetic.
- Some datasets may have incomplete or delayed labels. Unknown labels will not be treated automatically as legitimate transactions.
- The initial experiment will focus on transaction-level labels. Account- or subgraph-level predictions will be added only if a defensible target definition is available.
- The system will be developed as a research prototype and will use a manageable graph size suitable for the team’s available hardware.

## ⛓️ 2.4 Constraints

| Constraint | Effect on the project | Response |
|:--|:--|:--|
| Time | A limited academic development period | Prioritise batch ingestion, transaction-level GNN, bounded graph search and an evidence dashboard. |
| Compute | Graph training can become expensive as neighbourhoods grow | Start with a small graph, two message-passing layers and sampled neighbourhoods if needed. |
| Labels | Fraud labels may be sparse or synthetic | Report class balance and evaluate with precision-recall metrics; do not overstate generalisation. |
| Data access | Real financial records may not be available | Use synthetic data and document all generated attributes. |

| Constraint | Effect on the project | Response |
|:--|:--|:--|
| Integration | Database, model and frontend components have different data formats | Define stable schemas and API contracts early; test modules separately and together. |

## 🔗 2.5 Dependencies

| Dependency | Purpose |
|:--|:--|
| IBM AMLSim / prepared CSV dataset | Generate or obtain synthetic transaction records and known suspicious patterns [1]. |
| Python, pandas and NumPy | Data validation, preprocessing and feature creation. |
| PyTorch and PyTorch Geometric | Model training and heterogeneous graph data representation [2]. |
| Neo4j (optional graph database) | Graph exploration, bounded path queries and relationship visualisation [4]. |
| PostgreSQL | Store canonical records, model predictions, alerts, cases and audit history. |
| FastAPI and React | Expose services and build the analyst interface. |
| Git and Docker Compose | Version control, repeatable setup and local integration testing. |

## ☑️ 2.6 Acceptance Criteria

| Scenario | Expected result |
|:--|:--|
| Graph integrity | Every relationship used in an alert maps to an existing entity or transaction record; orphan references are reported. |
| Risk scoring | The trained model returns a valid score, a model version and a timestamp for each supported test transaction. |
| Suspicious-chain retrieval | Known paths in controlled fixtures are recovered within the configured hop and time limits. |
| Evidence provenance | All transaction facts in an evidence bundle link back to source records; provenance coverage target is 100%. |
| Explanation | An alert shows model output separately from factual records and rule-based indicators. |
| Case workflow | An investigator can open a case, inspect evidence, add notes, change status and retain an audit event. |
| Evaluation | The report contains time-aware test metrics and a comparison with at least one conventional baseline. |
| Stability | A scripted end-to-end test run completes without a critical application crash. |

---

# 👥 3. Stakeholders and RACI

The main stakeholders are the project team and analysts who would use an investigation tool, and the institution reviewing the prototype. The real-world users are represented through requirements and usability scenarios; the prototype will not be connected to a bank’s live operations.

| Activity | Responsible (R) | Accountable (A) | Consulted (C) | Informed (I) |
|:--|:--|:--|:--|:--|
| Requirements and planning | Shubhansh Gupta | Shubhansh Gupta | Team | Team |
| Graph schema and data pipeline | Saksham Gupta | Saksham Gupta | Shubhansh, Rachit | Team |
| GNN design and training | Shubhansh Gupta | Shubhansh Gupta | Saksham | Team |
| Backend and graph search | Rachit Gupta | Rachit Gupta | Saksham, Shubhansh | Team |
| Dashboard and case workflow | Rachit Gupta | Rachit Gupta | Saksham | Team |
| Integration and evidence design | Saksham Gupta | Saksham Gupta | Shubhansh, Rachit | Team |
| Testing and evaluation | All team members | Shubhansh Gupta | Team | Team |
| Final review and delivery | All team members | Suraksha Squad | Team | Team / department |

R = performs the work; A = owns the final outcome; C = provides input; I = receives progress information.

---

# 🧑‍💻 4. Team and Roles

| Member | Role | Responsibilities | Availability |
|:--|:--|:--|:--|
| Shubhansh Gupta | GNN / ML Developer | Define prediction target and features; train GNN and tabular baselines; manage temporal splits, metrics and model versioning. | Approx. 10-15 hrs/week |
| Rachit Gupta | Full Stack Developer | Develop FastAPI endpoints, graph queries and the analyst dashboard; implement alert filters and evidence display. | Approx. 10-15 hrs/week |
| Saksham Gupta | Data and Integration Engineer | Prepare datasets, build graph snapshots, link source records, integrate model and backend, and create repeatable tests. | Approx. 10-15 hrs/week |

Responsibilities are a proposed allocation and can be adjusted after the first review. All team members will take part in end-to-end testing, documentation and the final demonstration.

---

# 🗓️ 5. Weekwise Plan and Assignments

The project is planned over eight weeks. The first version focuses on batch data, transaction-level prediction and evidence-based investigation. Streaming and advanced model extensions will be considered only after the core workflow is stable.

| Week | Focus | Planned work | Deliverable |
|:--|:--|:--|:--|
| Week 1 | Requirements and design | Confirm problem scope, select the data source, define labels and draw the initial architecture. | Requirements document, dataset decision, first graph schema. |
| Week 2 | Data pipeline and baseline | Validate records; build transaction-level features; implement logistic regression or tree-based baseline. | Clean dataset, label summary, baseline metrics. |
| Week 3 | Graph construction | Define typed nodes and relations, generate graph snapshots and verify references. | Graph builder, graph integrity tests, initial visualisation. |
| Week 4 | GNN implementation | Implement a small heterogeneous GNN and train using time-aware train/validation/test splits. | Saved model checkpoint and preliminary evaluation. |
| Week 5 | Risk scoring and pattern rules | Create score thresholds, rapid-transfer rules, fan-in/fan-out checks and bounded path retrieval. | Ranked alerts with linked transaction chains. |
| Week 6 | Investigation evidence | Build evidence bundles, model explanations, source links and case status history. | Investigation API and test cases for evidence provenance. |
| Week 7 | Frontend and integration | Develop alert queue, graph explorer and case workspace; connect API, graph store and model. | Integrated prototype and end-to-end demonstration. |
| Week 8 | Evaluation and delivery | Run test scenarios, compare baselines, document limits, fix critical defects and prepare presentation. | Final report, reproducible code, metrics and demonstration package. |

## 🛠️ 5.1 Working Method

- Use Git branches and short, reviewable commits so that data, model and interface work can be integrated throughout the project.
- Run a small integration test at the end of each week rather than waiting until the final week.
- Keep an experiment log containing dataset version, feature configuration, random seed, model parameters and metrics.
- Defer optional work such as streaming or a temporal GNN if the core evidence workflow is not yet reliable.

---

# 🧭 6. Users and User Experience

## 👤 6.1 User Personas

| User | Main need | Interface support |
|:--|:--|:--|
| Fraud investigator | Understand why an alert was raised and what records support it. | Risk-ranked queue, transaction timeline, graph view, source links and case notes. |
| Investigation supervisor | Prioritise cases and review how decisions were recorded. | Case status filters, evidence completeness, workload view and audit history. |
| Model administrator | Check whether the model is behaving as expected. | Version, evaluation metrics, score distributions and data-quality warnings. |
| Project tester | Reproduce a scenario and verify the expected outcome. | Dataset/run identifier, filters, test logs and synthetic case fixtures. |

## 🧭 6.2 Main User Journey

1. A scheduled scoring run or a test transaction creates a candidate alert.
2. The investigator opens the alert and reviews its score, model version and triggered rules.
3. The investigator opens the graph panel to inspect nearby accounts, devices, merchants and transactions.
4. The evidence panel displays source-linked facts and the chronological order of any retrieved transaction chain.
5. The investigator records a status, explanation or request for additional information.
6. The decision and subsequent changes are saved to the case history for later review.

## 💬 6.3 User Stories

As an investigator, I want each alert to show the transactions and relationships that contributed to the concern, so that I can check the facts before escalating it.  
As a supervisor, I want to filter cases by status and review their audit history, so that pending work and prior decisions are visible.  
As a model administrator, I want to compare the GNN with a conventional baseline on a held-out time period, so that the value of graph learning is measured rather than assumed.

## 🎨 6.4 UX Principles

- Show the risk score, facts, rule triggers and model explanation as separate items.
- Use clear labels for account, customer, device, merchant and transaction nodes.
- Make every graph edge inspectable and traceable to a relationship or transaction record.
- Use neutral language such as “requires review” instead of declaring a customer fraudulent.
- Keep the dashboard readable at laptop resolution and provide table-based alternatives to graph visualisation.

---

# 🧪 7. Existing Approaches and Project Positioning

The project will be compared with common categories of financial fraud detection rather than claiming to replace commercial banking platforms. The comparison is intended to explain where graph learning may help and what must be tested.

| Approach | Strength | Limitation addressed by this project |
|:--|:--|:--|
| Rule-based systems | Transparent and easy to audit for known patterns. | Rules may miss patterns that are spread across several entity types or differ from predefined templates. |
| Traditional tabular ML | Can learn from amounts, timestamps, account statistics and other structured features. | Relationships between accounts and other entities may be difficult to represent without engineered aggregates. |
| Graph algorithms and network rules | Useful for paths, communities, centrality and defined network motifs [4]. | Often depend on selected graph measures or hand-designed thresholds; they do not automatically learn a fraud classifier. |

| Approach | Strength | Limitation addressed by this project |
|:--|:--|:--|
| Graph Neural Networks | Can learn from node features and neighbouring graph structure [2]. | Need careful label handling, temporal validation, interpretability and safeguards against noisy links. |
| Proposed hybrid engine | Combines a GNN, configurable pattern rules, bounded path retrieval and evidence generation. | Its value must be established through comparison and evidence-quality tests; no performance advantage is assumed in advance. |

## 🧭 7.1 Project Positioning

The intended difference is the link between detection and investigation. The GNN will rank candidate transactions; graph algorithms will retrieve the surrounding chain or subgraph; and the evidence service will attach source identifiers, timestamps, rule results and model metadata. This gives the user both a prediction and a way to examine it. Prior work has also explored scalable graph learning for anti-money-laundering analysis on synthetic transaction graphs, although this does not by itself establish performance on live financial data [6].

---

# 🎯 8. Objectives and Success Metrics

| Objective | Measure | Proposed acceptance target |
|:--|:--|:--|
| O1. Detect suspicious transactions | Average Precision / PR-AUC, precision, recall and precision@K on a held-out time period. | Report results for GNN and at least one tabular baseline; investigate any difference instead of relying on accuracy alone. |
| O2. Make risk ranking useful | Recall among the top K alerts or within a fixed review budget. | Select K from a stated review-capacity assumption and report the resulting precision and recall. |
| O3. Recover transaction chains | Path recovery rate on known synthetic test patterns. | Recover at least 90% of the selected, bounded test chains under the stated graph and time constraints. |
| O4. Provide traceable evidence | Share of factual evidence items linked to source record IDs. | 100% of transaction facts shown in generated evidence must contain a source reference. |
| O5. Support investigation | Case workflow tests and usability observations. | All defined core case actions must pass scripted end-to-end tests. |
| O6. Keep prototype responsive | Latency for a single score request and bounded graph query on the test environment. | Aim for under 2 seconds for the standard test case; report hardware and graph size. |
| O7. Make experiments reproducible | Ability to recreate a run using stored versions and configuration. | Save data split, seed, features, model version and metrics for each reported run. |

The targets above are proposed engineering targets for the prototype. They are not achieved results. The final report will state the measured values, dataset limitations and any target that could not be met.

---

# 🧰 9. Key Features

| Priority | Feature | Description / acceptance idea |
|:--|:--|:--|
| Must | Heterogeneous graph | Represent customers, accounts, devices, merchants and transactions as typed nodes and preserve relationship direction. |
| Must | GNN-based risk scoring | Produce a risk score for supported transactions and store model/version metadata. |
| Must | Baseline comparison | Evaluate a conventional transaction model with the same time-aware split. |
| Must | Suspicious-chain retrieval | Retrieve relevant bounded paths with transaction IDs and timestamps. |
| Must | Evidence bundle | Show source-linked facts, rule triggers, graph context and model explanation. |
| Must | Investigation workflow | Allow case review, notes, status changes and audit history. |
| Should | Shared-entity analysis | Surface accounts linked through the same device or another supported identifier. |
| Should | Subgraph ranking | Prioritise connected groups using model results and validated pattern evidence. |
| Could | Temporal GNN | Explore a time-aware graph model if the initial implementation and data volume justify it. |
| Could | Feedback loop | Use authorised reviewed outcomes for later evaluation or retraining, with controls to avoid label leakage. |

---

# 🏗️ 10. System Architecture

The design uses separate modules for data preparation, graph construction, model inference, pattern discovery, evidence generation and case management. This separation will make it easier to test each component and to trace an alert back to the records that produced it.

## 🧱 10.1 Main Components

| Component | Responsibility |
|:--|:--|
| Data ingestion and validation | Load records, standardise timestamps and amounts, detect duplicates and reject broken identifiers. |
| Canonical data store | Keep the source entities, transactions, labels, scoring results, alerts and case records. |
| Graph builder | Create typed nodes and relationships, generate feature tensors and verify graph integrity. |
| GNN service | Load a versioned model and feature configuration, then score eligible transactions. |
| Pattern and risk engine | Apply explicit rules such as rapid onward transfer, fan-in/fan-out and bounded cycles. |
| Graph investigation service | Retrieve bounded paths, linked entities and candidate subgraphs for a selected alert. |
| Evidence and case service | Combine source records, rule outcomes and model explanations into a traceable case. |
| API and dashboard | Expose the workflow to authorised users and show alerts, graphs, evidence and case status. |

## ⚙️ 10.2 Processing Mode

The first implementation will use batch ingestion and batch scoring. Once graph construction, scoring and evidence retrieval are stable, the same interfaces can be extended to accept streaming events. Streaming is an optional later stage rather than a dependency for proving the central idea.

## 💻 10.3 Technology Selection

Python is proposed for preprocessing, training and the API. PyTorch Geometric supports heterogeneous graph data, where different node and edge types can hold different features [2]. Neo4j can be used for graph exploration and path queries [4], while PostgreSQL will store canonical rows and investigation history. React will provide the dashboard. This stack is proposed for the prototype; final versions should be pinned in the repository.

---

# 🗃️ 11. Data Design

## 🗃️ 11.1 Core Entities and Attributes

| Entity | Primary key | Example attributes |
|:--|:--|:--|
| Customer | customer_id | Account tenure, historical activity summaries, permitted risk history |
| Account | account_id | customer_id, account age, inbound/outbound activity counts and amounts |
| Device | device_id | Device age, activity frequency, linked account count |
| Merchant | merchant_id | Merchant category, volume, typical amount and linked account count |
| Transaction | transaction_id | sender account, receiver account or merchant, amount, currency, timestamp, status, channel |
| Alert | alert_id | transaction_id, risk score, score type, model version, trigger source and creation time |
| Investigation case | case_id | status, assignee, created_at, updated_at, outcome and review notes |
| Evidence item | evidence_id | case_id, evidence type, source record reference, facts, generation time |

## 🔀 11.2 Graph Relationships

| Relationship | Meaning | Notes |
|:--|:--|:--|
| Customer -> Account | Customer owns an account | Use a source-supported ownership mapping. |
| Customer -> Device | Customer uses a device | Keep this relation distinct from account ownership. |
| Account -> Transaction | Account sends or receives a transaction | Transaction node retains its own ID and attributes. |
| Transaction -> Account | Transaction credits a receiving account | Direction matters for money-flow analysis. |
| Transaction -> Merchant | Transaction pays a merchant | Use only when the payment has a merchant recipient. |
| Device -> Transaction | Device initiates a transaction | Optional where the source records a device association. |
| Account -> Account | Derived money-flow link | Store reference to the underlying transaction ID; do not imply reverse money flow. |

## 🧮 11.3 Feature Groups

- Transaction features: log amount, channel, type, time-of-day, time since earlier activity and rolling counts from prior events only.
- Account features: inbound/outbound volume, distinct counterparties, recent activity changes and account age at transaction time.
- Device and merchant features: linked-account count, usage frequency, merchant category and transaction-volume changes.
- Graph features: relation-specific degree, bounded neighbourhood counts, fan-in/fan-out, connected-group statistics and eligible prior-risk indicators.
- Labels and provenance: label source, observation time and unknown-label status. Validate identifiers, document missing values, use only information available at scoring time and mask unknown labels.

---

# 📊 12. Technical Workflow Diagrams

## 🔄 12.1 State Transition Diagram

The diagram describes the alert and case lifecycle. A model alert is a request for review, not a final fraud decision. Cases can return to review when additional information arrives, and each status change should be recorded.

<div align="center">

![*Figure 1. Proposed alert and investigation states.*](C:\Users\rachi\T55-Graph-Neural-Network-Based-Financial-Fraud-Detection-and-Suspicious-Transaction-Investigation-En\state_transition_daigram.png)

</div>

## 🔁 12.2 Sequence Diagram

The sequence begins when the API receives a scoring or review request. Source records are validated, the scoring service returns a versioned result, the graph service retrieves bounded paths, and the evidence service stores the generated case details.

<div align="center">

![*Figure 2. Sequence of scoring, path retrieval and evidence generation.*](C:\Users\rachi\T55-Graph-Neural-Network-Based-Financial-Fraud-Detection-and-Suspicious-Transaction-Investigation-En\sequence_daigram.png)

</div>

## 👥 12.3 Use Case Diagram

The investigator reviews alerts and cases; a model administrator checks model performance and approved versions; and a supervisor reviews workload and case history. Training and model promotion are not exposed as unrestricted actions to all dashboard users.

<div align="center">

![*Figure 3. Principal users and supported use cases.*](C:\Users\rachi\T55-Graph-Neural-Network-Based-Financial-Fraud-Detection-and-Suspicious-Transaction-Investigation-En\use_case_daigram.png)

</div>

## 🔃 12.4 Data Flow Diagram

Validated source data feeds the canonical store and graph builder. The GNN and pattern engine generate candidate alerts. The investigation service combines their outputs with source records and graph paths before the dashboard displays the case.

<div align="center">

![*Figure 4. Level-1 movement of data through the system.*](C:\Users\rachi\T55-Graph-Neural-Network-Based-Financial-Fraud-Detection-and-Suspicious-Transaction-Investigation-En\data_flow_daigram.png)

</div>

## 🗂️ 12.5 ER Diagram

The core schema separates source financial entities from alerts, cases and evidence. This allows an alert to refer to an original transaction without copying the transaction into the case record as the only source of truth.

<div align="center">

![*Figure 5. Entity-relationship view of the main records.*](C:\Users\rachi\T55-Graph-Neural-Network-Based-Financial-Fraud-Detection-and-Suspicious-Transaction-Investigation-En\er_daigram.png)

</div>

## 🧭 12.6 Technical Workflow Diagram

<div align="center">

![*Figure 6. End-to-end development and investigation workflow.*](C:\Users\rachi\T55-Graph-Neural-Network-Based-Financial-Fraud-Detection-and-Suspicious-Transaction-Investigation-En\technical_workflow_daigram.png)

</div>

## 🏗️ 12.7 Work Architecture Diagram

The architecture keeps the model, graph search, canonical database and interface loosely coupled. The scoring and evidence services will exchange versioned payloads rather than depending on frontend-specific logic.

<div align="center">

![*Figure 7. Component-level work architecture.*](C:\Users\rachi\T55-Graph-Neural-Network-Based-Financial-Fraud-Detection-and-Suspicious-Transaction-Investigation-En\work_architecture_daigram.png)

</div>

---

# 🛡️ 13. Quality: Non-Functional Requirements and Testing

## 🛡️ 13.1 Non-Functional Requirements

| Quality area | Proposed target / rule | Measurement |
|:--|:--|:--|
| Performance | Aim for under 2 seconds for a standard single-transaction score and bounded evidence query on the documented test setup. | Record latency, graph size, and machine specifications. |
| Reliability | No critical crashes during the agreed end-to-end test suite. | Automated pass/fail results and error logs. |
| Evidence integrity | Every factual transaction detail displayed in an evidence item links to a source record. | Automated provenance coverage check; target 100%. |
| Reproducibility | Each experiment records data version, seed, feature configuration, split and model version. | Repeat a selected run and compare outputs and metrics. |
| Security | Restrict model administration and case decisions to authorised roles. | Role-based API and dashboard tests. |
| Privacy | Use synthetic data for demonstrations; avoid storing unnecessary personal information. | Inspect sample records and logs. |
| Maintainability | Separate graph building, scoring, discovery, evidence and UI modules. | Code review, typed API schemas and unit tests. |
| Auditability | Record score version, rule version, case status changes and evidence-generation time. | Audit completeness checks. |

## 🧪 13.2 Test Plan

| Test level | What will be tested | Exit condition |
|:--|:--|:--|
| Unit tests | Feature calculations, time-window boundaries, score conversion, risk-band thresholds and schema validation. | Critical calculations and validation rules pass. |
| Graph integrity tests | Node identifiers, relationship direction, referential integrity and transaction provenance. | No unreported broken references in the selected dataset. |
| Model tests | Training convergence, output shape, unknown-label masking and prediction reproducibility. | Model returns valid scores and evaluation artifacts are saved. |
| Integration tests | API to database, API to graph store, scoring to alert creation and evidence retrieval. | Expected records flow across module boundaries. |
| End-to-end tests | Create alert, open case, inspect graph, view evidence, update status and audit trail. | All agreed core journeys pass. |
| Security tests | Authentication, role permissions, input validation and restricted query access. | Unauthorised actions are rejected. |
| Performance tests | Single scoring request and bounded graph queries on sample graph. | Measured results are documented against the proposed target. |

## 🖥️ 13.3 Environments

- Development: individual machines with version-controlled code and small synthetic fixtures.
- Integration / staging: one consistent environment running the API, database, graph service and dashboard using Docker Compose.
- Demo: a fixed dataset and saved model checkpoint with documented configuration so the demonstration can be repeated.

---

# 🔐 14. Security and Compliance

## ⚠️ 14.1 Threat Model

| Asset / surface | Potential threat | Mitigation |
|:--|:--|:--|
| Transaction and entity data | Unauthorised access or accidental exposure. | Use synthetic data for the prototype, limit privileges, avoid secrets in source control and restrict logs. |
| Graph relationships | Incorrect or manipulated links create misleading paths. | Validate relationship provenance, retain source IDs and report data-quality exceptions. |
| Model and feature files | Unauthorised changes or an untracked checkpoint. | Store model versions and configuration hashes; restrict write access. |
| Prediction API | Malformed requests, excessive requests or arbitrary query injection. | Validate schemas, use parameterised queries, add rate limits if exposed beyond local testing. |
| Investigation cases | Unauthorised change to a decision or evidence. | Role-based permissions and append-only audit events for state changes. |
| Model outputs | An alert is treated as proof of wrongdoing. | Use review-oriented language, show evidence and limitations, require human decisions. |
| Label pipeline | Future information or unverified labels leak into training. | Time-aware splits, label provenance and documented eligibility rules. |

## 🔐 14.2 Authentication and Authorisation

The prototype will provide basic authenticated access for team members and separate investigator from model-administrator permissions. Training, threshold changes and model version promotion should be restricted. A user should not be able to modify model output by editing the displayed score in the browser.

## 🧾 14.3 Audit and Logging

The system will record scoring time, model version, rule version, case creation, investigator assignment, status changes and evidence generation. Logs should contain enough information to reproduce the flow without unnecessarily copying sensitive transaction data. For the synthetic prototype, a short documented retention period will be used; retention for a real institution would require a separate policy.

## ⚖️ 14.4 Compliance and Responsible Use

This academic prototype is not a production financial compliance service. If real financial data is ever introduced, the project would need institutional approval and a review of applicable privacy, security, retention and financial-sector requirements before processing it. No real customer data is required for the planned demonstration. Third-party datasets and libraries will be credited, and their licences will be checked before redistribution.

---

# 🚀 15. Delivery and Operations

## 🚀 15.1 Release Plan

| Release | Timing | Contents |
|:--|:--|:--|
| Alpha | End of Week 3 | Clean data pipeline, graph builder and conventional baseline. |
| Beta | End of Week 5 | First trained GNN, scoring API, risk-ranked alerts and transaction-chain search. |
| Candidate release | End of Week 7 | Evidence bundle, dashboard and case workflow integrated. |
| v1.0 demo | End of Week 8 | Evaluation results, documented limitations, reproducible setup and final demonstration. |

## 🔁 15.2 Version Control and Reproducibility

- Keep model checkpoints, feature configuration, rule configuration and code under version control or a versioned artifact store, subject to file size.
- Pin dependency versions and keep a short setup guide for Python, the graph database and frontend.
- Record the graph snapshot date range and the label/split policy used for every training run.
- Run automated tests before merging changes to the main branch.

## 📡 15.3 Monitoring

For the prototype, monitoring will focus on failed ingestion jobs, broken graph references, scoring errors, unexpected alert-volume changes and evidence-generation failures. If authorised labels later become available, the team can assess changes in PR-AUC, precision at a review budget and calibration. Drift indicators are warning signals and should not automatically trigger retraining without review.

## 📣 15.4 Communication Plan

The team will review progress at least once each week, keep a short list of open risks and decisions, and demonstrate the integrated workflow at the mid-point and final review. The mentor will be consulted when scope, data assumptions or the evaluation plan needs to change.

---

# ⚠️ 16. Risks and Mitigations

| Risk | Possible effect | Mitigation |
|:--|:--|:--|
| Incomplete labels | Model metrics may be misleading and legitimate cases may be treated as negatives. | Keep unknown labels separate, inspect the data dictionary, report label coverage and use appropriate masks. |
| Temporal leakage | Test scores overstate what a live system could achieve. | Split by transaction time and calculate features using only prior information. |
| GNN does not outperform baseline | Graph learning adds complexity without measurable predictive benefit. | Run a fair baseline comparison and retain the simpler model if it performs better. |
| Noisy entity links | Shared devices or identifiers create false associations. | Keep relationship provenance, assess link quality and avoid treating shared entities as proof. |
| Path explosion | Many graph paths cause high latency or huge evidence bundles. | Limit hop count, look-back window, result count and query runtime. |
| Synthetic-data bias | Patterns in simulation may not reflect actual financial crime. | State the limitation clearly and avoid claiming real-world effectiveness. |
| Compute limits | Large graphs or training runs exceed available resources. | Start small, sample neighbourhoods and use batch scoring. |
| Poor model explanation | A highlighted edge is mistaken for causal proof. | Show the explainer output separately from factual source evidence and include caveats. |
| Integration delays | Backend, graph, model and UI fail to work together in time. | Agree API contracts early and integrate thin vertical slices each week. |
| Privacy or access mistake | Sensitive records or decisions become available to the wrong user. | Use synthetic data, role permissions, minimal logs and security tests. |

Risk review is part of the weekly check-in. If time becomes limited, the order of priority is: reliable graph and data provenance, model evaluation, chain retrieval, evidence generation, and then optional advanced features.

---

# 📈 17. Evaluation Strategy and Success Metrics

## 🧪 17.1 Experimental Setup

- Create separate training, validation and test periods where timestamps allow it; do not tune thresholds on the final test set.
- Report dataset source, number of entities and transactions, label distribution, unknown-label handling, time period and preprocessing version.
- Compare a rule-based detector, a conventional tabular classifier and the proposed GNN using compatible data and the same test period.
- Repeat experiments with fixed seeds where practical and record run-to-run variation.
- Use known synthetic patterns to evaluate graph-path retrieval independently of transaction classification.

## 📊 17.2 Model Metrics

| Metric | Reason for use |
|:--|:--|
| Precision and recall | Show the trade-off between alert quality and the proportion of labelled cases detected. |
| F1-score | Provides one summary when precision and recall both matter. |
| Average Precision / PR-AUC | Useful for ranking under class imbalance; report the positive-class prevalence as context [5]. |
| Precision@K / Recall@K | Reflects a fixed analyst review capacity. |
| Calibration / Brier score | Use when the score is presented as a probability and calibration has been evaluated. |

## 🔎 17.3 Investigation Metrics

| Metric | Measurement approach |
|:--|:--|
| Chain recovery | Percentage of known test chains recovered within configured limits. |
| Entity / transaction retrieval precision | Share of retrieved items belonging to the known test pattern or approved ground truth. |
| Evidence completeness | Share of alerts containing required source IDs, timestamps, rules and model version. |
| Timeline correctness | Check that displayed transactions are ordered by source timestamp and amounts are not altered. |
| Case workflow completion | Pass rate of scripted case review, status update and audit-history scenarios. |
| Review time | Optional small usability exercise comparing the time required to understand an alert. |

## 📝 17.4 Reporting and Interpretation

Results will be reported as measured values rather than targets. If the GNN does not outperform a simpler model, this will be documented as a meaningful finding. A high score on a synthetic benchmark does not establish performance on live banking data. Any demonstration of suspicious links will be described as a candidate pattern for review unless it is supported by an appropriate verified label.

---

# 📚 18. Appendices

## 📖 18.1 Glossary

| Term | Meaning in this project |
|:--|:--|
| Graph | A representation consisting of entities (nodes) connected by relationships (edges). |
| Heterogeneous graph | A graph containing different node types and/or relationship types. |
| Graph Neural Network (GNN) | A neural network that learns from node features and their graph neighbourhoods. |
| Transaction chain | An ordered path of transactions or accounts showing a sequence of money movement. |
| Subgraph | A selected portion of the graph investigated as a group. |
| Risk score | A model or ranking output used to prioritise activity; not proof of fraud. |
| Temporal leakage | Use of information from after the prediction time in model features or evaluation. |
| Precision / Recall | Measures of alert correctness and the share of labelled positives found. |
| GNNExplainer | A method for identifying graph structure and input features relevant to a GNN prediction [3]. |
| AMLSim | An open-source simulator for synthetic banking transactions and known money-laundering patterns [1]. |
| PR-AUC / Average Precision | A summary of precision-recall ranking performance across thresholds. |
| Evidence provenance | A traceable reference showing which original record supports a displayed fact. |

## 🔗 18.2 References

[1] IBM, “AMLSim: Anti-Money Laundering Simulator,” project repository and documentation. Available: https://github.com/IBM/AMLSim (accessed 10 October 2026).  
[2] PyTorch Geometric, “Heterogeneous Graph Learning” and “torch_geometric.data.HeteroData” documentation. Available: https://pytorch-geometric.readthedocs.io/en/stable/ (accessed 10 October 2026).  
[3] Z. Ying, D. Bourgeois, J. You, M. Zitnik and J. Leskovec, “GNNExplainer: Generating Explanations for Graph Neural Networks,” Advances in Neural Information Processing Systems 32, 2019. Available: https://proceedings.neurips.cc/paper_files/paper/2019/hash/d80b7040b773199015de6d3b4293c8ff-Abstract.html.  
[4] Neo4j, “Graph Data Science Library: Algorithms and Path Finding,” official documentation. Available: https://neo4j.com/docs/graph-data-science/current/algorithms/ (accessed 10 October 2026).  
[5] scikit-learn developers, “Model Evaluation: Precision, Recall, F-measure and Average Precision,” official documentation. Available: https://scikit-learn.org/stable/modules/model_evaluation.html (accessed 10 October 2026).  
[6] M. Weber, J. Chen, T. Suzumura, A. Pareja, T. Ma, H. Kanezashi, T. Kaler, C. E. Leiserson and T. B. Schardl, “Scalable Graph Learning for Anti-Money Laundering: A First Look,” NeurIPS Workshop on Challenges and Opportunities for AI in Financial Services, 2018. Available: https://arxiv.org/abs/1812.00076.

## ⚠️ 18.3 Limitations of the Proposed Study

The prototype will depend on the structure and quality of the selected dataset. Synthetic transaction patterns are useful for controlled evaluation but may not represent the full range of behaviour in real financial systems. Entity links can be incomplete or noisy, fraud labels can be delayed, and model explanations do not establish causality. The study will therefore report data limitations alongside its metrics and keep final decisions with a human reviewer.

## 📦 18.4 Expected Deliverables

- Documented graph schema, data-preparation pipeline and synthetic test fixtures.
- Trained GNN model and a conventional baseline with reproducible evaluation scripts.
- Risk-scoring service and rule-based candidate-alert generation.
- Bounded transaction-chain and subgraph retrieval module.
- Evidence-generation service and investigation case workflow.
- Dashboard for alert review, graph exploration and case history.
- Final evaluation report, setup guide and source-code package.

## 🏁 18.5 Concluding Note

The proposed work is intended to demonstrate a complete, testable path from financial records to graph-based risk ranking and evidence-led investigation. Its value will be judged by the quality of the evaluation and by whether an analyst can follow the evidence back to the original records. The first release will remain a controlled academic prototype; further deployment would require additional data validation, security review and testing with authorised real-world data.

## 🌱 18.6 Future Enhancements

- Explore temporal GNN architectures that model changes in transaction relationships over time.
- Add streaming ingestion and incremental graph updates after batch scoring is stable.
- Use authorised investigator feedback for later evaluation or retraining, with label governance and leakage checks.
- Test on suitably anonymised, authorised institutional data before making claims about real-world performance.

---

<div align="center">

**GLA University**  
**GRAPH NEURAL NETWORK-BASED FINANCIAL FRAUD DETECTION AND INVESTIGATION ENGINE**

</div>