# Job Skills Analysis [![Google Colab Notebook](https://img.shields.io/badge/Google%20Colab-Open-orange?logo=google-colab)](https://colab.research.google.com/)

The objective of this project is to automatically extract required skills from job advertisements. The goal is to gain an understanding of how skill requirements have evolved over time.

## Methodology
The project uses job listings data provided by the platform JobTeaser. The project includes translation, natural language processing, and topic modeling techniques to extract relevant information from the job descriptions.

## Implementation
The project is implemented in Python and makes use of various libraries such as pandas, nltk, langdetect, translatepy, BeautifulSoup, re, IPython, requests, pyldavis, odfpy, matplotlib, spacy, seaborn, wordcloud, ipywidgets, scikit-learn, tomotopy, gensim and lda-over-time.

## Project Structure

The project is divided into three parts:

- **Part I: General Preprocessing and Translation**

  Designed to filter out duplicate job postings, translate non-English job postings into English language, and perform initial general preprocessing. The results will be outputted in an Excel file, which can be used for further analysis.

- **Part II: Skill Section Extraction**

  The system systematically extracts the qualification section from English job advertisements by scanning the HTML source code. It identifies key phrases and specific patterns, derived from the analysis of over 1500 job ads, to accurately pinpoint the skill section within a job description. The extracted qualifications, along with the remaining job ad data, are compiled in a data frame and exported to an Excel file for further analysis. Ads where the qualification section couldn't be extracted are automatically excluded from the export.

- **Part III: Text Preprocessing and Skill Analysis**

  Offers a variety of features designed to track and analyze the progression of desired job qualifications over time. The program should be executed in Google Colab. There are three implemented analysis options for this:

  1. Frequency Analysis
  2. LDA Topic Modeling
  3. Dynamic Topic Modeling

## Getting Started
- Please open the notebook in Google Colab and execute the cells sequentially. Start with Part 1, followed by Part 2 & Part 3. Each part, with the exception of Part 3, will generate an Excel document that serves as input for the subsequent part, ensuring a seamless transition and maintaining continuity in the analysis.
