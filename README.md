# Sentinel-AI

**Explainable AI-powered security analytics and user behavior anomaly detection.**

SentinelAI is a security analytics project designed to analyze authentication and user activity logs, identify unusual behavior, prioritize potential threats, and support security analysts with evidence-grounded AI-assisted investigations.

## Problem

Security teams receive large volumes of events. Rule-based detection can identify known patterns, but may miss unusual behavior that does not match predefined rules. Anomaly detection can help surface deviations, while risk scoring and incident workflows help analysts prioritize investigations.

## Planned Capabilities

- Security log ingestion and data validation
- Exploratory data analysis and behavioral feature engineering
- Machine learning-based anomaly detection
- Rule-based threat signals and explainable risk scoring
- Incident creation, prioritization, and analyst assignment
- REST API and interactive security dashboard
- Retrieval-Augmented Generation (RAG) for evidence-grounded investigation support
- Automated tests, model evaluation, and deployment

*Capabilities will be marked complete only after implementation and testing.*

## Architecture

The planned pipeline is:

`Security Logs -> Validation -> Feature Engineering -> Detection -> Risk Scoring -> Incidents -> Investigation -> Dashboard`

The investigation layer will retrieve relevant security documentation and provide evidence-linked explanations. AI-generated conclusions will be treated as recommendations, not verified facts.

## Technology Stack

- Python and Pandas for data processing
- Scikit-learn for machine learning
- FastAPI for the backend API
- SQL database for incident persistence
- Streamlit for the dashboard
- Embeddings and an LLM for RAG-based investigation support
- Pytest, Git, Docker, and GitHub Actions for testing and engineering

## Evaluation

The detection pipeline will be evaluated using appropriate metrics such as precision, recall, F1-score, and false-positive rate where ground-truth labels are available. Results will be compared against simple baselines.

## Project Status

**In development.** Models, datasets, measured results, deployment links, and screenshots will be added after they exist and have been verified.

## Responsible Use

SentinelAI is an educational prototype. It will use authorized or synthetic security data and will not autonomously execute disruptive security actions.