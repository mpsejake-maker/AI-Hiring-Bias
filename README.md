# AI-Hiring-Bias
The catalog organizes data related to recruitment processes and bias analysis in hiring practices. It contains schemas for candidate profiles, interview feedback, hiring metrics, and bias assessment reports. Use this catalog for analyzing recruitment trends, assessing bias in hiring, and improving diversity initiatives.

https://dbc-a73524c0-9fa2.cloud.databricks.com/dashboardsv3/01f1627a9d44184b9059115e34d4b6b0/published?o=7474656807876502&f_a367028b%7Emerit_gap_analysis=%257B%2522columns%2522%253A%255B%2522x%2522%255D%252C%2522rows%2522%253A%255B%255B%2522Non-Binary%2522%255D%255D%257D 

**Objective of the AI Hiring Bias Dataset**

The ai_recruitment_biasness.ai_bias.ai_hiring_bias_dataset is designed to detect and analyze bias in AI-powered recruitment processes. Specifically, it aims to:

**Primary Goals:**
**1. Identify Hiring Bias Patterns**

Detect disparate treatment across demographic groups (gender, age, education, university prestige)
Measure adverse impact using compliance standards (4/5ths rule)
Reveal whether hiring decisions correlate with candidate merit or demographic attributes

**2. Evaluate AI System Fairness**

Assess whether AI resume screening (ai_resume_score) and bias detection systems (ai_bias_score) perpetuate or mitigate bias
Compare AI-generated scores against objective assessments (technical, coding, aptitude tests)
Determine if AI tools introduce systematic discrimination

**3. Support Evidence-Based Decision Making**

Provide quantitative evidence for legal compliance reviews
Enable intersectional analysis (e.g., gender × university tier × experience level)
Guide remediation strategies with data-driven insights

**Key Dataset Features:**
Demographics: age, gender, education_level, university_tier Qualifications: years_experience, project_count, certifications_count, github_activity_score Assessments: technical_skill_score, communication_score, aptitude_test_score, coding_test_score AI Metrics: ai_resume_score, ai_bias_score Outcome: hired (binary: 1 = hired, 0 = not hired)

**Use Cases:**
HR Compliance Audits — Verify adherence to equal employment laws
Process Improvement — Identify where bias enters the hiring funnel
AI Tool Validation — Test whether AI recruitment tools are fair and accurate
Diversity Analytics — Track representation gaps and hiring rate disparities
The dataset enables organizations to answer critical questions like: "Do equally qualified candidates from different demographics have equal hiring outcomes?" and "Are AI screening tools helping or harming fairness?"
____________________________________________________________________________________________________________________________________________________________________________
**Sample Questions for AI Recruitment Bias Dataset**

**1. Gender & Merit Questions**

"Are male candidates with lower technical scores being hired over female candidates with higher scores?"
"What is the hiring rate gap between genders when controlling for identical assessment score ranges (e.g., 80-90 technical score)?"

**2. Educational Bias Questions**

"How many Tier 3 university candidates were rejected despite having higher assessment scores than hired Tier 1 candidates?"
"What is the cost difference in expected salary between Tier 1 and Tier 3 candidates with equivalent qualifications?"

**3. Experience Discrimination Questions**

"For candidates with 10+ years experience vs 0-2 years, what is the average assessment score difference, and does it justify the 3.4x hiring rate gap?"
"Are we rejecting entry-level candidates with Masters degrees in favor of experienced candidates with only Bachelor's degrees?"

**4. Intersectional Analysis Questions**

"Which demographic combination faces the most severe bias - female + Tier 3 university, or non-binary + under 25 age?"
"Do female candidates from Tier 1 universities get hired at the same rate as male candidates from Tier 2 universities?"

**5. AI System Audit Questions**

"Is the AI resume score (ai_resume_score) correlated with actual hiring decisions, or are human reviewers overriding AI recommendations?"
"Do candidates with high AI bias scores (ai_bias_score) actually experience lower hiring rates - i.e., is our bias detection system accurate?"

**6. Qualification vs Outcome Questions**

"Among candidates with 5+ projects, 3+ certifications, and 70+ GitHub scores, what are the hiring rates by gender and university tier?"
"Are candidates with employment gaps being penalized differently based on their gender or age?"

**7. Compliance & Risk Questions**

"Which demographic groups fail the 4/5ths adverse impact rule, and what is our legal exposure?"
"If we applied a purely merit-based cutoff (e.g., technical score >75), how would our hired cohort demographics change?"

**8. Financial Impact Questions**

"What is the average expected salary of rejected candidates vs hired candidates with equivalent assessment scores?"
"Are we overpaying for experienced hires when equally skilled entry-level candidates are available at lower salary expectations?"

