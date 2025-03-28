# Graph and Machine Learning Project: Node Classification and Link Prediction

## Overview
This project aims to apply machine learning techniques to a bibliographic dataset using graph-based approaches. You will work in groups of up to four members. Each group must be divided into two sub-groups: one will be responsible for the **node classification** task, while the other will work on the **link prediction** task. The dataset is provided in CSV format, and students will need to clean, preprocess, and construct a graph to train models using **Neo4j** or Python-based machine learning frameworks integrated with Neo4j. The **data cleaning, preprocessing, and graph construction** should be common for both sub-groups.


## Dataset Description
The dataset consists of the following CSV files:

- **authors.csv**: Contains `Author ID` (unique identifier), `Author Name`, `Author URL`
- **journal.csv**: Contains `Journal Name`, `Journal Publisher`
- **paper.csv**: Contains `Paper ID` (unique identifier), `Paper DOI`, `Paper Title`, `Paper Year`, `Paper URL`, `Paper Citation Count`, `Field of Study`, `Journal Volume`, `Journal Date`
- **topic.csv**: Contains `Topic ID`, `Topic Name`, `Topic URL`
- **paper_journal.csv**: Contains `Paper ID`, `Journal Name`, `Journal Publisher`
- **paper_topic.csv**: Contains `Paper ID`, `Topic ID`
- **paper_reference.csv**: Contains `Paper ID`, `Referenced Paper ID`

The dataset is available at [GitHub Repository](https://github.com/habib-university/cs343-project).

## Work Distribution
Each group must split their efforts equally between two tasks:

### Node Classification (Assigning labels to nodes)
You will work on one of the following potential use cases of node classification for bibliographic data.
- **Author Classification:** Predict the research domain or expertise of an author based on their co-authorship network.
- **Paper Classification:** Classify papers into different topics or research fields using citation and co-citation relationships.
- **Journal Classification:** Identify whether a journal belongs to a particular subject category based on its citation patterns.
- **Affiliation Classification:** Predict the academic institution or organization an author is associated with.

### Link Prediction (Predicting missing or future links)
You will work on one of the following potential use cases of link prediction for bibliographic data.
- **Future Collaborations:** Predict potential future collaborations between researchers based on their previous co-authorship networks.
- **Citation Recommendation:** Suggest relevant citations for a research paper by predicting possible citation links.
- **Journal-Paper Recommendation:** Identify suitable journals for submitting a manuscript by predicting which journals are likely to cite it.
- **Topic Evolution Analysis:** Tracks how research topics evolve by predicting future links between papers in different domains.

## Project Workflow

### 1. Data Preprocessing
- Clean and structure the data appropriately.

### 2. Graph Construction
- Develop a Graph Property Model for the data.
- Load the structured data into Neo4j to form a meaningful graph representation.
- Compute graph properties and visualize key statistics.

### 3. Model Selection and Training
- Implement node classification and link prediction using machine learning models.
- Groups can use **Neo4j’s built-in algorithms** within Neo4j Browser or access Neo4j through Python libraries.

### 4. Evaluation and Analysis
- Report the performance of the model using metrics like accuracy, precision, recall, F1-score for node classification; or AUC-ROC, precision-recall for link prediction.
- Discuss model failures and iterative improvements.

## Project Deliverables

### 1. GitHub Repository (One per group)
- Code for data loading, preprocessing, graph construction, and model training.
- Clearly structured README file with instructions for reproducing results.
- Commit history to track individual contributions.

### 2. Report
- **Methodology:** Describe preprocessing steps, chosen models, and reasoning behind selections.
- **Results:** Present success and failure cases, highlighting key findings.
- **Discussion:** Discuss improvements, alternative approaches, and possible extensions.
- **Maximum Limit:** Maximum of 8 pages in a two-column IEEE format (available at [IEEE Templates](https://www.ieee.org/conferences/publishing/templates.html)).

## Submission and Grading Criteria
- **Data Cleaning & Graph Construction (10%)**
- **Model Implementation & Training (20%)**
- **Evaluation & Analysis (30%)**
- **GitHub Repository Structure & Reproducibility (10%)**
- **Report Clarity & Insightfulness (10%)**
- **Progress Check (20%)**
- **Bonus:** The group achieving the best results will be awarded bonus points.

## Milestones and Deadlines
- **Progress Check:** Week 16 (A presentation to show current progress and direction).
- **Report Submission:** May 7, 2025

