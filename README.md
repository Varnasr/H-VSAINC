# Hyderabad Electoral Analysis (1999-2023)

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Data: Election Commission](https://img.shields.io/badge/Data-Election%20Commission-blue.svg)](https://eci.gov.in/)

Interactive analysis of Hyderabad District Assembly Elections spanning 24 years (1999-2023): Vote share trends, party performance metrics, and constituency-level political economy insights.

## 📊 Overview

This repository provides a comprehensive quantitative analysis of electoral patterns in Hyderabad District across six assembly election cycles (1999, 2004, 2009, 2014, 2018, and 2023). The analysis covers five constituencies: Bahadurpura, Chandrayangutta, Charminar, Malakpet, and Yakutpura, tracking vote share dynamics for major political parties including AIMIM, INC, BJP, TRS/BRS, TDP, and MBT.

### Key Features

- **Interactive HTML Dashboard**: Self-contained, single-file report with responsive visualizations
- **Comprehensive Data Analysis**: 27 data points across 6 parties and 5 constituencies
- **Statistical Metrics**: Volatility analysis, growth rates, and comparative performance indicators
- **Export Capabilities**: PDF, PNG (charts), and CSV (data tables) export functionality
- **Political Economy Interpretation**: Contextual analysis of electoral dynamics and party systems

## 🎯 Research Questions Addressed

1. How have party vote shares evolved across Hyderabad constituencies over 24 years?
2. What patterns of electoral dominance, competition, and realignment are observable?
3. How do constituency-specific factors influence party performance?
4. What is the trajectory of emerging political forces (BJP, TRS/BRS) in the region?
5. How does vote share volatility vary across parties and constituencies?

## 📁 Repository Structure

```
hyderabad-electoral-analysis/
├── data/
│   ├── HYD-DIST-RESULTS.csv                    # Primary election data
│   └── Hyderabad-INC-VoteShare-1999-2023.docx  # Supplementary analysis
├── outputs/
│   └── Hyderabad_Electoral_Analysis_Report.html # Interactive report
├── .gitignore
├── LICENSE
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Modern web browser (Chrome, Firefox, Safari, or Edge)
- No installation required - the report is a self-contained HTML file

### Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Varnasr/hyderabad-electoral-analysis.git
   cd hyderabad-electoral-analysis
   ```

2. **Open the report:**
   - Simply open `outputs/Hyderabad_Electoral_Analysis_Report.html` in your web browser
   - Or double-click the file to launch it

3. **Export functionality:**
   - **PDF**: Click "Export Full Report to PDF" button (uses browser print)
   - **PNG**: Each chart has an individual PNG export button
   - **CSV**: Export complete dataset or individual tables

## 📈 Data Sources

- **Primary Source**: Election Commission of India (constituency-level results)
- **Time Period**: 1999-2023 (6 election cycles)
- **Geographic Scope**: Hyderabad District, Telangana
- **Variables**: Party-wise vote share percentages for each constituency and year

### Data Notes

- Empty cells indicate party did not contest in that constituency/year
- Vote shares are expressed as percentages of total valid votes
- The 2004 Malakpet anomaly (INC: 52.12%) occurred due to AIMIM not fielding a candidate

## 🔍 Key Findings

### Electoral Dominance
- **AIMIM** maintains consistent electoral superiority with vote shares ranging from 30-78%
- Particularly strong in Bahadurpura (78.46% in 2014) and Charminar constituencies

### Party Trajectories
- **BJP**: Significant growth from marginal presence (1999) to competitive positions (15-27% in 2023)
- **TRS/BRS**: Emerged as significant player post-2014, particularly in Bahadurpura and Yakutpura
- **TDP**: Systematic decline from competitive positions to marginal presence
- **INC**: Variable performance with notable constituency-specific patterns

### Constituency Dynamics
- **Bahadurpura**: AIMIM fortress (62-78% vote share)
- **Charminar**: Most competitive; BJP emerging as strong challenger
- **Malakpet**: Highest volatility; multi-party competition
- **Yakutpura**: AIMIM showing recent vulnerability (decline from 57% to 33%)
- **Chandrayangutta**: Consistent AIMIM dominance with growing BJP-TRS challenge

## 📊 Methodology

### Analytical Approach
- **Descriptive Statistics**: Mean, median, standard deviation of vote shares
- **Trend Analysis**: Time-series examination of party performance
- **Volatility Metrics**: Standard deviation as measure of electoral stability
- **Comparative Analysis**: Constituency-level and party-level cross-sectional comparisons
- **Growth Rate Analysis**: Period-over-period changes (1999 vs 2023)

### Visualization Techniques
- Line charts for temporal trends
- Bar charts for comparative analysis
- Grouped visualizations for multi-party competition
- Color-coded party identification for clarity

## 🛠️ Technical Stack

- **Data Processing**: JavaScript (native)
- **Visualization**: Chart.js v4.4.0
- **Export Functions**: html2canvas, jsPDF
- **Styling**: Custom CSS with responsive design
- **Format**: Self-contained HTML (no external dependencies required at runtime)

## 📚 Academic Context

This analysis contributes to understanding:
- **Electoral Geography**: Urban voting patterns in Indian metropolitan constituencies
- **Party Systems**: Dominant party systems and multi-party competition dynamics
- **Political Economy**: Identity politics, regional dynamics, and national party performance in local contexts
- **Voter Behavior**: Vote bank stability, swing patterns, and electoral volatility

## 🤝 Contributing

Contributions are welcome! Areas for enhancement:
- Additional statistical tests (e.g., regression analysis, correlation matrices)
- Demographic overlay analysis
- Comparison with other metropolitan constituencies
- Predictive modeling for future elections
- Interactive filters and drill-down capabilities

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📧 Contact

**Varna Sri Raman**  
Pinpoint Ventures  
Development Economist

For questions, suggestions, or collaborations:
- Open an issue in this repository
- Connect via GitHub: [@Varnasr](https://github.com/Varnasr)
- Academic inquiries welcome

## 🙏 Acknowledgments

- Election Commission of India for public data availability
- Political analysts and researchers whose work informs this analysis
- Open-source community for visualization and analysis tools

## 📖 Citation

If you use this analysis in your research, please cite:

```bibtex
@misc{hyderabad_electoral_2024,
  title={Hyderabad Electoral Analysis 1999-2023: Vote Share Trends and Political Economy Insights},
  author={Raman, Varna Sri},
  year={2024},
  publisher={GitHub},
  organization={Pinpoint Ventures},
  url={https://github.com/Varnasr/hyderabad-electoral-analysis}
}
```

---

**Note**: This is an independent academic analysis. Vote share data is based on official Election Commission results. Interpretations and analysis represent scholarly assessment of electoral patterns.
