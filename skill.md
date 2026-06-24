# 🧭 Project Workbook & AI Context Ledger (skill.md)

This file serves as the definitive source of truth, historical ledger, and developer guide for the **BITS Pilani M.Sc. DS & AI - Advanced Apex Project II**. It provides immediate, rich context for both human developers and future AI coding agents.

> [!IMPORTANT]
> **AI AGENT RULE:** Before starting any work in this workspace, read this entire file. When a new week's folder is added or new milestones are achieved, **you must update this file** following the maintenance instructions at the bottom.

---

## 🚀 Project Dashboard

| Metric | Project Detail |
|---|---|
| **Course** | M.Sc. Data Science & Artificial Intelligence (Cohort-1, Trimester-3) |
| **Instructor** | Prof. Bharathi Dasari |
| **Project Selection** | **P1: Employee Attrition Prediction & Workforce Risk Analysis** |
| **Selected Dataset** | `Employee_Dataset_Retail.csv` (10,000 rows × 23 columns) |
| **Primary Domain** | Retail Operations & HR Analytics |
| **Project Type** | Supervised Machine Learning (Binary Classification) |
| **Current Stage** | **Week 2: Project Outline & Baseline Setup** (Completed) |

---

## 📂 Project Directory Structure

```
📂 apex-project2-bits/ (Root)
├── 📁 resources/                       # Course resource directory
│   ├── 📄 Problem Statements_Apex-2_C1.pdf
│   ├── 📄 Student_Guidance_Document_C1_Apex-2_Bharathi.docx.pdf
│   ├── 📁 week1/
│   │   └── 📄 powerpoint.pdf
│   └── 📁 week2/
│       ├── 📄 Advanced_Apex_Project2_Week2_Outline_Template.pdf
│       ├── 📓 Apex2_Week2_Notebook_Template1.ipynb
│       ├── 📓 Retail_Attrition_Assignment.ipynb
│       └── 📄 Week2_Submission_Expectations.pdf
├── 📁 submission/                      # Submission directory (notebook, dataset, outline, and feedback)
│   ├── 📓 2025EM1100026_AnikDas_Week2_Notebook.ipynb
│   ├── 📄 Employee_Dataset_Retail.csv
│   ├── 📄 2025EM1100026_AnikDas_Week2_Outline.docx
│   ├── 📄 2025EM1100026_AnikDas_Week2_Outline.pdf
│   └── 📄 2025EM1100026_Anik_Das_week2_feedback.txt
├── 📁 backup/                          # Backup folder with old datasets
├── 📄 skill.md                         # THIS FILE (AI Context & Project Ledger)
├── 📄 pyproject.toml                   # Project dependencies (managed via uv/pip)
├── 📄 uv.lock                          # Dependency lock file
└── 📁 .venv/                           # Python Virtual Environment
```

---

## 🎓 Academic Core Values & Grading Rubric
The BITS Pilani evaluator and course curriculum emphasize the following core tenets:
1. **Experimentation > Perfection:** Selecting a unique, retail-specific dataset with missing values demonstrates *sincere effort* and initiative over copying standard tutorials.
2. **Multi-Model Evaluation:** At least **4-5 models** must be trained and compared (Logistic Regression, Decision Trees, Random Forests, Gradient Boosting, and KNN).
3. **The "What-Why-Which-Insight" Rule:** A metric result is not enough. You must interpret:
   - *What happened* (performance comparison)
   - *Why it happened* (model characteristics)
   - *Which features influenced it* (feature importance)
   - *What business insights apply* (actionable recommendations for store managers)
4. **Rich Explanations:** Include clear markdown commentary before and after all code cells to support AI-assisted grading quality.

---

## 📅 Cumulative Weekly Progress

### 📍 Week 1: Problem Selection & Foundation
- **Orientation & Scope:** Understood that Apex Project II is an *experimentation-oriented* project rather than deployment-oriented.
- **Problem Selected:** Selected **P1: Employee Attrition**.
- **Key Concepts Learned:** Classification workflows, importance of establishing baselines, and course deliverables layout.
- **Key Artifact Created:** `week1_ppt_analysis.md` summarizing the core course expectations.

### 📍 Week 2: Dataset Selection & Project Outline Setup
- **Dataset Verdict:** Evaluated the popular IBM HR dataset vs. custom alternatives. Rejected IBM HR because it is massively overused (1,470 rows, zero missing values, zero retail-specific context).
- **Adopted Dataset:** Selected `Employee_Dataset_Retail.csv` (10,000 rows × 23 features), purpose-built for retail, with a balanced size, and intentional missing values (1.5% in key variables) to show preprocessing and imputation skills.
- **Baseline Plan:** Planned Logistic Regression as the baseline.
- **Comparison Models:** Selected Decision Trees, Random Forests, Gradient Boosting, and KNN.
- **Evaluation Plan:** Target ROC-AUC and F1-score (Class 'Yes') to counter the ~16% class imbalance using SMOTE/class weights.
- **Key Deliverables Created:** 
  1. `Employee_Dataset_Retail.csv` downloaded and calibrated to 16.12% attrition at root.
  2. `Retail_Attrition_Assignment.ipynb` fully structured and written to root with custom retail headers and code setups.
  3. `week2_analysis.md` artifact detailing all submission expectations and templates.

---

## 🤖 Instructions for AI Agents (Maintenance & Governance)

Future AI agents working on this project **MUST** adhere to the following rules:

### 1. Document Everything
Any file changes, model experiments, or feature engineering choices must be commented clearly in the `.ipynb` notebook and documented in a matching markdown log. Keep the project extremely clean and elegant.

### 2. Follow the Academic Style
Never write lazy or superficial code. Write clean, modular scikit-learn pipelines. Visualize comparisons using high-quality matplotlib/seaborn charts. Ensure that markdown insights are written in a professional, academic tone.

### 3. How to Update `skill.md` (Crucial Maintenance Rule)
Whenever you start a new week or complete a major project phase:
1. Locate the **Cumulative Weekly Progress** section.
2. Add a new sub-heading `### 📍 Week [Number]: [Title/Milestone]`.
3. List the **Objectives accomplished**, **Key decisions made**, and **Deliverables produced** in a concise bullet-point list.
4. Update the **Current Stage** and **Status** in the `🚀 Project Dashboard` table at the top.
5. If you create new folders (e.g. `week3/`), add them to the `📂 Project Directory Structure` diagram.
6. Commit the changes back to `skill.md` as part of your turn execution.

---

### 📝 Next Action Items (For Future Weeks)
- **Data Preprocessing (Week 3/4):** Perform group-wise median imputation on `MonthlyIncome` based on `JobRole`, encode categorical variables, and apply standard scaling.
- **EDA & Visualizations:** Plot distribution of Age, Income, and Attrition across departments/roles, and analyze correlation matrices.
- **Feature Engineering:** Extract season and tenure from `Date_of_Joining`, compute pay ratio metrics relative to role medians, and progression ratios.
- **Model Training:** Establish the baseline Logistic Regression and train the advanced tree-based classifiers.
