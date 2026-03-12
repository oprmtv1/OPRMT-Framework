

| OPRMT™ FRAMEWORK OFFICIAL SPECIFICATION DOCUMENT Version 1.0  |  OPRMT™ Standards Initiative  |  © 2026 Michael W. Fleming |
| :---: |

**CLASSIFICATION: Proprietary — Internal and Licensed Use Only**

Document Control: OPRMT-SPEC-001-v1.0

Issuing Authority: OPRMT™ Standards Initiative

Effective Date: 2026

Contact: engineering@oprmt.solutions

# **Executive Summary**

The OPRMT™ Framework is a structured prompt engineering methodology developed by Michael W. Fleming under the OPRMT™ Standards Initiative. It defines a five-component architecture for constructing, governing, versioning, and validating AI prompts across enterprise, commercial, and operational contexts.

This specification establishes the authoritative reference for all OPRMT™ prompt construction, library publishing, compliance scoring, and derivative framework development. All licensees, contributors, and platform integrations must conform to the standards defined herein.

The framework addresses three systemic failures observed in enterprise AI adoption:

* Prompts constructed without structural rigor, producing inconsistent and ungovernable outputs.

* No standardized mechanism for versioning, auditing, or validating prompt performance over time.

* Absence of a portable, model-agnostic specification that survives across LLM generations.

OPRMT™ resolves these failures through five deterministic components, a compliance scoring system, and a version control protocol compatible with Git-based workflows.

# **1\. Framework Overview**

## **1.1 Purpose and Scope**

The OPRMT™ Framework provides a universal architecture for prompt engineering that is applicable across industries, AI platforms, and use cases. It is designed to function as both a construction standard and a governance protocol — enabling organizations to build, audit, and scale their prompt operations with the same rigor applied to software engineering.

This specification governs:

* Prompt construction and structural compliance

* Metadata standards for commercial prompt library publication

* Compliance scoring via the Deterministic Compliance Index (DCI™)

* Version control conventions for prompt lifecycle management

* Variable injection standards for universal reuse

## **1.2 Founding Principles**

| Principle | Definition |
| :---- | :---- |
| Determinism | Prompt outputs must be reproducible given identical inputs. Structure eliminates ambiguity. |
| Portability | Prompts must function across AI models without structural revision. Logic is model-agnostic. |
| Governance | Every prompt must carry verifiable metadata, a version record, and a compliance signature. |
| Commercialization | Framework-compliant prompts are publishable intellectual property, not disposable queries. |
| Scalability | The framework must accommodate single-use prompts and enterprise-scale prompt operations equally. |

## **1.3 Framework Position**

OPRMT™ occupies the intersection of prompt engineering, knowledge management, and operational governance. It is not a prompt template library. It is not an AI product. It is a specification layer — analogous in function to a software architecture standard or a legal document drafting protocol.

# **2\. The Five-Component Architecture**

Every OPRMT™-compliant prompt must contain exactly five structural components, executed in sequence. Each component is labeled with its designator and maps to a specific function within the prompt's operational logic.

| CORE ARCHITECTURE: O · P · R · M · T |
| :---- |

## **2.1 \[O\] Objective**

The Objective component defines the terminal goal of the prompt. It is not a task description. It is a precise statement of the desired outcome, including the beneficiary, the context, and the success condition.

Required elements:

* Primary goal — what must be produced

* Intended recipient or operator — who will use the output

* Success condition — what constitutes a satisfactory result

Objective statements must be written in outcome language, not imperative language. The prompt does not instruct the model to try — it defines what done looks like.

## **2.2 \[P\] Parameters**

The Parameters component defines all input variables, constraints, and configuration settings that govern the prompt's execution. Parameters are the control surface of the prompt — every value that changes the output must be declared here.

Parameter sections must include:

* Labeled input variables with types and acceptable values

* Default values for all optional parameters

* Auto-correction logic for missing or invalid inputs

* Constraint declarations (word limits, format locks, scope boundaries)

Parameters are organized in named sections (A, B, C) when the prompt requires multiple input domains. Each section header identifies the input domain it governs.

## **2.3 \[R\] Results**

The Results component is a precise specification of the deliverable — not a description of effort, but an enumeration of what the operator will receive upon successful execution.

Results declarations must include:

* Output type (report, table, roadmap, checklist, decision matrix, etc.)