**9. Pipeline Analysis Questions**

"At what stage of the hiring funnel (resume screening, technical assessment, final decision) does the biggest demographic disparity occur?"
"How many candidates passed all assessment thresholds but were still not hired - and what are their demographic profiles?"

**10. Intervention Testing Questions**

"If we implemented blind resume review (hiding name, university, age), what would be the projected change in hiring rates by demographics?"
"What minimum representation targets (% female, % Tier 2/3, % entry-level) would we need to achieve statistical parity based on our applicant pool?"
____________________________________________________________________________________________________________________________________________________________________________

**Dashboard**

<img width="664" height="337" alt="image" src="https://github.com/user-attachments/assets/1c4ef9f7-77b4-4bb8-96df-0f4fededb052" /> 

<img width="598" height="273" alt="image" src="https://github.com/user-attachments/assets/f97537cd-87a3-4daa-a51b-80a019a8dc6b" /> 

<img width="599" height="274" alt="image" src="https://github.com/user-attachments/assets/96d03d62-8a02-4582-8943-400f29e0fa82" /> 

<img width="602" height="272" alt="image" src="https://github.com/user-attachments/assets/3de7aca6-7739-452e-a883-3ba602ecc5d5" />

____________________________________________________________________________________________________________________________________________________________________________
**Executive Summary: Systemic Hiring Bias Analysis**

**Critical Finding: Merit Does Not Predict Hiring**

Across all assessment dimensions (technical, communication, aptitude, coding), candidate scores are statistically identical across demographics. Yet hiring outcomes diverge by up to 3.4x - proving bias occurs at the decision stage, not in candidate quality.

**1. Gender Discrimination**
Impact: Males hired at 35.3% vs 30.9% females vs 26.6% non-binary
Gap: 4.4 percentage points (14% relative disadvantage for females)
Merit Evidence: Identical assessment scores across all groups (~69 technical, ~65 communication, ~65 aptitude, ~64 coding)
Qualifications: Equal project counts (~6), certifications (~3), GitHub scores (~62)
Conclusion: Gender is influencing decisions despite equal merit

**2. Educational Prestige Bias**
Impact: Tier 1 university graduates hired at 44% vs 26% for Tier 3
Gap: 18 percentage points (1.7x multiplier)
Merit Evidence: Technical scores nearly identical (Tier 1: ~69, Tier 3: ~68)
Risk: Missing qualified talent due to university branding bias
Cost: Potential discrimination claims; reduced talent pool diversity

**3. Age Discrimination**
Impact: 35-44 age group at 38% vs under-25 at 19% hire rate
Gap: 19 percentage points (2x disadvantage for younger candidates)
Pattern: Strong mid-career preference, systematically excluding younger and older talent
Legal Risk: Age-based discrimination violates equal employment laws

**4. Experience Barrier (Career-Starter Penalty)**
Impact: 10+ years experience at 54% vs 0-2 years at 16% hire rate
Gap: 38 percentage points (3.4x multiplier - largest bias in dataset)
Merit Evidence: Entry-level candidates show strong technical scores comparable to experienced hires
Consequence: Creates impossible barrier - can't get experience without first job; blocks diverse, younger talent pipeline
Business Impact: Losing fresh perspectives and tech-native skills

**5. AI System Amplification Risk**
Finding: AI resume scores and bias scores are being generated but hiring decisions show bias patterns
Question: Is the AI detecting bias or perpetuating it?
Action Needed: Audit AI resume scoring system for demographic parity
Red Flag: AI bias scores vary by gender (avg ~44 male, ~42 female) - requires investigation

**6. Equal Input, Unequal Output (The Smoking Gun)**
Most Damning Evidence:
Technical skill: Male 69.1, Female 68.8, Non-Binary 69.1 (0.3 point range)
Communication: Male 66.2, Female 65.4, Non-Binary 65.7 (0.8 point range)
Aptitude: Male 65.5, Female 65.8, Non-Binary 65.1 (0.7 point range)
Coding: Male 64.9, Female 64.3, Non-Binary 64.5 (0.6 point range)
Yet hiring rates span 26.6% to 35.3% - a 33% relative difference
This is statistically impossible to explain by merit. The assessment process is fair; the hiring decision process is biased.

**Legal & Compliance Risks**
Adverse Impact Analysis (4/5ths Rule):
Gender: Female hire rate (30.9%) / Male hire rate (35.3%) = 0.875 - PASSES threshold but concerning
Age: Under-25 (19%) / 35-44 (38%) = 0.50 - FAILS (below 0.80 threshold)
Experience: 0-2 years (16%) / 10+ years (54%) = 0.30 - CRITICAL FAIL
Litigation Risk: High - clear statistical evidence of disparate impact without business justification

