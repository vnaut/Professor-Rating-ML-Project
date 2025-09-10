# 🌟 Professor Rating ML Project

This repository contains a data science and machine learning pipeline for analyzing professor ratings, course data, and grade distributions using the [PlanetTerp API](https://planetterp.com/api/v1). The core workflow is implemented in the Colab notebook: [`PlanetTerp_Professors_ML_Project.ipynb`](https://github.com/vnaut/Professor-Rating-ML-Project/blob/main/PlanetTerp_Professors_ML_Project.ipynb).

## 🚀 Project Overview

This project:
- Fetches professor, course, and grade distribution data from PlanetTerp via their public API.
- Cleans, aggregates, and organizes this data for analysis.
- Builds rich feature sets for professors, combining course history, grades, and student review sentiment.
- Applies sentiment analysis (using [Flair](https://github.com/flairNLP/flair)) to professor reviews.
- Prepares ML-ready datasets for rating prediction, analytics, or further research.

## 📒 Main Notebook

Open the main notebook in Google Colab:<br>
<a href="https://colab.research.google.com/github/vnaut/Professor-Rating-ML-Project/blob/main/PlanetTerp_Professors_ML_Project.ipynb" target="_parent">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>

## 🧑‍💻 How It Works

1. **Data Collection:**  
   - Fetches all professors, courses, and grade distributions from the PlanetTerp API.
   - Stores data in `professors.json`, `courses.json`, and `grades.json`.

2. **Feature Engineering:**  
   - Aggregates course-level and grade-distribution statistics per professor.
   - Sentiment analysis on student reviews using Flair NLP (`en-sentiment` model).
   - Maps expected letter grades to numeric values for averaging.

3. **Dataset Construction:**  
   - Joins all features to produce a single row per professor, suitable for ML or statistical analysis.

## ⚡ Quick Start

1. **Clone the repository:**
   ```bash
   git clone https://github.com/vnaut/Professor-Rating-ML-Project.git
   ```

2. **Open the Colab notebook** and run all cells:  
   [PlanetTerp_Professors_ML_Project.ipynb](https://github.com/vnaut/Professor-Rating-ML-Project/blob/main/PlanetTerp_Professors_ML_Project.ipynb)

3. **Dependencies:**  
   The notebook installs required packages automatically, including `flair` for sentiment analysis.

## 📊 Outputs

- **professors.json** — All professors and their details
- **courses.json** — Detailed course metadata
- **grades.json** — Grade distributions per professor/course
- **ML dataset** — Aggregated features for modeling professor ratings

## 📝 Example Analyses

- What course features predict higher professor ratings?
- How do grade distributions correlate with student sentiment?
- Do certain departments or courses have systematically different review patterns?

## 🤝 Contributing

Pull requests and suggestions welcome! Please open an issue or PR to discuss major changes.

## 📄 License

This project is distributed under the MIT License.

---

**Created by [vnaut](https://github.com/vnaut)**  
For questions or collaboration, feel free to reach out!