* Output structure (sections, headers, depth)

* Format specification (markdown, plain text, JSON, etc.)

* Scope and completeness criteria

## **2.4 \[M\] Method**

The Method component defines the step-by-step execution logic the model must follow to produce the specified result. It is the operational core of the prompt — the process that converts inputs into outputs.

Method requirements:

* Numbered steps, each describing a discrete action

* No ambiguous directives (avoid: 'analyze thoroughly'; use: 'identify the three primary failure modes and rank by severity')

* Decision logic declared explicitly for branching paths

* Verification steps included for quality-critical outputs

## **2.5 \[T\] Tools**

The Tools component identifies the frameworks, reasoning systems, models, or external integrations the prompt invokes. For prompts operating within AI environments, this section declares which capabilities are engaged.

Tools declarations include:

* Reasoning frameworks (chain-of-thought, tree-of-thought, structured reasoning)

* External models or APIs if applicable

* Domain knowledge systems or taxonomies referenced

* Compliance standards or evaluation frameworks applied

# **3\. Metadata Specification**

Every OPRMT™-compliant prompt published to the commercial library must carry a complete metadata record. Metadata is not supplementary documentation — it is a structural requirement. Prompts without complete metadata are non-compliant and ineligible for library publication.

## **3.1 Essential Metadata**

| Field | Definition |
| :---- | :---- |
| Prompt ID | Unique identifier. Format: OPRMT-\[CATEGORY\]-\[NUMBER\]-v\[VERSION\] |
| Title | Descriptive commercial name. Clear, searchable, outcome-focused. |
| Category | Primary taxonomy node (e.g., Market Research, Business Infrastructure, Legal). |
| Subcategory | Secondary taxonomy node within the category. |
| Description | 1–2 sentence summary of what the prompt produces and for whom. |
| Use Case | Specific operational scenario the prompt resolves. |
| Difficulty Level | Beginner / Intermediate / Advanced |
| Tags | Comma-separated searchable keywords. Minimum 5 tags. |

## **3.2 Functional Metadata**

| Field | Definition |
| :---- | :---- |
| Input Requirements | Exact data the operator must provide. Enumerated list. |
| Output Format | Specific format type: report, roadmap, table, bullets, JSON, etc. |
| Estimated Length | Short (under 500 words) / Medium (500–1500) / Long (1500+) |
| Industry | Target industry if domain-specific; 'General' if cross-industry. |
| Role / Department | Primary operator profile (e.g., Marketing Manager, Legal Counsel). |

## **3.3 Quality and Usage Metadata**

| Field | Definition |
| :---- | :---- |
| Popularity / Usage Count | Numeric counter. Default: 0 at publication. |
| Rating | Aggregate operator rating. Default: Not yet rated. |
| Last Updated | ISO date of most recent revision. |
| Version | Semantic version string. Format: v\[MAJOR\].\[MINOR\] |
| Created Date | ISO date of initial publication. |

## **3.4 Enhanced Discovery Metadata**

| Field | Definition |
| :---- | :---- |
| Related Prompts | Internal cross-links to functionally related prompts by Prompt ID. |
| Prerequisites | Knowledge, data, or access required before executing the prompt. |
| Examples | Sample input values and expected output summary. |
| Tips | Best practices, common failure modes, optimization notes. |
| Language | Default: English. Specify if localized. |

## **3.5 Advanced Metadata**

| Field | Definition |
| :---- | :---- |
| Customization Level | Low / Medium / High — degree of variable modification required. |
| Time to Complete | Estimated operator setup time (excluding model execution). |
| Author / Creator | OPRMT™ Engine, or named contributor if applicable. |
| License / Usage Rights | Proprietary — licensed per OPRMT™ commercial terms. |

# **4\. Variable Injection Standard**

OPRMT™ prompts are not static documents. They are parameterized templates designed for reuse across operators, industries, and contexts. The Variable Injection Standard governs how input variables are declared, placed, and enforced across all prompt types.

## **4.1 Universal User Variables**

The following variables are mandatory in every OPRMT™ prompt, regardless of category or complexity:

