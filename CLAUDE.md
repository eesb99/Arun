# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

Medical research project investigating treatment options for a 65-year-old patient with metastatic EGFR+ NSCLC (non-small cell lung cancer), 4th line therapy. Key comorbidities: heart failure, renal dysfunction, cytopenias.

## Research Workflow

- Phase-based: track progress in `context/progress.md`
- Session context and cumulative findings in `context/claude.md`
- Final deliverables as timestamped markdown (e.g., `2026-02-01_arun_treatment_recommendations.md`)
- All recommendations must include PubMed IDs or trial NCT numbers for verifiability
- Geographic focus: Southeast Asia (Malaysia, Singapore) for clinical trial feasibility

## MCP Usage

7 domain MCPs configured in `.mcp.json`: cBioPortal, ChEMBL, PubMed, UniProt, Reactome, ClinicalTrials.gov, PubChem. Read-only access only.

- Cross-reference findings across multiple databases before making recommendations
- Always check drug interactions and contraindications against the patient's comorbidities
- When searching clinical trials, filter for Southeast Asia recruitment sites

## Session Protocol

- Start each session by reading `context/claude.md` and `context/progress.md` for continuity
- Update `context/progress.md` after completing any phase milestone
- Update `context/claude.md` with session findings before ending

## File Naming

Deliverables: `YYYY-MM-DD_arun_<description>.md`
