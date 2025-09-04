# Google Sentiment Analysis: Examining Search Bias in Political Topics

## Overview

This project analyzes Google search bias using sentiment analysis across 100+ political topics. Our research reveals consistent non-neutral patterns in search results, showing a lean toward Progressive (58.7%) and Collectivist (59.6%) viewpoints. This data-driven approach demonstrates how search algorithms subtly influence information discovery on controversial political issues.

## 🔍 Research Question

**"Does Google return search results that are biased for controversial political topics?"**

Our analysis examines whether Google's search algorithm exhibits systematic bias when presenting information on politically sensitive subjects.

## 📊 Key Findings

- **Progressive Bias**: 58.7% of analyzed topics show progressive-leaning results
- **Collectivist Bias**: 59.6% of topics lean toward collectivist viewpoints
- **Topic Variation**: Bias levels vary significantly across different political subjects
- **Consistent Patterns**: Non-neutral sentiment patterns appear across multiple controversial topics

## 🗂️ Dataset

The project includes comprehensive data collection across various political topics including:

### Political Issues Analyzed
- **Electoral Politics**: Trump/Biden voting preferences, mail-in ballots, voter ID laws
- **Gun Policy**: Gun control, background checks, concealed carry, assault weapon bans
- **Healthcare**: Universal healthcare, prescription costs, rural healthcare investment
- **Social Issues**: Abortion rights, LGBTQ+ education, affirmative action
- **Economic Policy**: Tax policy, universal income, student loan debt
- **Immigration**: DACA, asylum policies, sanctuary cities/states
- **Criminal Justice**: Police reform, racial bias, defunding initiatives
- **Environmental Policy**: Climate change education, environmental regulations
- **International Relations**: NATO, China, Iran, Israel/Palestine conflict

### Data Files Structure
- **Individual Topic Files**: 80+ CSV files for specific political questions
- **Aggregated Data**: `bipolar-topics.csv`, `questionScores.csv`
- **Sentiment Lexicon**: `AFINN-en-165.csv` for sentiment scoring
- **Analysis Notebook**: `Project3.ipynb` containing full methodology

## 🛠️ Methodology

### Sentiment Analysis Approach
1. **Data Collection**: Automated scraping of Google search results for political queries
2. **Sentiment Scoring**: Using AFINN-165 lexicon for sentiment quantification
3. **Bias Classification**: Categorizing results as Progressive/Conservative and Individualist/Collectivist
4. **Statistical Analysis**: Aggregating sentiment scores across topics and categories

### Tools & Technologies
- **Python**: Primary analysis language
- **Jupyter Notebook**: Interactive analysis environment
- **AFINN Sentiment Analysis**: Standardized sentiment scoring
- **CSV Data Processing**: Structured data storage and analysis

## 📈 Results Analysis

The analysis reveals systematic patterns in Google search results:

- **Non-neutral baseline**: Results consistently deviate from neutral sentiment
- **Progressive tendency**: Majority of topics show left-leaning result compilation
- **Collectivist preference**: Search results favor community-oriented over individual-focused perspectives
- **Topic sensitivity**: Bias magnitude varies based on political controversy level

## 🚀 Getting Started

### Prerequisites
```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Running the Analysis
1. Clone the repository:
```bash
git clone https://github.com/AnthonyMerlinGoHokies/Google-Sentiment-Analysis.git
cd Google-Sentiment-Analysis
```

2. Open the Jupyter notebook:
```bash
jupyter notebook Project3.ipynb
```

3. Run all cells to reproduce the analysis

### Data Structure
- Each CSV file contains search results for specific political queries
- `questionScores.csv` provides aggregated sentiment scores
- `AFINN-en-165.csv` contains the sentiment scoring lexicon

## 💻 Technical Implementation Details

### Core Functions
- `googleSearchLinks()`: Scrapes Google search results and extracts article URLs
- `getArticle()`: Extracts clean text from article URLs using regex parsing
- `sentimentAnalysis()`: Applies AFINN-165 sentiment scoring to article text
- `queryDataDictionary()`: Organizes scraped data by topic/question
- `clusterAnalysis()`: Performs K-means clustering on TF-IDF matrices
- `applyAxes()`: Maps sentiment scores to political ideology dimensions

### Visualization Functions
- `create_divergent_bar()`: Generates positive/negative sentiment bar charts
- `create3DPoliticalScatter()`: 3D political compass visualization with clustering
- `politicalPieCharts()`: Distribution charts for political axis preferences
- `articlePieCharts()`: Article sentiment distribution analysis

### Data Processing Pipeline
1. **Query Generation**: Load topics and questions from CSV files
2. **Web Scraping**: Automated Google search and article extraction
3. **Text Cleaning**: Remove HTML, normalize text, filter by length
4. **Sentiment Calculation**: Apply lexicon-based scoring
5. **Political Mapping**: Transform sentiment into political axis scores
6. **Clustering**: Group similar topics using text similarity
7. **Visualization**: Generate comprehensive analysis charts

## 🔬 Research Implications

This research contributes to understanding:
- **Algorithmic Bias**: How search algorithms may unconsciously influence information access
- **Information Asymmetry**: Potential impacts on democratic discourse and opinion formation
- **Search Engine Responsibility**: Questions about platform neutrality in information presentation
- **Methodological Framework**: Reproducible approach for analyzing search result bias

## 📊 Reproducibility

All data, code, and methodology are provided for full reproducibility. The analysis can be extended to:
- Additional political topics
- Different time periods
- Alternative search engines
- Cross-cultural comparisons

## 🤝 Contributing

Contributions are welcome! Areas for expansion:
- Additional political topics
- Temporal bias analysis
- International search engine comparisons
- Alternative sentiment analysis methods

## 📄 License

This project is available for academic and research purposes. Please cite appropriately if used in academic work.

## 📞 Contact

**Author**: Anthony Merlin  
**Institution**: Virginia Tech  
**Repository**: [Google-Sentiment-Analysis](https://github.com/AnthonyMerlinGoHokies/Google-Sentiment-Analysis)

---

*This research aims to promote transparency in information systems and contribute to discussions about algorithmic fairness in search technologies.*