| Variable | Default Value | Purpose |
| :---- | :---- | :---- |
| \[Brand\_Name\] | Your Brand | Operator or organization identity |
| \[Creator\_Name\] | The Creator | Prompt author or content owner |
| \[Audience\_Type\] | General Audience | Target reader or end user |
| \[Industry\_or\_Niche\] | General Business | Operational domain for context calibration |
| \[Tone\] | Professional | Register and formality of output |
| \[Voice\] | Educator | Persona or perspective of the output |
| \[Reading\_Level\] | General Public | Complexity calibration for output language |
| \[Output\_Length\] | Medium | Short / Medium / Long |
| \[Format\_Type\] | Structured Bullets | Output structure type |
| \[Platform\] | Generic / Cross-platform | Deployment or publication context |
| \[CTA\] | Learn more | Call to action text |
| \[CTA\_Placement\] | End | Position of CTA within output |

## **4.2 Enhancement Variables**

Enhancement variables increase output quality, specificity, and governance control. They are included in all prompts with complexity level Intermediate or Advanced, and in any prompt where the output will be published, distributed, or used in a commercial context.

| Variable | Default Value | Purpose |
| :---- | :---- | :---- |
| \[Expert\_Level\] | Expert | Depth and sophistication of output |
| \[Assumptions\_Allowed\] | Yes | Permit model to fill unstated gaps |
| \[Explain\_Reasoning\] | No | Include rationale alongside output |
| \[Novelty\_Level\] | Medium | Differentiation from generic outputs |
| \[Avoid\_Repetition\] | Yes | Suppress redundant content |
| \[Perspective\] | Strategist | Analytical stance of the output |
| \[Word\_Limit\] | None | Numeric cap on output length |
| \[Emoji\_Allowed\] | No | Permit or prohibit emoji in output |
| \[Hashtag\_Limit\] | 0 | Maximum hashtag count for social content |

## **4.3 Variable Placement Rules**

All variables must appear in three locations within every prompt:

1. Variable Definitions Block — at the top of the prompt, labeled and commented, listing all variables with their defaults.

2. Prompt Body — variables are actively referenced within the \[P\] Parameters and \[M\] Method sections.

3. Metadata Block — all input variables are enumerated under Input Requirements.

## **4.4 Auto-Correction Rules**

The following logic must be enforced by all OPRMT™-compliant execution environments:

* If a variable is missing or empty, apply its declared default value.

* If user input conflicts with declared constraints (e.g., word limit exceeded), revise output to comply.

* If \[Platform\] is specified, adapt formatting and tone to that platform's conventions automatically.

* If \[Audience\_Type\] is vague or absent, infer from \[Industry\_or\_Niche\].

* Never request follow-up clarification unless \[Assumptions\_Allowed\] \= No.

# **5\. Deterministic Compliance Standard (DCS v2.0)**

The Deterministic Compliance Standard defines the criteria against which every OPRMT™ prompt is evaluated for certification. Compliance is not a binary pass/fail — it is a scored assessment that determines certification tier and library publication eligibility.

## **5.1 The Deterministic Compliance Index (DCI™)**

The DCI™ is the primary quality metric for OPRMT™ prompts. It is computed from two sub-scores:

* Structural Integrity (SI) — measures architectural completeness across the five OPRMT™ components and all required metadata fields.

* Execution Fidelity (EF) — measures output consistency, variable compliance, and auto-correction adherence across multiple executions.

DCI Formula:

**DCI \= (SI × 0.60) \+ (EF × 0.40)**

## **5.2 Certification Tiers**

| Tier | DCI Score Range | Publishing Status |
| :---- | :---- | :---- |
| Certified — Gold | 90–100 | Full library publication authorized |
| Certified — Silver | 75–89 | Conditional publication with noted limitations |
| Provisional | 60–74 | Review required before publication |
| Non-Compliant | Below 60 | Publication blocked; revision mandatory |

## **5.3 Structural Integrity Scoring**

Structural Integrity is evaluated across 12 criteria. Each criterion is scored 0–10. The SI score is the weighted average of all 12 criteria scores.

| Criterion | Weight |
| :---- | :---- |
| Objective: clarity and outcome specificity | 10% |
| Parameters: variable completeness and default coverage | 10% |
| Results: output specification accuracy | 10% |
| Method: step completeness and ambiguity score | 10% |
| Tools: framework declaration accuracy | 5% |
| Essential metadata: all required fields present | 10% |
| Functional metadata: complete and accurate | 10% |
| Quality metadata: populated with valid defaults | 8% |
| Discovery metadata: cross-links and examples present | 10% |
| Variable injection: universal variables declared | 9% |
| Auto-correction rules: all four rules declared | 5% |
| System header and footer: exact format compliance | 3% |

