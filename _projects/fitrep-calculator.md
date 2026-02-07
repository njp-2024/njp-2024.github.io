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

Performance evaluations in the USMC (known as FitReps) require calculating relative value scores and writing structured narrative sections. The process is manual, error-prone, and time-consuming — especially for reporting seniors managing multiple Marines.

There was no lightweight tool to automate the math or help draft narratives consistently.

## Approach

Built a web application using Streamlit that accepts evaluation inputs and computes relative value based on USMC guidelines. Integrated the OpenAI API to generate draft narrative sections from structured inputs, giving users a starting point they could refine.

Chose Streamlit for rapid prototyping and zero-infrastructure deployment. Hosted on GitHub Pages via a static export approach.

## Tradeoffs

- **Streamlit vs. a custom frontend:** Streamlit was faster to build but limits UI customization. Acceptable for an internal tool, but would need rethinking for broader adoption.
- **AI-generated narratives:** Useful as drafts, but require human review. Designed the UI to frame outputs as suggestions, not final products.
- **No authentication:** Kept the tool stateless and open. No user data is stored.

## Outcome

The tool reduces evaluation preparation time and provides a consistent starting point for narrative writing. Demonstrated the value of combining domain knowledge with accessible AI tooling.
