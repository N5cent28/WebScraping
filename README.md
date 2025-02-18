
---

# Web Scraping Overview

This repository contains various scripts and Jupyter Notebooks used for web scraping tasks, primarily focused on gathering and analyzing data for different bioinformatics projects.

## Contents

### [GEO_Webscrape_fromRTF.ipynb](https://github.com/N5cent28/WebScraping/blob/main/GEO_Webscrape_fromRTF.ipynb)

This Jupyter Notebook scrapes demographic data from individuals to regress on covariants for epigenetic age predictions. The dataset was then fed to an unsupervised machine learning model to investigate the epigenetics of aging. The notebook includes:
- Reading and parsing RTF files.
- Extracting GSM IDs, URLs, and sample titles.
- Scraping demographic information from individual pages.
- Converting data to a DataFrame and saving to CSV.

### [GEO_Webscrape_fromTXT.ipynb](https://github.com/N5cent28/WebScraping/blob/main/GEO_Webscrape_fromTXT.ipynb)

Similar to the previous notebook, this script scrapes demographic data from individuals to regress on covariants for epigenetic age predictions, but reads data from a TXT file. It includes:
- Reading individual codes from a TXT file.
- Scraping demographic information from individual pages.
- Converting data to a DataFrame and saving to CSV.

### [ScrapeDeltaG.py](https://github.com/N5cent28/WebScraping/blob/main/ScrapeDeltaG.py)

This Python script was created for a project at Proteovista LLC. It automates the interaction with IDT's Oligo Analyzer Tool to match oligo annealing temperatures. The script demonstrated that the sequence of the HSV genome chosen was not suitable for the task. It later helped find the optimal 900bp region of the HSV genome to maximize the ability to anneal sub-oligos at the same temperature. The script includes:
- Automated login to the IDT website.
- Sequence analysis for dimer and hairpin formations.
- Reading sequences from an Excel file and writing results back.
- Customizing concentration parameters for the analysis.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/N5cent28/WebScraping.git
   ```

2. Navigate to the project directory:
   ```bash
   cd WebScraping
   ```

3. For Jupyter Notebooks, open them using JupyterLab or Jupyter Notebook:
   ```bash
   jupyter lab
   # or
   jupyter notebook
   ```

4. Execute the cells in the notebook to run the analysis and scrape the data.

For the Python script, follow these steps:
1. Ensure you have the required Python packages installed:
   ```bash
   pip install selenium openpyxl httpcore
   ```

2. Set the correct path for ChromeDriver in the script.

3. Run the script:
   ```bash
   python ScrapeDeltaG.py
   ```

---