## **5.4 SHA-256 Compliance Hashing**

Upon certification, each compliant prompt is assigned a SHA-256 hash of its canonical text. This hash serves as the tamper-evident signature for the prompt version. Any revision invalidates the hash and requires re-certification.

Hash storage format:

* Recorded in the JSON audit artifact for the prompt

* Stored in the GitHub version control record

* Referenced in the Prompt Version Control (PVC) system entry

# **6\. Prompt Version Control (PVC) System**

The PVC system governs the lifecycle of every OPRMT™ prompt from initial publication through deprecation. It is modeled on software semantic versioning and is fully compatible with Git-based version control workflows.

## **6.1 Version Numbering Convention**

All OPRMT™ prompts use two-component semantic versioning:

**v\[MAJOR\].\[MINOR\]**

| Component | Trigger Condition |
| :---- | :---- |
| MAJOR increment | Structural revision to any of the five components, or metadata schema change. |
| MINOR increment | Variable default change, tip addition, tag update, or non-structural text edit. |
| Version lock | Certified Gold prompts. Version increments require re-certification. |
| Initial publication | All prompts begin at v1.0. |

## **6.2 Git Workflow Convention**

The canonical source for all OPRMT™ prompts is the GitHub repository. The following conventions are enforced:

* Each prompt occupies a dedicated directory: /prompts/\[CATEGORY\]/\[PROMPT-ID\]/

* Each directory contains: prompt.md, metadata.json, audit.json

* Commits follow the format: \[PROMPT-ID\] v\[VERSION\] — \[change summary\]

* Tags mark certification events: cert-gold, cert-silver, provisional

* Branches are used for draft revisions; main branch contains only certified content

## **6.3 Deprecation Protocol**

Prompts are deprecated, not deleted. Deprecated prompts remain in the repository with a DEPRECATED flag in metadata and a forwarding reference to their replacement. Deprecated prompts are removed from active library listings but remain accessible via direct ID reference.

# **7\. Prompt Taxonomy**

The OPRMT™ library is organized by a two-level taxonomy: Category and Subcategory. All prompts must be assigned to a valid taxonomy node at publication. New taxonomy nodes require Standards Initiative approval before use.

## **7.1 Primary Category Registry**

| Category Code | Category Name |
| :---- | :---- |
| SMEDIA | Social Media Operations |
| MRS | Market Research System |
| BIZ | Business Infrastructure |
| LEGAL | Legal and Compliance |
| FIN | Financial Operations |
| OPS | Operational Systems |
| HR | Human Resources |
| MKTG | Marketing and Brand |
| TECH | Technical and Engineering |
| EDU | Education and Training |
| EXEC | Executive and Strategy |
| SALES | Sales and Revenue |

## **7.2 Prompt ID Format**

All prompts must carry a unique Prompt ID conforming to the following format:

**OPRMT-\[CATEGORY\]-\[NUMBER\]-v\[VERSION\]**

Example: OPRMT-MRS-001-v1.0 — Market Research System, Prompt 001, Version 1.0

Numbering within each category is sequential and permanent. A number retired with a deprecated prompt is not reused.

# **8\. System Header and Footer Standards**

Every published OPRMT™ prompt must begin with a compliant System Header and end with a compliant System Footer. These elements are non-negotiable structural components and are included in the SI scoring criteria.

## **8.1 Required System Header**

| Header Field | Format |
| :---- | :---- |
| OPRMT™ MASTER PROMPT SYSTEM | Static label |
| Prompt ID | OPRMT-\[CATEGORY\]-\[NUMBER\]-v\[VERSION\] |
| Category | Primary category name |
| Subcategory | Secondary category name |
| Difficulty | Beginner / Intermediate / Advanced |
| Version Control | GitHub (Canonical Source) |

## **8.2 Required System Footer**

| Footer Field | Format |
| :---- | :---- |
| END OF OPRMT™ PROMPT | Static label |
| Category | Primary category name |
| Version Control | GitHub (Canonical) |
| License | Proprietary to OPRMT™ |
| Copyright | © 2026 Michael W. Fleming. All rights reserved. |
| Support | engineering@oprmt.solutions |

