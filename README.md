# Student Performance Prediction Using Machine Learning

A mini project from MNR University using a Random Forest Classifier to classify students as **Pass** (G3 >= 10) or **Needs Support** (G3 < 10).

## Project overview

- Dataset: UCI Student Performance — Mathematics (`student-mat.csv`)
- Records: 395 students; 33 attributes, as described in the project report
- Algorithm: Random Forest Classifier (200 trees)
- Model A: uses background and behavioural features without G1/G2 for early-warning prediction
- Model B: includes G1/G2 as a comparison model
- Libraries: Pandas, NumPy, Matplotlib, Seaborn and Scikit-learn

## Files

- `student_performance.py` — complete Python implementation extracted from the report
- `Project_Report.docx` — uploaded project report
- `requirements.txt` — Python dependencies
- `DATASET_LINK.txt` — official dataset download instructions
- `figures/` — graphs are generated here when the script runs

## Setup and run

1. Install Python 3.
2. Download the Mathematics dataset from the [UCI Student Performance page](https://archive.ics.uci.edu/dataset/320/student+performance).
3. Extract `student-mat.csv` into this repository's main folder, beside `student_performance.py`.
4. Open a terminal in this folder and install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

5. Run the project:

   ```bash
   python student_performance.py
   ```

The script prints dataset information and model evaluation, creates graph images in `figures/`, and writes `results.json`.

## Reported results

According to the report, Model A achieved 72.15% test accuracy and 69.37% mean 5-fold cross-validation accuracy. Model B achieved 91.14% test accuracy and 91.39% mean 5-fold cross-validation accuracy. Model B uses previous-period grades, so Model A is the early-warning model.

## Team

- Sukanya Devi Rayapati — 25RBAIM0074
- Nandini Nagadapally — 25RBAIM0070
- Someshwari Thogarpally — 25RBAIM0075
- Sahitya Chamanthula — 25RBAIM0077

Department of Computer Science and Engineering (AI & ML), MNR University, Academic Year 2026–2027. Faculty Guide: Dr. M. Praveen.

## Before submission

Add the final project presentation (`Project_Presentation.pptx`) and a demo video or public video link. Run the code on your computer and verify the output before submitting. Each team member should create or fork their own public GitHub repository and submit their own repository URL, as instructed by the course announcement.
