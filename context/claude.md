# Arun Cancer Investigation Project

## Current State
- **Project**: Advanced EGFR+ NSCLC treatment research for patient case
- **Status**: Research complete, MCP tools configured
- **Last Updated**: 2026-01-16

## Patient Case Summary
- **Diagnosis**: Metastatic NSCLC with EGFR exon 20 and 21 mutations
- **Metastases**: Lung -> Liver -> Bone -> Thyroid -> Eye (ocular)
- **Treatment History**: 3 prior chemotherapy regimens + PD-L1 (all initially responded, then progressed)
- **Current**: 4th line therapy
- **Location**: Malaysia/Southeast Asia

## Session 1 Summary (2026-01-16)

### Goals
- Research advanced cancer treatment options for EGFR+ NSCLC patient
- Identify clinical trials accessible in Southeast Asia
- Configure scientific MCPs for cancer investigation
- Develop strategies to improve treatment outcomes

### Key Research Findings

**EGFR Exon 20 Treatments:**
- Amivantamab (bispecific antibody): 40% ORR
- Sunvozertinib (oral TKI): 46-61% ORR, approved July 2025
- Izalontamab brengitecan (ADC): 66% ORR, breakthrough designation

**Brain Metastases Options:**
- Osimertinib: 70-91% CNS ORR (gold standard)
- Furmonertinib: 46% CNS ORR (Asia-developed)
- Zorifertinib: 80%+ CNS ORR (EVEREST trial)

**Treatment Improvement Strategies:**
- Molecular re-testing (ctDNA + tissue NGS) - Critical first step
- Maintain dose intensity >=80-85% (proven survival benefit)
- Early palliative care (+2 months OS)
- Nutritional support (protein 1.0-1.5g/kg/day)
- Exercise program (150 min/week aerobic)

### Decisions Made
- Configure MCPs at project level (not global) - User preference
- Focus on Asia-accessible treatments (Sunvozertinib, Furmonertinib)
- Prioritize clinical trial access through regional centers

### Files Created
1. `.mcp.json` - Project-level MCP configuration (7 MCPs)
2. `~/.claude/plans/gentle-mapping-feather.md` - Comprehensive treatment plan

### MCPs Configured (Project Level)
- cbioportal - Cancer genomics database
- chembl - Drug discovery
- pubmed - Literature search
- uniprot - Protein data
- reactome-server - Pathway analysis
- clinicaltrials - Clinical trial data
- pubchem - Compound data

### Next Steps
- [ ] Confirm exact EGFR mutation type (T790M vs insertion)
- [ ] Request liquid biopsy for resistance mechanisms
- [ ] Contact regional cancer centers for clinical trial access
- [ ] Ophthalmology consult for ocular metastasis
- [ ] Test MCPs after Claude Code reload

## Quick Reference

### Key Contacts (Southeast Asia)
- National Cancer Centre Singapore
- Universiti Malaya Cancer Research Institute
- Asian Thoracic Oncology Group (ATOG)

### Critical Questions for Oncologist
1. Is exon 20 mutation an insertion or T790M?
2. MET amplification status?
3. Clinical trial availability?

### Plan File
`~/.claude/plans/gentle-mapping-feather.md` - Full treatment research
