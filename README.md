<h1 align="center">Natural Language Processing & Social Media Analytics with Python</h1>

This repository showcases an end-to-end **Natural Language Processing (NLP) and social media analytics workflow** built from more than **1 million tweets**, with approximately **409,915 records** retained for analysis after preprocessing. I developed the analytical pipeline independently, covering data cleaning, text preprocessing, sentiment analysis, topic modeling, visualization, and interpretation.

Although the project uses **COVID-19 Twitter data** as its case study, the techniques demonstrated, including **text mining, sentiment analysis, topic modeling, feature extraction, exploratory analysis, and large-scale text processing**, are broadly transferable across marketing, customer analytics, healthcare, public policy, communications, finance, and other data-driven domains.

Using **Python**, **VADER**, **LDA**, **AWS S3**, and a range of NLP and visualization libraries, I transformed large-scale unstructured social media data into interpretable insights about sentiment, dominant discussion themes, and engagement patterns.

The project was completed under a tight **two-day deadline**. I independently developed the technical analysis while also briefing my MBA teammates on the methodology and findings, enabling the team to communicate the results through a concise final presentation.

# 🤝 Technical Leadership & Team Delivery

Although completed as a group assignment, I served as the project's primary analyst and independently developed the complete analytical workflow.

My responsibilities included:

- Building the NLP pipeline from raw data through final analysis.
- Cleaning and processing approximately **409,915 usable tweets**.
- Conducting sentiment analysis and topic modeling.
- Developing the project's analytical visualizations.
- Interpreting the technical findings.
- Explaining the methodology and results to non-technical teammates.
- Supporting the development of the final presentation.

This allowed the broader team to focus on communicating the analytical findings while demonstrating my ability to combine technical execution with cross-functional communication.

# 🎯 Project Goals

The project was designed to apply Natural Language Processing and social media analytics to large-scale unstructured text data.

The primary goals were to:

- Clean and preprocess large-scale social media datasets.
- Analyze public sentiment using NLP techniques.
- Identify dominant conversation themes through topic modeling.
- Explore engagement patterns across social media content.
- Visualize complex textual data clearly.
- Translate NLP outputs into actionable communication insights.
- Demonstrate a reproducible end-to-end text analytics workflow.

# 🏗️ Solution Architecture

### Workflow

```text
Raw Twitter Datasets
        ↓
Amazon S3 Storage
        ↓
Data Cleaning & Preprocessing
        ↓
Text Normalization
        ↓
Exploratory Data Analysis
        ↓
Sentiment Analysis (VADER)
        ↓
Topic Modeling (LDA)
        ↓
Engagement Analysis
        ↓
Data Visualization
        ↓
Analytical Interpretation
        ↓
Final Presentation
```

### Data

- **Dataset:** COVID-19 Twitter Posts
- **Original Volume:** 1M+ tweets across three datasets
- **Processed Volume:** ~409,915 usable tweets
- **Source:** Kaggle
- **Storage:** Amazon S3
- **Data Type:** Unstructured social media text and engagement metadata

### Data Preparation

Prepared the Twitter datasets by:

- Combining multiple source datasets.
- Removing unusable or incomplete records.
- Cleaning URLs, punctuation, emojis, and special characters.
- Normalizing text and capitalization.
- Removing stopwords.
- Tokenizing and lemmatizing text.
- Preparing cleaned text for sentiment and topic modeling.

### Exploratory Data Analysis

Analyzed:

- Tweet volume
- Language distribution
- Hashtag frequency
- Engagement patterns
- User activity
- Sentiment distributions
- Temporal changes in discussion

### Sentiment Analysis

Applied **VADER** sentiment scoring to classify tweets as:

- Positive
- Neutral
- Negative

Sentiment results were then compared with engagement behavior such as likes, replies, and retweets.

### Topic Modeling

Applied **Latent Dirichlet Allocation (LDA)** to identify recurring themes within the Twitter discourse.

Topic modeling was supported by:

- Text vectorization
- Token processing
- Topic extraction
- Keyword interpretation
- Word clouds
- Comparative visualizations

### Data Visualization

Developed analytical visualizations using:

- Matplotlib
- Seaborn
- Plotly
- WordCloud
- Squarify

Visual outputs included sentiment charts, topic distributions, engagement comparisons, word clouds, and treemaps.

### Cloud Storage

Used **Amazon S3** to store both raw datasets and major project deliverables, keeping the GitHub repository lightweight while demonstrating cloud-based data management.

# 📊 Analytical Insights

### Sentiment

- Approximately **53%** of analyzed tweets were negative.
- Roughly **39%** were neutral.
- Positive sentiment represented approximately **8%** of the dataset.
- Negative and uncertain sentiment dominated much of the observed COVID-19 discourse.

### Topic Modeling

LDA identified recurring discussion themes involving:

