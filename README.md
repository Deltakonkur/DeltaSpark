# DeltaSpark Intelligent Konkur Advisor System Documentation

Advanced AI-powered system for weakness analysis and personalized study planning

## Table of Contents

* [System Introduction](#system-introduction)
* [Installation and Setup](#installation-and-setup)
* [Key Features](#key-features)
* [System Architecture](#system-architecture)
* [User Guide](#user-guide)

## System Introduction

**DeltaSpark** is an advanced analytical platform that leverages machine learning and optimization algorithms to identify students' weak points and generate a personalized study plan to improve academic performance.

### Main Capabilities:

* Use of combined Ensemble models for higher accuracy
* Automated identification and prioritization of weak topics
* Personalized study plan generation using Genetic Algorithm

## Installation and Setup

### Requirements

* Python 3.8 or higher
* pip (latest version)
* Operating system: Windows/Linux/MacOS

### Install Libraries

```bash
pip install streamlit pandas numpy plotly scikit-learn xgboost lightgbm catboost geneticalgorithm joblib sqlite3
```

Or use the requirements file:

```bash
pip install -r requirements.txt
```

### Running the System

```bash
streamlit run delta_spark.py
```

By default, the app will be accessible at `http://localhost:8501`.

### Initial Configuration

1. Register a new student from the sidebar on the main page
2. Enter test data manually or use the "Load Sample Data" button
3. Train the AI model by clicking "Train New Model"
4. Use different tabs for data analysis and receiving the study plan

## Key Features

### Student Management

* Full student profiles including name, major, and academic goals
* Data stored in an SQLite database
* Sample data generation for testing

### AI Models

* Advanced models: XGBoost, LightGBM, and CatBoost
* Combined Ensemble model for improved accuracy
* Manual threshold adjustment for weakness detection

### Analysis and Reporting

* Interactive charts with Plotly for data visualization
* Complete classification reports
* Progress trend analysis over time

### Study Planning

* Genetic Algorithm for optimizing study time allocation
* Weekly total study hours customization
* Customized recommendations for each type of weakness

## System Architecture

### Layers of the System

1. **Data Layer**: SQLite Database
2. **Processing Layer**: Python & ML Models
3. **Presentation Layer**: Streamlit UI

### Workflow

1. Data Entry: test scores, study hours, and student info
2. Preprocessing: encoding and normalization of data
3. Model Training: machine learning models trained on data
4. Weakness Analysis: models identify and prioritize weaknesses
5. Plan Optimization: genetic algorithm distributes study time among topics
6. Results Display: visual reports and study plans

## User Guide

### Main Tabs

#### Overview Analysis

* Distribution of scores across subjects
* Study efficiency analysis (score per study hour)
* Identification of weaknesses by subject and topic

#### Study Plan

* Optimized study plan generation with genetic algorithm
* Weekly total study hours adjustment
* Customized solutions for each topic

#### Academic Progress

* Trends of score changes over time
* Score distribution across subjects
* Error and study time distribution analysis

#### Advanced Settings

* Manage and download data
* View model training history
* Review previous study plans

### Important Notes

* For effective performance, at least 10 data samples per student are required.
* Retrain the model after each new data entry for best results.

## Contact Information
* GitHub-Delta: [https://github.com/Deltakonkur](#)
* GitHub-Arshia: [https://github.com/itashia](#)

© 2025 All rights reserved. Version 1.0.0
