# Social Isolation and Ambition

**Independent research project** • Alexander Anikeev • 2026

This repository contains the manuscript, anonymized data, and reproducibility script for a two-wave study on the relationship between school peer ostracism and goal abandonment in high-achieving adolescents.

## Abstract (short version)

Across two independent samples (Wave 1, N = 82, CIS-based Co-founder ecosystem; Wave 2, N = 35, international communities), we observe a strong positive correlation between school ostracism and frequency of thoughts about abandoning one's startup or key life goal (Wave 1 r = 0.61; Wave 2 r = 0.62; pooled N = 117). A formal Baron-Kenny mediation analysis supports full mediation through school burnout (Sobel z = 3.23, p = 0.001; 73% of total effect mediated). The buffering role of belonging to a project-identity-aligned community is supported in Wave 1 (r = −0.43, p < 0.01) and partially supported in Wave 2 (r = −0.37, p = 0.07).

## Contents

| File | Description |
|---|---|
| `Social_Isolation_Ambition.pdf` | Full manuscript (v6, June 2026) |
| `wave2_anonymous.csv` | Wave 2 anonymized data (N = 35, post-exclusion) |
| `analysis.py` | Python script reproducing all reported statistics |
| `survey_questions.md` | Full text of the questionnaire used in Wave 2 |

## Reproducing the analysis

```bash
pip install pandas numpy scipy
python analysis.py
```

Expected output matches values in Sections 3.2, 5.1, 5.2.1, 5.5, and Appendix B of the manuscript.

## Data anonymization

The public CSV contains aggregated scale scores rather than raw item-level responses, and country has been coarsened to one of five regions (USA, EU, Asia, CIS, AU/NZ, Other) to prevent re-identification of participants from countries with cell sizes below five. Original raw data is retained privately for internal verification. No identifying information (names, IP addresses, email, exact location) was ever collected; participation was anonymous and voluntary via a Google Form with no authentication and no email collection.

## Conflict of interest

The first author is a co-founder of the Co-founder ecosystem from which Wave 1 was recruited. Wave 2 was deliberately recruited from communities entirely outside this ecosystem (Hack Club, ApplyingToCollege, Indie Hackers, Reddit r/Entrepreneur) and provides an independent check on the central findings. This is also disclosed in the manuscript abstract and Sections 4.3 and 6.6.

## Limitations

This is an independent student research project. It did not undergo formal institutional ethics review, used custom item sets modeled on (rather than identical to) validated parent instruments, and is cross-sectional rather than longitudinal. These limitations are discussed in Section 6.6 of the manuscript. Results should be read as preliminary correlational evidence motivating future longitudinal work, not as definitive causal claims.

## Citation

If you reference this work:

> Anikeev, A. (2026). *Social isolation and ambition: A two-wave correlational study of school ostracism and goal abandonment in high-achieving adolescents.* Independent research preprint. 

## Contact

For questions about the data or analysis: open an issue in this repository.