- Government policy
- Lockdowns and quarantine
- Vaccines
- Economic uncertainty
- Employment
- Health information
- COVID-19 symptoms

### Engagement Patterns

- Negative or controversial content tended to generate stronger retweet activity.
- Neutral posts generated comparatively more replies than likes.
- Engagement spikes often coincided with major COVID-related developments and policy changes.

### Communication Strategy

The analysis demonstrated how organizations can combine sentiment, topic, and engagement data to better understand audience concerns and adapt communication strategies accordingly.

# ⚠️ Project Limitations

- Social media users are not representative of the broader population.
- Demographic attributes were unavailable for most users.
- Social media text contains noise, slang, sarcasm, and contextual ambiguity.
- VADER and LDA provide useful analytical approximations but cannot fully capture human language or intent.
- Findings reflect the available Twitter datasets and should not be generalized to all public opinion.

# 📈 Analytical Recommendations

Based on the analyses:

- Monitor sentiment alongside topic frequency to identify emerging audience concerns.
- Track engagement patterns to determine which subjects generate the strongest public response.
- Adapt messaging strategies when negative sentiment increases around specific topics.
- Combine social media analytics with additional audience and survey data for more complete decision support.
- Use more advanced domain-specific NLP models when deeper sentiment or contextual interpretation is required.

# 🛠️ Technical Skills Demonstrated

### Programming

- Python

### Natural Language Processing

- Text Mining
- Sentiment Analysis
- VADER
- Latent Dirichlet Allocation (LDA)
- Tokenization
- Lemmatization
- Stopword Removal
- Text Normalization
- Topic Modeling

### Data Analysis

- Exploratory Data Analysis (EDA)
- Engagement Analysis
- Social Media Analytics
- Distribution Analysis
- Comparative Analysis
- Large-Scale Text Processing

### Data Preparation

- Data Cleaning
- Data Transformation
- Text Preprocessing
- Missing Data Handling
- Feature Extraction
- Dataset Integration

### Data Visualization

- Matplotlib
- Seaborn
- Plotly
- WordCloud
- Squarify
- Data Storytelling

### Libraries

- pandas
- NumPy
- NLTK
- gensim
- scikit-learn
- VADER
- Matplotlib
- Seaborn
- Plotly
- WordCloud
- Squarify

### Cloud & Software

- Amazon S3
- Visual Studio Code
- Jupyter Notebook

# 💡 What This Project Demonstrates

This project demonstrates the ability to independently design, execute, and communicate an end-to-end NLP workflow using large-scale unstructured data.

Key competencies demonstrated include:

- Transforming raw text into structured analytical data.
- Developing reproducible NLP and text-mining workflows.
- Applying sentiment analysis and topic modeling to real-world datasets.
- Extracting meaningful patterns from large volumes of unstructured information.
- Translating technical outputs into actionable audience and communication insights.
- Communicating complex analytical methods to non-technical collaborators.
- Delivering a complete analytical solution under tight time constraints.

Although centered on social media data, the NLP, analytical reasoning, data preparation, visualization, and communication skills demonstrated are broadly transferable across marketing, customer analytics, healthcare, finance, public policy, research, and other data-driven fields.

# 📁 Repository Structure

```text
Natural-Language-Processing-Social-Media-Analytics-Python/
│
├── Datasets/
│   └── README.md
│       └── AWS S3 link to raw Twitter datasets
│
├── Outputs/
│   └── README.md
│       └── AWS S3 links to project deliverables
│
└── README.md
    └── Project documentation
```

**Datasets**

Contains an AWS S3 link to the original COVID-19 Twitter datasets used throughout the analysis.

**Outputs**

Provides access to:

- Complete Jupyter Notebook
- Project visualizations
- Final presentation

**Repository**

The root README documents the project goals, solution architecture, analytical findings, technical skills, and replication steps.

# 🚀 Replicating the Project

### Clone the Repository

```bash
git clone https://github.com/Awale-Abdi/Natural-Language-Processing-Social-Media-Analytics-Python.git
cd Natural-Language-Processing-Social-Media-Analytics-Python
```

### Download the Data

Open:

```text
Datasets/
```

and follow the provided AWS S3 link to download the original Twitter datasets.

### Access the Project Files

Open:

```text
Outputs/
```

and follow the AWS S3 link to access the complete project deliverables.

Launch:

```text
Social Media Analytics - Team 5 Code by Awale Abdi.ipynb
```

### Run the Analysis

Execute the notebook sequentially to reproduce:

- Data cleaning and preprocessing
- Exploratory data analysis
- Sentiment analysis
- Topic modeling
- Engagement analysis
- Data visualization
- Analytical findings

# 📬 Contact Me

**Email**

[Awaleiabdi@outlook.com](mailto:Awaleiabdi@outlook.com)

**LinkedIn**

https://www.linkedin.com/in/awale-abdi