# **9\. Output Format Standards**

OPRMT™ prompts produce structured, professional outputs. The following standards govern output formatting across all prompt types:

* Use clear, labeled section headings. No generic headers such as 'Introduction' or 'Conclusion'.

* Numbered steps are used for procedural outputs. Bullets for enumerated items. Tables for comparative data.

* No emojis in default output configuration unless \[Emoji\_Allowed\] \= Yes is explicitly set.

* No marketing language in structural outputs. Tone defaults to professional unless overridden by \[Tone\].

* All outputs assume professional operators as the recipient unless \[Audience\_Type\] specifies otherwise.

* Word counts conform to \[Output\_Length\]: Short \= under 500 words; Medium \= 500–1500; Long \= 1500+.

* Format adheres to \[Format\_Type\]: paragraph, bullets, steps, or table. Mixed formats require explicit declaration in \[R\] Results.

# **10\. Intellectual Property and Licensing**

## **10.1 Ownership**

All OPRMT™ prompts, specifications, taxonomies, scoring systems, and derivative frameworks are proprietary intellectual property of Michael W. Fleming, published under the OPRMT™ Standards Initiative. All rights are reserved.

## **10.2 Licensed Use**

Commercial use of OPRMT™-compliant prompts, frameworks, or library assets requires an active license agreement with the OPRMT™ Standards Initiative. Licensing inquiries are directed to engineering@oprmt.solutions.

## **10.3 Permitted Activities Under License**

* Execution of licensed prompts within licensed operator environments

* Internal distribution of prompt outputs within the licensed organization

* Creation of derivative prompts that comply with this specification, subject to attribution requirements

## **10.4 Prohibited Activities**

* Reproduction or redistribution of OPRMT™ prompt text without an active license

* Publication of OPRMT™ prompts to third-party platforms without written authorization

* Removal of OPRMT™ system headers, footers, metadata, or attribution from any prompt

* Reverse engineering or repackaging of the DCI™ scoring methodology without authorization

# **11\. Compliance Audit Record**

Each OPRMT™ prompt maintains a JSON audit artifact stored alongside the prompt file in the GitHub repository. The audit record documents the certification history, DCI scores, and version lineage for the prompt.

## **11.1 Audit Artifact Schema**

| Field | Type and Definition |
| :---- | :---- |
| prompt\_id | String. Canonical OPRMT Prompt ID. |
| version | String. Semantic version at time of audit. |
| audit\_date | ISO 8601 date of certification evaluation. |
| dci\_score | Numeric. Computed DCI™ score (0–100). |
| si\_score | Numeric. Structural Integrity component score. |
| ef\_score | Numeric. Execution Fidelity component score. |
| certification\_tier | String. Gold / Silver / Provisional / Non-Compliant. |
| sha256\_hash | String. SHA-256 hash of canonical prompt text. |
| auditor | String. OPRMT™ Engine or named auditor. |
| notes | String. Audit findings, exceptions, or revision requirements. |
| prior\_versions | Array. Ordered list of prior version audit records. |

# **12\. Governance and Standards Evolution**

## **12.1 Standards Authority**

The OPRMT™ Standards Initiative holds sole authority over this specification. All amendments, extensions, and deprecations of specification components require formal review and versioned release. This document is Version 1.0 of the OPRMT™ Framework Specification.

## **12.2 Contribution Protocol**

Contributions to the OPRMT™ framework, including proposed new taxonomy nodes, variable additions, or scoring criteria modifications, are submitted to engineering@oprmt.solutions for review. Accepted contributions are attributed in the version changelog.

## **12.3 Specification Versioning**

This specification follows the same semantic versioning convention as individual prompts. Breaking changes to the architecture, metadata schema, or scoring system trigger a MAJOR version increment. Non-breaking additions or clarifications trigger a MINOR increment.

# **Document Control**

| Version | Date | Change Summary |
| :---- | :---- | :---- |
| v1.0 | 2026 | Initial publication. Full specification of five-component architecture, DCS v2.0, PVC system, metadata standard, and variable injection standard. |

OPRMT™ Standards Initiative  |  oprmt.solutions  |  engineering@oprmt.solutions

© 2026 Michael W. Fleming. All rights reserved.
