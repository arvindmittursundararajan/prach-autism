# Prach AI: Technical Architecture and Development Plan

This document outlines the technical architecture and development plan for Prach AI, a platform designed to empower the neurodiverse community.

## I. User Interaction & LLM

*   **Multimodal Input:**  Supporting diverse modalities like speech, touch, and gestures for seamless user interaction.
*   **Predictive LLMs:** Utilizing Large Language Models (LLMs) to predict user responses, powering Automatic Speech Recognition (ASR) and interpreting visual cues for dynamic communication.

## II. Content & Gamification

*   **Gen AI Content:** Generating engaging learning content (images, videos) for children using generative AI models to visually explain concepts.
*   **Gamification:** Integrating gamification with Dash Plotly for displaying scores and progress to motivate and encourage user engagement.

## III. Model Enhancement & Data

*   **Mixture of Experts (MoE) Approach:** Employing a Mixture of Experts approach, combining Gemini with LLAMA for better, more nuanced responses.
*   **Data Grounding:** Prioritizing data grounding by creating our own preferred content to combat misinformation and ensure trustworthy information.

## IV. Accessibility & UX

*   **Neurodiversity-Friendly Prompts:** Conducting extensive prompt engineering to craft neurodiversity-friendly responses tailored to individual needs.
*   **WCAG Compliance:** Incorporating Web Content Accessibility Guidelines (WCAG) into our UX design for an inclusive and user-friendly experience.

## V. Specialized SLMs

*   **Targeted SLMs:** Developing small language models (SLMs) for speech, Occupational Therapy (OT), and special education, focusing on specific needs.

## VI. Bias Mitigation & Data Integrity

*   **Bias Identification:** Implementing bias identification using fairness metrics to detect and mitigate bias in our deployed models.
*   **Bias Mitigation Techniques:** Utilizing bias mitigation techniques, including data pre-processing and algorithm modification, to address bias in classification.
*   **Data Diversity & Monitoring:** Emphasizing diverse data and continuous monitoring to ensure representative data and promote fairness.

## VII. Prompting & Refinement

*   **Structured Prompting:** Using structured prompting with clear, specific prompts to guide AI responses for targeted information and support.
*   **Context & Persona:** Leveraging context and persona in prompts, tailoring AI interactions for specific client needs and scenarios.
*   **Output Refinement:** Refining AI outputs through exemplars and tone prompting to ensure accuracy, relevance, and ethical considerations.

## VIII. Conversation Management

*   **Organized Conversations:** Organizing and labeling conversations for easy access and reference, improving efficiency and knowledge management.

## IX. Data Architecture

*   **Data Storage:** PostgreSQL database with normalized schema for operational data, coupled with robust metadata management for discoverability and governance.
*   **Data Warehouse:** A dedicated data warehouse stores aggregated and transformed data, enabling analytical reporting, performance monitoring, and business intelligence insights.
*   **Knowledge Graph:** A property graph database (e.g., Neo4j) represents relationships between neurodiversity concepts, resources, experts, and user profiles, facilitating knowledge discovery.
*   **Vector Database:** Prach utilizes Pinecone, a scalable vector database, with OpenAI embeddings and cosine similarity to power semantic search and retrieval for RAG.
*   **Data Pipeline:** The data pipeline includes validation against schemas, user-generated content moderation, data extraction from diverse sources, and transformation using Python tools.
*   **RAG:** The Retrieval Augmented Generation process involves generating and storing embeddings, retrieving relevant chunks from the vector database and knowledge graph, and augmenting LLM prompts.
*   **Data Access:** Prach employs Role-Based Access Control (RBAC), data federation for external sources, OAuth 2.0 authentication, and manages separate RAG instances for data privacy and relevance.
