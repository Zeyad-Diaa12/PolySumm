# PolySumm: Multimodal Scientific Paper Summarization

## Project Overview

### Problem Statement
The exponential growth of scientific literature presents a significant challenge for researchers seeking to efficiently extract key information. Traditional summarization approaches primarily focus on text, often neglecting critical information embedded within figures and tables. This limitation leads to incomplete understanding and inefficient knowledge acquisition, particularly in fields where visual data representations are crucial.

### Objectives
This project aimed to develop a comprehensive multimodal summarization system for scientific papers. The system integrates information from text, figures, and tables to generate more complete and informative summaries. Our specific objectives included:

1.  **Designing a Robust Pipeline:** To extract structured content from scientific PDF documents.
2.  **Implementing Specialized Summarization Models:** For different content types (text, figures, and tables).
3.  **Integrating Components within a RAG Framework:** To leverage Retrieval-Augmented Generation for enhanced summarization.
4.  **Providing an Accessible User Interface:** To enable researchers to easily utilize this technology.

### Methodology
PolySumm employs a sophisticated system architecture that combines advanced OCR capabilities with specialized summarization models within a Retrieval-Augmented Generation (RAG) framework. The core methodology involves:

*   **Multimodal Data Extraction:** Utilizing PaddleOCR to process scientific PDFs, extracting text, identifying figures, and recognizing table structures. The extracted data is then outputted in a structured JSON format.
*   **Data Preprocessing:** The structured JSON data undergoes rigorous preprocessing, including semantic chunking and embedding generation, before being fed into the RAG pipeline.
*   **Distinct Summarization Approaches:** The system employs different summarization techniques tailored to each content type:
    *   **Text Summarization:** Achieved using transformer-based models.
    *   **Figure Description:** Handled by vision-language models.
    *   **Tabular Data Summarization:** Performed by specialized table-to-text models.
*   **User Interface:** A React-based frontend allows users to upload scientific papers and view the generated multimodal summaries.
*   **Comparative Evaluation:** To validate our approach, we implemented and compared two RAG pipelines: a custom system utilizing in-house summarization models and a second system relying on external APIs (specifically, Azure OpenAI).

### Achievements
The project successfully delivered an effective multimodal scientific paper summarization system. Key achievements include:

*   **Implementation of Two RAG Pipelines:** A custom-built system with in-house summarization models and an API-based system via Azure OpenAI.
*   **Superior Performance of Custom System:** The custom system demonstrated higher accuracy, better integration of figures and tables, faster inference times, and lower resource usage. This makes it particularly well-suited for domain-specific tasks requiring deep multimodal understanding.
*   **Validation of Tailored Approach:** The custom RAG pipeline consistently outperformed the API-based system in terms of accuracy, efficiency, and content completeness, validating the benefits of a tailored, modality-aware summarization approach for scientific documents.

## Key Features

*   **Multimodal Summarization:** Summarizes scientific papers by integrating information from text, figures, and tables.
*   **PDF Processing:** Robust pipeline for extracting structured content from PDF documents.
*   **Advanced OCR:** Leverages PaddleOCR for accurate text, figure, and table recognition.
*   **Retrieval-Augmented Generation (RAG):** Enhances summarization quality by retrieving relevant information.
*   **Specialized Models:** Utilizes transformer-based models for text, vision-language models for figures, and table-to-text models for tables.
*   **User-Friendly Interface:** Intuitive React-based frontend for easy paper uploads and summary viewing.
*   **Comparative Analysis:** Provides insights into the performance of custom vs. API-based RAG implementations.

## Technologies Used

*   **Frontend:** React
*   **OCR:** PaddleOCR
*   **Natural Language Processing (NLP):** Transformer-based models (for text summarization), Vision-Language Models (for figure summarization), Table-to-Text Models (for table summarization)
*   **Backend/Framework:** Retrieval-Augmented Generation (RAG)
*   **Optional Integration:** Azure OpenAI

## Demo Video

A short demonstration of the PolySumm system in action is available below:

[//]: # (Placeholder for demo video)

<video src="PolySumm-Demo.mp4" controls title="PolySumm Demo"></video>


