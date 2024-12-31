
# Biomedical Text Extraction

PubMed is a vast repository of medical research papers that provides API access to its wealth of data. This data can be harnessed to build knowledge graphs for healthbots and recommender systems. However, a significant challenge lies in sorting the papers effectively: while some journals have high impact factors, others do not. To address this, the current project introduces a scoring method using an unsupervised learning approach.

## Problem Overview

The sorting of papers is based on various features such as:
- Citation count
- Impact factor of the journal
- Research score of the university
- Study type

Due to limitations in web scraping, only the impact factor and research score of universities could be scraped. In this project:
- Data scraping is achieved for impact factors and research scores from different sources.
- The extracted data is merged into a single dataframe.
- GLiner transformer is used to extract entities like universities and study types.

## Key Features

- **Data Extraction**: Extract PubMed data and append impact factors and research scores of different universities.
- **Data Visualization**: Perform exploratory data analysis to understand correlations between various categories.
- **Feature Importance**: Identify and weigh critical features to rank high-quality papers effectively.
- **Entity and Relationship Extraction**: Use Large Language Models (LLMs) such as Llama 3.1 to extract entities and relationships from text and build knowledge graphs.
- **Knowledge Graphs**: Populate data into Neo4j, enabling explainable insights and chatbot functionality for healthcare providers.

## Structure

The repository is organized as follows:

- `pubmed/` - Main directory containing PubMed data processing resources.
  - `notebooks/` - Jupyter notebooks with detailed examples and use cases.
  - `csv/` - Sample CSV files for testing and demonstration purposes.
- `README.md` - Project documentation (you are here!).
- `.gitignore` - Specifies files and directories to ignore in the repository.

## Pipeline Overview

1. **Data Extraction**:
   - Extract data from PubMed.
   - Append impact factor and research scores of universities.
2. **Data Visualization**:
   - Analyze correlations between different categories.
3. **Feature Importance**:
   - Determine and weigh critical features to filter high-quality papers.
4. **Entity and Relationship Extraction**:
   - Utilize BERN2 to extract entities and LLama 3.1 to identify the relationships.
   - Build knowledge graphs using Neo4j.
5. **Chatbot Integration**:
   - Use knowledge graphs to power a chatbot for healthcare providers, offering insights and explainability.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/amulya-incorrigible/Biomedical-Text-Extraction.git
   cd Biomedical-Text-Extraction
