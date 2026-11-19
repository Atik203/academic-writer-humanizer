# Academic Writer & Humanizer

[![Turnitin Benchmark](https://img.shields.io/badge/Turnitin%20AI%20Detection-0%25%20Verified-brightgreen?style=flat-square)](writing-support/VOICE_PROFILE.md)
[![Self-Tests](https://img.shields.io/badge/Self--Tests-46%20Passing-success?style=flat-square)](evals/run_selftest.sh)
[![Elsevier CAS Layout](https://img.shields.io/badge/LaTeX-cas--sc%20Ready-orange?style=flat-square)](templates/paper_template.tex)
[![Python](https://img.shields.io/badge/Python-3.8%2B%20(Stdlib)-blue?style=flat-square)](scripts/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=flat-square)](LICENSE)

**An authentic, evidence-grounded research-writing and humanization skill for peer-reviewed papers, theses, and LaTeX manuscripts — calibrated to 0% Turnitin AI detection.**

Standard AI coding assistants produce flat, formulaic, and highly predictable prose. Commercial AI writing detectors (Turnitin, GPTZero, CopyLeaks) flag these drafts due to uniform sentence rhythms, robotic connectors (*"Furthermore"*, *"In conclusion"*), generic filler frames (*"plays a crucial role"*, *"in today's rapidly evolving landscape"*), and fragmented 3-line micro-paragraphs.

**Academic Writer & Humanizer** eliminates these machine signatures through **deep linguistic restructuring and authentic academic voice calibration** — without resorting to deceptive tricks, character-swapping, or ungrammatical filler that damages academic credibility.

---

## Key Highlights

- **Turnitin 0% Calibrated Baseline:** Calibrated against empirical, 0% AI-detected journal papers ([`writing-support/VOICE_PROFILE.md`](writing-support/VOICE_PROFILE.md)). Employs natural sentence length variance ($\sigma \approx 10.8$ words, span 5–49 words) and substantive, cohesive paragraphs ($150–250+$ words).
- **Elsevier `cas-sc` Starter Template:** Complete, publication-ready LaTeX starter template ([`templates/paper_template.tex`](templates/paper_template.tex)) supporting Method-focused, Dataset-focused, and Mixed (Method + Dataset) architectures.
- **5 Structural Evasion & Humanization Principles:**
  1. *PDTB 2.0 Discourse Connector Rotation:* Dynamic variation across causal, contrastive, and conditional transitions; zero robotic transitions (*Furthermore*, *In conclusion*).
  2. *Syntactic Tree Inversion:* Diverse clausal rhythm (fronted adverbial clauses, participial leads, topicalized prepositional phrases).
  3. *Determiner & Possessive Anti-Repetition:* Eliminates list-like, monotonous sentence runs (*"The... The... This..."*).
  4. *5-Gram Cliché Shattering:* Systematic elimination of dead giveaways (*"tapestry"*, *"delve"*, *"testament"*, *"beacon"*, *"pivotal"*, *"paves the way"*).
  5. *Risk-Driven Citation Shielding:* Tight empirical anchoring of all declarative technical claims directly to primary sources.
- **Locked 6-Section Standard:** Exactly 6 numbered main sections as standard (Intro $\rightarrow$ Conventional/Corpus $\rightarrow$ Proposed Method $\rightarrow$ Experiments $\rightarrow$ Results $\rightarrow$ Conclusion), with 4–6 core thematic subsections max (strictly avoiding 5.1–5.10 sprawl).
- **Formal Mathematical & Visual Standards:** Display equations followed immediately by unindented, lowercase `where $x$ denotes...` (never informal `here a = ...`). High-resolution figures ($600+$ DPI, $\ge 8\,\text{pt}$ typography) with concise captions ($\le 35$ words).
- **Automated Diagnostic Suite:** Includes standard-library Python linter ([`scripts/pattern_scan.py`](scripts/pattern_scan.py)) checking for informal variables, micro-paragraphs, overlong captions, subsection sprawl, robotic openers, and flat cadence.
- **Universal Multi-Agent Compatibility:** Native configurations for **OpenCode**, **Claude Code**, **Codex**, **Cline**, **Roo Code**, **Cursor**, **GitHub Copilot**, and **Gemini CLI**.

---

## Repository Architecture

```text
academic-writer-humanizer/
├── SKILL.md                          # Main skill instructions and priority routing
├── templates/
│   ├── paper_template.tex            # Elsevier cas-sc journal starter template
│   ├── voice-profile.md              # Turnitin 0% calibrated voice profile template
│   ├── project-brief.md              # Project evidence inventory template
│   ├── claim-evidence-map.md         # Source-to-claim audit map
│   └── ai-use-ledger.md              # Transparent AI disclosure ledger
├── writing-support/
│   └── VOICE_PROFILE.md              # Reference calibration from 0% Turnitin paper
├── docs/
│   ├── writing-guide.md              # Locked G0-G15 supervisor guidelines + fast-path
│   ├── prompt.md                     # Detailed prose, voice, and quality specs + fast-path
│   ├── clarity-playbook.md           # Ambiguity reduction and information flow
│   ├── detector-awareness.md         # Sourced Turnitin & detector mechanics
│   ├── detector-log.md               # Empirical detector behavior log
│   ├── voice-calibration.md          # Voice calibration instructions
│   └── integration-guide.md          # Tool-by-tool setup documentation
├── scripts/
│   ├── pattern_scan.py               # Style, cliché, and structure linter
│   ├── metric_consistency.py         # CSV vs. prose/LaTeX table consistency audit
│   ├── project_scan.py               # Fast, secure project inventory utility
│   └── integrity_check.py            # AST-level LaTeX editing integrity verifier
├── evals/
│   ├── run_selftest.sh               # 46-test regression test suite
│   └── fixtures/                     # Test fixtures for linters and checkers
└── integrations/                     # Pre-configured agent configs (OpenCode, Claude, etc.)
```

---

## 5 Core Structural Humanization Principles

Rather than corrupting academic grammar with arbitrary synonyms or deceptive zero-width characters, this skill applies five empirical principles derived from authentic peer-reviewed prose:

```
┌────────────────────────────────────────────────────────────────────────┐
│                   5 STRUCTURAL HUMANIZATION PRINCIPLES                  │
├───────────────────────────────┬────────────────────────────────────────┤
│ 1. PDTB 2.0 Connector Rotation│ Causal, contrastive & condition shifts;│
│                               │ purges "Furthermore", "In conclusion"  │
├───────────────────────────────┼────────────────────────────────────────┤
│ 2. Syntactic Tree Inversion   │ Left-branching clauses, fronted PPs,   │
│                               │ broken subject-verb-object monotony    │
├───────────────────────────────┼────────────────────────────────────────┤
│ 3. Determiner Anti-Monotony   │ Prevents consecutive "The... The...    │
│                               │ This..." runs (>50% trigger threshold) │
├───────────────────────────────┼────────────────────────────────────────┤
│ 4. 5-Gram Cliché Shattering   │ Purges "tapestry", "delve", "testament"│
│                               │ "crucial role", "paves the way", etc.  │
├───────────────────────────────┼────────────────────────────────────────┤
│ 5. Citation Shielding         │ Immediate primary source anchoring on  │
│                               │ high-risk empirical & technical claims │
└───────────────────────────────┴────────────────────────────────────────┘
```

---

## Manuscript Structure & Writing Standards

### 1. Locked 6-Section Standard Architecture
Manuscripts are structured into **exactly 6 main numbered sections** as standard (consult author before creating more):
1. **Introduction:** Real-world domain grounding (3–4 citations in P1), prior limitation analysis (5–6 studies reviewed in P2), proposed mechanism & headline contributions.
2. **Conventional Method / Corpus Construction:**
   * *Method papers:* Mathematical preliminaries & conventional baseline formulation.
   * *Dataset papers:* Corpus provenance, annotation protocol, inter-annotator agreement.
   * *Mixed papers:* Task formulation & dataset characteristics.
3. **Proposed Method:** Architecture workflow, mathematical formulation, and operational algorithms (`algorithm` / `algorithmic`).
4. **Experiments:** Compute environment, datasets summary table, baseline protocols, and **mandatory formal Evaluation Metrics** (complete equations for $F_1$, AUROC, ECE, etc.).
5. **Results & Discussion:** Test set benchmark comparison, ablation study, calibration under shift, **rigorous statistical significance testing** (McNemar, bootstrap), and error analysis.
6. **Conclusion:** **Strictly one cohesive single paragraph** (120–160 words) summarizing the problem, proposed mechanism, concrete quantitative gains, and boundary conditions. Zero generic meta-fluff.
*(Followed by unnumbered Declarations, Acknowledgements, and References)*.

### 2. Core Subsections Only (No Sprawl)
Limit each section to **4–6 core thematic subsections max**. Consolidate minor points into cohesive prose paragraphs instead of fragmenting into sprawling heading trees (e.g., strictly avoid 4.1–4.8 or 5.1–5.10).

### 3. Paragraph Cohesion (No Micro-Paragraphs)
Never write fragmented 3–5 line stub paragraphs. Consolidate context, mechanics, and empirical implications into unified, substantive paragraphs (**150–250+ words**, 8–18 lines).

### 4. Mathematical Equation Rigor
Every display equation must be followed immediately by an unindented, lowercase `where $x$ denotes...` sentence defining newly introduced variables. Never write informal definitions such as `"here a = ..."` or `"here, W is ..."`.

### 5. Figure & Visual Quality
* Render all figures and infographics at **600+ DPI** (vector PDF preferred, or high-res PNG/TIFF).
* Typography within charts, legends, and diagrams must be legible ($\ge 8\,\text{pt}$).
* Captions must be concise (1–2 sentences, $\le 35$ words). Reserve all detailed interpretation and statistical takeaways for the body text.

---

## Quickstart: Using the Starter Template

The template at [`templates/paper_template.tex`](templates/paper_template.tex) provides the Elsevier CAS single-column layout with built-in float controls, tight caption spacing, and author blocks:

```bash
# 1. Copy the starter template into your paper workspace
cp templates/paper_template.tex my_paper/main.tex

# 2. Compile with pdflatex or latexmk
latexmk -pdf my_paper/main.tex
```

Toggle the commented section headers inside `main.tex` to match your paper type:
* **Variant A:** Method-Focused Paper
* **Variant B:** Dataset-Focused Paper
* **Variant C:** Mixed (Method + Dataset) Paper

---

## Diagnostic Tooling

Run the bundled diagnostic scanner on any LaTeX or Markdown file:

```bash
# Diagnostic scan for robotic phrases, cadence, micro-paragraphs, and informal math
python scripts/pattern_scan.py my_paper/main.tex

# JSON output mode for automated CI/CD
python scripts/pattern_scan.py my_paper/main.tex --json
```

Audit metric consistency between experimental CSVs and LaTeX tables/prose:

```bash
python scripts/metric_consistency.py --root my_project/ --manifest my_project/metric-audit.csv
```

Verify that an automated edit did not corrupt equations, citations, or numbers:

```bash
python scripts/integrity_check.py original.tex edited.tex
```

---

## Installation & Integration Guide

### OpenCode

Install globally into OpenCode:

```bash
# Linux / macOS
cp -r . ~/.config/opencode/skills/academic-writer-humanizer/
cp integrations/opencode/commands/academic-writer-humanizer.md ~/.config/opencode/commands/

# Windows PowerShell
robocopy . "$HOME\.config\opencode\skills\academic-writer-humanizer" /MIR /XD .git __pycache__ node_modules
Copy-Item integrations\opencode\commands\academic-writer-humanizer.md "$HOME\.config\opencode\commands\"
```

**Invoke in OpenCode:**
* Mention the skill: `@academic-writer-humanizer` (or `@academic-student-writer`)
* Or use the slash command: `/academic-writer-humanizer`

### Other AI Coding Agents

| Tool | Project Install | Personal / Global Install | Invocation |
|---|---|---|---|
| **Claude Code** | `.claude/skills/academic-writer-humanizer/` | `~/.claude/skills/academic-writer-humanizer/` | `/academic-writer-humanizer` |
| **Codex** | `.agents/skills/academic-writer-humanizer/` | `~/.agents/skills/academic-writer-humanizer/` | `$academic-writer-humanizer` |
| **Cline** | `.cline/skills/academic-writer-humanizer/` | `~/.cline/skills/academic-writer-humanizer/` | Skills menu or `/academic-writer-humanizer` |
| **Roo Code** | `.roo/skills/academic-writer-humanizer/` | `~/.roo/skills/academic-writer-humanizer/` | `/academic-writer-humanizer` |
| **Cursor** | `.agents/skills/academic-writer-humanizer/` | User Rules + skill path | Copy `integrations/academic-writer.mdc` to `.cursor/rules/` |
| **GitHub Copilot** | `.agents/skills/academic-writer-humanizer/` | Copilot custom instructions | Copy `integrations/copilot-instructions.md` to `.github/` |
| **Gemini CLI** | Skill in readable directory | `~/.gemini/GEMINI.md` | Copy `integrations/GEMINI.md` to project root |

See [`docs/integration-guide.md`](docs/integration-guide.md) for detailed configuration options.

---

## Operating Modes

When invoking the skill, specify the operational mode:

| Mode | Purpose | Description |
|---|---|---|
| **Mode 0** | **Understand** | Ingests project materials (code, data, results, drafts) and outputs `PROJECT_BRIEF.md` and `VOICE_PROFILE.md`. No writing yet. |
| **Mode 1** | **Edit & Polish** | Refines supplied text for flow, vocabulary, and structure while preserving exact mathematical meaning, numbers, and claim strength. |
| **Mode 2** | **Draft from Evidence** | Generates new manuscript sections directly from verified project data, logs, and notes. Flags any missing values with placeholders. |
| **Mode 3** | **Repair Clarity** | Dissects dense or confusing prose, restructuring argument flow according to the Clarity Playbook. |
| **Mode 4** | **Audit** | Audits the manuscript against the G0–G15 guidelines, identifying evidence gaps, metric discrepancies, or stylistic violations by severity. |

---

## Testing & Verification

Run the comprehensive 46-test regression test suite:

```bash
bash evals/run_selftest.sh
```

All 46 automated tests verify:
- LaTeX edit integrity checking
- Pattern scanner detection of clichés, micro-paragraphs, informal variables, overlong captions, and subsection sprawl
- CSV-to-LaTeX metric audit consistency
- Project inventory privacy and symlink safety
- Sourced Turnitin detector behavior compliance

---

## Research Integrity & Ethical Stance

**Academic Writer & Humanizer is designed to assist legitimate academic researchers in communicating their work clearly, rigorously, and naturally.**

- **Zero Invention:** It never invents data, p-values, benchmarks, or citations. Missing evidence is flagged with explicit placeholders (`[METRIC NEEDED]`).
- **Zero Deception:** It does not use zero-width spaces, character homoglyphs, or intentional typos to fool detectors.
- **Evidence Over Fluency:** A grammatically smooth sentence is rejected if it overclaims or contradicts project findings.
- **Transparent Disclosure:** Includes [`templates/ai-use-ledger.md`](templates/ai-use-ledger.md) to facilitate transparent disclosure in compliance with institutional and publisher AI policies (IEEE, ACM, Elsevier, Springer).

---

## Citation

If you use this repository in your academic research or workflow, please cite:

```bibtex
@software{academic_writer_humanizer_2026,
  author    = {Rahaman, Md. Atikur and contributors},
  title     = {Academic Writer \& Humanizer: Authentic Research Writing and Humanization for Academic Manuscripts},
  version   = {3.2.0},
  year      = {2026},
  url       = {https://github.com/Atik203/academic-writer-humanizer}
}
```

---

## License

This project is licensed under the [MIT License](LICENSE).
