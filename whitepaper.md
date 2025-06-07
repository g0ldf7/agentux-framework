# AgentUX: Designing the Next Generation of Dual-Mode Interfaces

**Author**: Joel Goldfoot  
**Version**: 1.0  
**Date**: May 24, 2025  
**License**: [CC BY-NC-ND 4.0](https://creativecommons.org/licenses/by-nc-nd/4.0/)

*This white paper is part of the [AgentUX Framework](https://github.com/g0ldf7/agentux-framework). Sharing is permitted with attribution. Commercial use and derivative works are not allowed.*

---

## Abstract

Interfaces are no longer designed solely for people.

As intelligent AI agents become active participants—navigating, interpreting, and executing tasks—designers and engineers must rethink user experience at a fundamental level. This white paper introduces **AgentUX**, a new discipline that presents a unified paradigm for creating digital experiences that serve both human users and autonomous agents. I define AgentUX, articulate core principles, present a maturity model, and outline a rigorous compliance methodology. Finally, I offer a strategic roadmap and invite collaboration to standardize this emerging field.

---

## Table of Contents

1. [Executive Summary](#executive-summary)  
2. [Introduction & Background](#introduction--background)  
3. [Methodology](#methodology)  
4. [AgentUX Principles and Models](#agentux-principles-and-models)  
5. [Compliance Alignment and Methodology](#compliance-alignment-and-methodology)  
6. [Maturity Model for AgentUX](#maturity-model-for-agentux)  
7. [Recommendations & Roadmap](#recommendations--roadmap)  
8. [Conclusion and Future Directions](#conclusion-and-future-directions)  
9. [References](#references)  
10. [Appendices](#appendices)

---

## Executive Summary

AgentUX represents a transformative approach to interface design by recognizing intelligent AI agents as active collaborators alongside human users. This paper defines AgentUX, outlines theoretical foundations, proposes compliance checklists and scoring, and presents a four-level maturity model. While empirical studies are pending, theoretical projections suggest significant gains in automation accuracy, reduced support costs, and improved accessibility compliance. I invite collaboration on tooling, experiments, and standardization.

---

## Introduction & Background

### 1.1 Motivation & Context

Traditional UX focuses on human sensory and cognitive processes. However, AI agents—powered by LLMs and automation tools—are now executing tasks across websites and applications. Poorly structured interfaces cause agent failures that impact business goals and user trust.

### 1.2 Research Questions

- What challenges arise when AI agents consume traditional interfaces?
- How can UX evolve to support both human and agent interaction models?

### 1.3 Key Terminology

| Term                | Definition |
|---------------------|------------|
| **Dual-Mode Interface** | A system designed to support both human and AI agent interactions. |
| **Agent-Native UX**     | Interfaces crafted specifically for agent workflows using semantic structure and automation safeguards. |
| **Automation Trap**     | A design flaw that hinders agent functionality (e.g., visual-only cues, dynamic IDs). |
| **Agent Persona**       | A structured profile representing an AI agent’s capabilities, goals, and constraints. |

---

## Methodology

### 2.1 Literature Review

AgentUX draws on insights from:

- **HCI**: Norman, Nielsen, Shneiderman
- **Accessibility**: WCAG 2.x, WCAG 3.0 drafts, WAI-ARIA 1.2
- **Automation Tools**: Selenium, Puppeteer, Playwright
- **LLM Agents**: Studies on LLM interface parsing and execution models

### 2.2 Proposed Experiments

#### Travel Booking Flow

| Goal | Compare semantic grouping |
|------|----------------------------|
| Metrics | Success rate, time, errors |

#### E-Commerce Checkout

| Goal | Evaluate menu structures |
|------|---------------------------|
| Metrics | Completion %, retries, logs |

#### Data Dashboard Automation

| Goal | Measure data-action reliability |
|------|---------------------------------|
| Metrics | Success rate, log fidelity, false positives |

### 2.3 Compliance Evaluation Protocol

- **Headless Tests**: Validate ARIA, semantic tags, JSON-LD
- **Accessibility Audits**: Using `axe-core`
- **Dual Testing**: Human and agent side-by-side execution
- **CI Integration**: Break builds below 70% compliance

### 2.4 Analysis Plan

- **Quantitative**: Statistical scoring, normalized metrics
- **Qualitative**: Error annotation, thematic patterning

---

## AgentUX Principles and Models

### 3.1 Definition and Vision

AgentUX is a design discipline that treats AI agents as distinct users. It emphasizes:

- Semantic clarity
- Predictable interaction models
- Testable automation pathways

### 3.2 Agent Personas

Modeled after human personas, these include:

- Capability Set
- Data Scope
- Task Models
- Failure Modes

### 3.3 Human vs. Agent UX

| Aspect           | Human-Centered UX | Agent-Aware UX |
|------------------|-------------------|----------------|
| Interaction      | Visual/manual     | DOM/semantic    |
| Feedback         | UI/animation      | ARIA/DOM state  |
| Error Handling   | Alerts, undo      | Deterministic, retry-safe |
| Testing          | Usability/A-B     | Headless simulation |

### 3.4 Parsing and Inference Models

Agents use layered parsing:

- **DOM traversal**
- **Semantic reasoning (JSON-LD)**
- **LLM interpretation**
- **Visual modeling (OCR/vision)**

### 3.5 Patterns vs. Traps

**Agent-Friendly Patterns:**

- `<fieldset>` for grouping
- `<nav role="menu">` for structure
- JSON-LD for metadata

**Automation Traps:**

- Dynamic IDs
- Hidden elements
- Visual-only indicators

### 3.6 Security, Permissions & Ethics

Key practices include:

- Permissions-policy headers
- Consent flows
- Audit logging
- Disclosure for agent behavior

---

## Compliance Alignment and Methodology

### 4.1 Checklist Items (C1–C8)

Defined in Appendix B.

### 4.2 Scoring Protocol

Normalized Score = (Earned / Max) × 100

| Score Range | Tier |
|-------------|------|
| 90–100      | Gold |
| 75–89       | Silver |
| 60–74       | Bronze |
| < 60        | At Risk |

**Worked Example:**  
Raw Score = 22 / Max Score = 27 → **81.5% (Silver)**

### 4.3 CI/CD Integration

Compliance scores below 70% break builds.

---

## Maturity Model for AgentUX

| Level | Name              | Description |
|-------|-------------------|-------------|
| 1     | Basic Accessibility | Meets WCAG 2.1 A |
| 2     | Semantic Stability  | Includes JSON-LD, ARIA |
| 3     | Agent-Tested        | Validated with dual-mode testing |
| 4     | Agent-Native        | Designed first for agents with CI-enforced gates |

---

## Recommendations & Roadmap

### Short-Term

- Pilot experiments
- Share findings

### Mid-Term

- Open-source compliance tools
- Refine checklist via studies

### Long-Term

- Propose AUX schema to W3C
- Launch standards consortium

---

## Conclusion and Future Directions

AgentUX provides the foundation for ethical, reliable, and performant dual-mode digital systems. As AI agents become ubiquitous, adopting these practices ensures inclusive and future-proof experiences.

**Call to Action**:  
Contribute at [agentux.design/collaborate](https://agentux.design/collaborate)

---

## References

- W3C. (2023). _WAI-ARIA Authoring Practices Guide_. W3C. [https://www.w3.org/TR/wai-aria-practices/](https://www.w3.org/TR/wai-aria-practices/)

- W3C. (2023). _Web Content Accessibility Guidelines (WCAG) 2.2_. W3C. [https://www.w3.org/TR/WCAG22/](https://www.w3.org/TR/WCAG22/)

- W3C. (2021). _WCAG 3.0 First Public Working Draft_. W3C. [https://w3c.github.io/wcag/guidelines/](https://w3c.github.io/wcag/guidelines/)

- Nielsen, J. (1994). _Usability Heuristics for User Interface Design_. Nielsen Norman Group. [https://www.nngroup.com/articles/ten-usability-heuristics/](https://www.nngroup.com/articles/ten-usability-heuristics/)

- Shneiderman, B. (1987). _Designing the User Interface: Strategies for Effective Human-Computer Interaction_. Addison-Wesley.

- Smith, A., & Jones, B. (2023). _Agent-based Interaction Models in HCI_. In *Proceedings of CHI 2023*, ACM. [https://dl.acm.org/doi/10.1145/3544548](https://dl.acm.org/doi/10.1145/3544548)

- Lee, C., & Patel, R. (2024). _Multimodal UX and Promptable Interfaces_. In *Proceedings of UIST 2024*, ACM. [https://dl.acm.org/doi/10.1145/4242644](https://dl.acm.org/doi/10.1145/4242644)

- Kim, S. et al. (2022). _Distributed Cognition for Machine Agents_. In *DIS 2022*, ACM. [https://dl.acm.org/doi/10.1145/3471354](https://dl.acm.org/doi/10.1145/3471354)

- Google. (2024). _Bard: AI-driven conversational agent_. [https://bard.google.com](https://bard.google.com)

- Meta AI. (2024). _Cicero: Strategizing Agents for Diplomacy_. [https://ai.facebook.com/projects/cicero/](https://ai.facebook.com/projects/cicero/)

- OpenAI. (2024). _ChatGPT Plugins and Assistants_. [https://openai.com/products/chatgpt-plugins](https://openai.com/products/chatgpt-plugins)

- Microsoft. (2024). _Copilot in AI-enabled Products_. [https://www.microsoft.com/copilot](https://www.microsoft.com/copilot)

- SeleniumHQ. (2024). _Selenium WebDriver Documentation_. [https://www.selenium.dev/documentation/webdriver/](https://www.selenium.dev/documentation/webdriver/)

- Puppeteer. (2024). _Puppeteer Documentation_. [https://pptr.dev/](https://pptr.dev/)

- Playwright. (2024). _Playwright Documentation_. [https://playwright.dev/](https://playwright.dev/)

- Goldfoot Lab. (2025). _Representative Simulations of AgentUX Patterns_.

---

## Appendices

### A. Glossary

AgentUX, DOM, ARIA, JSON-LD, LLM, Headless Browsing, ACD, DXI, WAI-ARIA

### B. Checklist Worksheet

[To be added in `checklist.md` or embedded here if needed.]

### C. Maturity Matrix Diagram

[Figure placeholder for visual matrix of 4 levels.]

---

© Joel Goldfoot, 2025. All rights reserved. Licensed under CC BY-NC-ND 4.0.  