**Business Impact**
Talent Loss: Rejecting 70-84% of entry-level and Tier 2/3 university candidates who score identically to hired candidates
Cost: Higher salaries for 10+ year candidates when entry-level talent could perform equally well
Innovation Risk: Homogeneous hiring (mid-career, Tier 1, male-skewed) reduces cognitive diversity and fresh perspectives
Reputation: Bias patterns contradict stated diversity commitments - risk to employer brand

**Recommended Immediate Actions**
Implement Blind Resume Review: Remove names, universities, graduation dates pre-screening
Structured Interview Scoring: Use standardized rubrics; assessment scores should drive decisions
Diverse Interview Panels: Reduce individual bias through panel diversity
Audit AI Systems: Validate AI resume scoring for demographic parity
Set Representation Targets: 35% female, 40% Tier 2/3, 25% entry-level in next cohort
Manager Training: Data-driven bias awareness with these specific findings
Monthly Monitoring: Track hire rates by demographics; flag deviations >5%

Bottom Line: This organization has built fair assessment tools but is not using them to make fair decisions. The fix is process-based, not candidate-based.

____________________________________________________________________________________________________________________________________________________________________________

## Tools & Purpose for AI Hiring Bias Analysis

| Tool | Purpose | Application to AI Hiring Bias Dataset |
| --- | --- | --- |
| **Databricks** | Unified data platform and analytics workspace | Hosts the `ai_recruitment_biasness.ai_bias.ai_hiring_bias_dataset` table, provides compute for SQL queries, supports collaborative analysis, and serves interactive dashboards for bias detection |
| **Databricks Genie Space** | AI-powered conversational analytics agent | Enables natural language queries like "Show me hiring rate disparities by gender" and automatically generates SQL to analyze the 5,000 candidate records, accelerating insight discovery |
| **PySpark** | Distributed data processing and analysis | Prepares and transforms the 18-column candidate dataset, calculates derived metrics (age groups, experience levels), performs statistical analysis for adverse impact ratios, and creates aggregated views for visualization |
| **SQL** | Query language for data validation and analysis | Validates hiring outcomes across demographics, checks data quality (null values, outliers in scores), computes compliance metrics (4/5ths rule), and answers specific analytical questions like "What's the average technical score for hired vs not-hired candidates?" |
| **Lakeview Dashboards** | Interactive business intelligence visualization | Displays 27+ widgets showing hiring rates, merit gaps, intersectional analysis, and compliance indicators; 5 global filters enable dynamic exploration by gender, university tier, experience, age, and education |
| **Unity Catalog** | Data governance and metadata management | Provides schema documentation, lineage tracking, access controls for sensitive candidate data (PII protection), and ensures audit trails for compliance reporting |
| **GitHub** | Version control and collaboration | Manages dashboard YAML definitions, SQL queries, PySpark scripts, analysis notebooks, and project documentation; enables reproducible bias audits and peer review of analytical methods |
| **Microsoft Word / Markdown** | Documentation and reporting | Creates executive summaries, legal compliance reports, methodology documentation, and actionable recommendations for HR leadership; formats findings for non-technical stakeholders |
| **Python (Pandas)** | Statistical analysis and data export | Performs advanced statistical tests (chi-square, t-tests), generates Excel exports with multiple analysis sheets, creates summary statistics, and validates dashboard calculations |
| **Metric Views** | Centralized business metrics layer | Defines reusable measures (`hire_rate`, `avg_technical_score`) and dimensions (`gender`, `university_tier`) to ensure consistent calculations across all dashboards and reports |

## Workflow Integration

**1. Data Ingestion** → Databricks (Unity Catalog) hosts raw candidate data  
**2. Exploration** → Genie Space + SQL for initial pattern discovery  
**3. Analysis** → PySpark for statistical calculations, metric views for standardized KPIs  
**4. Visualization** → Lakeview dashboards with 27 widgets and 5 global filters  
**5. Validation** → SQL queries to cross-check findings and test compliance thresholds  
**6. Documentation** → Word/Markdown for executive summary and legal recommendations  
**7. Version Control** → GitHub for reproducibility and audit trails  
**8. Export** → Python/Pandas for Excel deliverables to non-technical stakeholders

This toolkit enables end-to-end bias analysis from raw candidate data to actionable compliance recommendations, supporting both technical deep-dives and executive-level decision-making.

____________________________________________________________________________________________________________________________________________________________________________
**Curated by Mono Sejake**
