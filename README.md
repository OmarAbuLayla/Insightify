# Insightify – AI-Powered Data Storytelling from CSVs

Insightify is a streamlined, local AI tool that transforms raw CSV data into structured, human-readable insights. Designed for analysts, strategists, and decision-makers, Insightify enables fast, contextual understanding of trends, risks, and opportunities—without writing code.

**Demo Video:** [Watch on YouTube](https://youtu.be/G_MMJpKSuwg)

---

## Key Features

- CSV file upload with optional drag-and-drop functionality
- User-defined analysis goal (e.g., "Find key churn indicators")
- Audience targeting for tone and relevance (e.g., "Marketing team")
- Automatic generation of narrative insights using a local LLM
- Secure by design—your data is processed entirely offline
- Clean, minimal interface built with Tailwind CSS

---


## How It Works

1. The user uploads a `.csv` dataset through the web interface.
2. They enter a specific **goal** and specify the **intended audience**.
3. The backend extracts statistical insights using a custom Python engine:
   - Descriptive statistics (mean, standard deviation, skew)
   - Outlier detection (Z-score)
   - Correlations (Pearson's r)
   - Value distributions for categorical data
   - Detection of duplicates and missing values
4. These insights are passed to a local LLM (Zephyr-7B-beta) through a prompt template.
5. The model generates a structured narrative with:
   - Paragraph 1: Overview of the dataset
   - Paragraph 2: Key patterns and risks
   - Paragraph 3: Recommendations

---

## Tech Stack

- Backend: Python, Flask
- LLM Engine: Zephyr-7B-beta via HuggingFace Transformers and BitsAndBytes
- Data Processing: pandas, numpy, scipy
- Architecture: Local-only (no external API calls)

---

## Use Cases

- Business analysts generating reports from raw business data
- Marketing and sales teams understanding customer patterns
- Founders or product managers presenting insights to stakeholders
- Students or researchers summarizing experimental data

---
