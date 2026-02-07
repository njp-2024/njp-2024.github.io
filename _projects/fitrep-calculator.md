---
title: FitRep Calculator
description: A Python/Streamlit app that calculates relative value and generates AI-assisted narratives for USMC performance evaluations.
tech:
  - Python
  - Streamlit
  - OpenAI API
repo: "https://github.com/njp-2024/fitrep-calculator"
live: "https://njp-2024.github.io/fitrep-calculator/"
order: 1
---

## Problem

Performance evaluations in the U.S. Marine Corps require both quantitative scoring and tightly structured narrative assessments. The workflow combines rule-based calculations with subjective written justification, making it time-consuming and error-prone, particularly for evaluators responsible for multiple reports.

At the time, no lightweight tool existed to display the quantitative scores or help standardize narrative drafting while preserving human judgment.

---

## Approach

I built a web application that accepts structured evaluation inputs and computes relative value scores according to published guidelines. The application then uses a large language model to generate draft narrative sections aligned with those inputs, providing users with a consistent starting point rather than a finished product.

The system separates deterministic logic (scoring and validation) from probabilistic output (narrative drafting), ensuring transparency and user control. Streamlit was selected to enable rapid iteration, low operational overhead, and easy access for non-technical users. The application integrates the OpenAI API behind a controlled interface, abstracting prompt construction while keeping the underlying inputs explicit.

In addition to its operational purpose, the project serves as a controlled environment for evaluating different LLM sizes, deployment approaches, and interaction patterns (browser-based tools vs. API-driven integration).

---

## Tradeoffs

- **Rapid framework vs. custom frontend:** Streamlit enabled fast delivery and experimentation but limits UI customization. This was acceptable for an internal decision-support tool and helped inform what a future production-grade implementation would require.
- **AI abstraction vs. cost transparency:** Centralizing AI interactions simplifies the user experience but introduces API costs. To explore this tradeoff, the tool also exposes structured prompts that can be used directly in browser-based LLM interfaces.
- **Stateless design vs. personalization:** The application intentionally avoids authentication and persistent storage. This reduces complexity and risk while avoiding duplication of data already managed by existing enterprise systems.

---

## Outcome

The tool is currently in active testing and use, reducing manual calculation errors and improving consistency in narrative drafting. More broadly, it has become a practical reference point for discussing AI integration patterns, tradeoffs, and governance within an operational setting.

The project remains iterative by design, with future work focused on usability refinement, evaluation of alternative models, and potential pathways to a more integrated production solution.