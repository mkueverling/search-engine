# Search Engine & Information Retrieval

This repository contains a series of exercises and projects exploring the core technologies behind modern search engines. Starting with the fundamentals of Apache Solr and Elasticsearch, the projects cover practical tasks such as environment setup, corpus indexing, and query execution. The repository culminates in a comprehensive capstone project participating in the TREC 2024 Product Search challenge.

## Project Structure

Each section represents a distinct module focusing on a specific search technology or assignment.

### 1. Apache Solr Basics
* **Files:** `solr_exercises/`
* **Description:** This section introduces the Apache Solr search platform. It includes a series of introductory exercises designed to familiarize the user with the ecosystem. Topics include launching a local Solr instance, configuring cores, and performing basic data operations to understand how Solr manages and retrieves content.

### 2. Elasticsearch Fundamentals
* **Files:** `elasticsearch/`
* **Description:** This module transitions to Elasticsearch, focusing on the programmatic management of indices. The first assignment demonstrates how to set up an index from scratch and ingest a text corpus. It establishes the groundwork for handling unstructured data and defining mappings for efficient retrieval.

### 3. Capstone Project: TREC 2024 Product Search
* **Files:** `trec-project/`
* **Description:** The most significant component of this repository, this capstone project focuses on the **TREC 2024 Product Search Track**. It involves processing and indexing a massive e-commerce corpus containing **1.1 million documents**.
    * **Objective:** To build a robust retrieval system capable of handling real-world e-commerce data challenges.
    * **Core Task:** The primary implementation is located in `2_assignment.ipynb`, which details the indexing pipeline, data preprocessing, and search configuration required to handle the scale of the TREC dataset.
    * **Context:** This project addresses the complexities of product search, such as handling diverse product descriptions and optimizing for relevance in a large-scale catalog.

## Key Concepts Covered
* **Search Engines:** Apache Solr, Elasticsearch
* **Information Retrieval:** Indexing pipelines, Schema design, Document ingestion.
* **Data Handling:** Processing large-scale corpora (1.1M+ documents), E-commerce data structures.
* **Evaluation:** working within the constraints and standards of the Text REtrieval Conference (TREC).
* **Python Integration:** Using client libraries to interface with search servers programmatically.

## How to Use
1.  Clone the repository to your local machine:
    ```bash
    git clone [https://github.com/mkueverling/search-engine.git](https://github.com/mkueverling/search-engine.git)
    ```
2.  Navigate into the cloned directory:
    ```bash
    cd search-engine
    ```
3.  **Prerequisites:** Ensure you have Java installed (for Solr/Elasticsearch) and the necessary Python drivers:
    ```bash
    pip install elasticsearch pysolr pandas jupyter
    ```
4.  **Running the Capstone:**
    * Navigate to `trec-project/`.
    * Ensure your Elasticsearch instance is running and accessible.
    * Open the core assignment notebook:
        ```bash
        jupyter notebook 2_assignment.ipynb
        ```
    * Follow the notebook cells to ingest the corpus and execute search queries.
