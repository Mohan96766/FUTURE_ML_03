# Resume Screening & Candidate Ranking System
**Built with Python, NLP & Machine Learning**  
This project automatically screens, scores, and ranks resumes based on a job description — just like HR-tech tools.

## 📝 Business Problem
Recruiters spend hours manually reading resumes. This project solves that by:
- Shortlisting candidates faster
- Matching skills with job requirements
- Identifying missing or weak skills
- Reducing recruiter workload

## ⚙️ Features
- Clean and preprocess resumes and job description text
- Extract skills using NLP (spaCy PhraseMatcher)
- Compute similarity score with TF-IDF + weighted required skills
- Identify skill gaps per candidate
- Rank candidates by role fit
- Visualizations:
  - Top candidate match scores (bar chart)
  - Skills matched vs missing (stacked bar)
  - Skill coverage heatmap
  - Skill gap heatmap (red/green)
  - Word cloud of top skills
- Export ranked candidates and skill gaps to Excel

## 🛠 Tools & Libraries
- **Python 3**
- **Jupyter Notebook**
- **Libraries**: pandas, numpy, scikit-learn, nltk, spacy, matplotlib, seaborn, wordcloud
- **Optional**: Streamlit / Gradio for interactive dashboard

## 📊 How it Works
1. Resume and job description texts are cleaned and preprocessed.
2. Skills are extracted from resumes using a PhraseMatcher against a curated skill list.
3. Each resume is scored using TF-IDF vectorization + cosine similarity.
4. Must-have skills in the job description are weighted higher.
5. Skill gaps are identified (skills in JD but missing in resume).
6. Candidates are ranked based on final weighted score.
7. Top candidates are visualized using charts and tables.
   
## 🖼 Screenshots / Demo

### Top 10 Candidates Table
![Top Candidates Table](demo_screenshots/top_candidates_table.png)

### Top Candidate Match Scores
![Top Candidates Bar Chart](demo_screenshots/top_candidates_bar_chart.png)

### Skills Matched vs Missing per Candidate
![Skills Matched vs Missing](demo_screenshots/skills_matched_vs_missing.png)

### Skill Coverage Heatmap
![Skill Coverage Heatmap](demo_screenshots/top_candidates_skill_heatmap.png)

### Skill Gap Heatmap (Red = Missing, Green = Present)
![Skill Gap Heatmap](demo_screenshots/skill_gap_heatmap.png)

