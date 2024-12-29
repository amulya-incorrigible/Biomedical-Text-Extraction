# Biomedical Text Extraction

This repository contains tools and methods for creating a pipeline to extract, analyze, and visualize data from biomedical text sources such as PubMed. The project leverages advanced Natural Language 
Processing (NLP) techniques, data visualization, and knowledge graph construction to streamline the process of identifying high-quality biomedical research papers and making their insights accessible.

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
   - Utilize Llama 3.1 to extract entities and relationships.
   - Build knowledge graphs using Neo4j.
5. **Chatbot Integration**:
   - Use knowledge graphs to power a chatbot for healthcare providers, offering insights and explainability.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/amulya-incorrigible/Biomedical-Text-Extraction.git
   cd Biomedical-Text-Extraction

## Usage

### Example Workflow

1. **Input Data**: Provide PubMed data or related biomedical text files.
2. **Run Notebook**: Open a Jupyter notebook from the `pubmed/notebooks/` directory and follow the instructions for each stage of the pipeline.
3. **Extract High-Quality Papers**: Use feature importance to rank papers.
4. **Build Knowledge Graphs**: Extract entities and relationships, then populate the graph database.


