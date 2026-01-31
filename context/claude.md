# Arun Cancer Investigation Project

## Current State
- **Project**: Advanced EGFR+ NSCLC treatment research for patient case
- **Status**: Session 2 complete - Comprehensive treatment recommendations generated
- **Last Updated**: 2026-02-01
- **Repository**: https://github.com/eesb99/Arun (private)

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

---

## Session 2 Summary (2026-02-01)

### Goals
- Execute comprehensive MCP searches across PubMed, ClinicalTrials.gov, ChEMBL, cBioPortal
- Research cardio-safe chemotherapy options (patient has heart failure)
- Research renal-safe chemotherapy options (patient has renal dysfunction)
- Evaluate immunotherapy safety in EGFR-mutant NSCLC
- Find clinical trials in Southeast Asia (Singapore interest confirmed)
- Develop cytopenia management plan (low Hb, PLT, WBC)

### Key Research Findings

**Cardio-Safe Chemotherapy:**
- Carboplatin: Preferred platinum (no significant cardiotoxicity)
- Lazertinib: Cardio-safer alternative to osimertinib (PMID 40919674)
- **AVOID:** Bevacizumab (CHF risk), anthracyclines

**Renal-Safe Chemotherapy:**
- Pemetrexed: **Contraindicated if CrCl <45 mL/min** (PMID 32505078)
- Carboplatin: Dose-adjustable by Calvert formula
- EGFR-TKIs: Generally renal-safe

**Immunotherapy Decision:**
- EGFR-mutant NSCLC has lower ICI efficacy (~10-20% vs 30-40%)
- Pre-existing cardiac dysfunction increases myocarditis risk
- Recommendation: Prefer TKI or chemo alone over chemo-IO

**Clinical Trials Found:**
- 1,271+ trials in Singapore/Malaysia region
- Key recruiting: REZILIENT3 (zipalertinib), Sunvozertinib adjuvant
- Patient confirmed interest in Singapore travel

**Cytopenia Management:**
- G-CSF prophylaxis recommended (2026 AGIHO guidelines, PMID 41570611)
- ESA consideration if Hb <10 g/dL (caution: thrombosis risk)

### Decisions Made
- Prioritize EGFR-TKIs over chemo-IO combinations (cardiac safety + EGFR efficacy)
- Lazertinib as potential cardio-safer alternative to osimertinib
- Pemetrexed eligibility depends on CrCl (need lab values)

### Files Created
1. `2026-02-01_arun_treatment_recommendations.md` - Comprehensive treatment synthesis (378 lines)

### MCP Tools Used
- **PubMed**: 20+ searches (cardiotoxicity, renal safety, G-CSF, EGFR resistance)
- **ClinicalTrials.gov**: Singapore, Malaysia, Thailand, T790M, exon 20 searches
- **ChEMBL**: Osimertinib, carboplatin, pemetrexed, gemcitabine profiles
- **cBioPortal**: 41 lung cancer studies identified, EGFR gene data

### Data Gaps Identified
- Current lab values needed: Hb, PLT, WBC/ANC, Creatinine/eGFR
- Cardiac evaluation needed: LVEF, ECG (QTc)
- EGFR mutation confirmation: T790M vs exon 20ins vs C797S

### Next Steps
- [ ] Obtain current CBC, CMP, GFR from oncologist
- [ ] Request cardiology evaluation (LVEF, ECG)
- [ ] Confirm current EGFR resistance mechanism
- [ ] Calculate carboplatin dose once GFR known
- [ ] Assess trial eligibility against actual lab values
