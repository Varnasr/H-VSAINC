# Data Documentation

## Overview

This folder contains electoral data for Hyderabad District Assembly Elections spanning 1999-2023. Data includes constituency-level vote share percentages for major political parties across six election cycles.

## File Descriptions

### HYD-DIST-RESULTS.csv

Primary dataset containing election results.

**Format**: CSV (Comma-Separated Values)  
**Size**: ~1.5 KB  
**Records**: 27 rows (excluding header)  
**Time Period**: 1999-2023  
**Update Frequency**: Post-election (every 5 years typically)

### Hyderabad-INC-VoteShare-1999-2023.docx

Supplementary analysis document providing context on INC performance patterns, specifically noting the 2004 Malakpet anomaly.

**Format**: Microsoft Word Document  
**Size**: ~240 KB  
**Content**: Textual analysis and contextual notes

## Data Dictionary

### HYD-DIST-RESULTS.csv

| Variable | Description | Data Type | Range/Values | Missing Values |
|----------|-------------|-----------|--------------|----------------|
| YEAR | Election year | Integer | 1999, 2004, 2009, 2014, 2018, 2023 | None |
| ACNAME | Assembly Constituency name | String | See constituency list below | None |
| AIMIM_VoteShare | All India Majlis-e-Ittehadul Muslimeen vote share | Float | 0-100 (percentage) | When party did not contest |
| TDP_VoteShare | Telugu Desam Party vote share | Float | 0-100 (percentage) | When party did not contest |
| MBT_VoteShare | Majlis Bachao Tehreek vote share | Float | 0-100 (percentage) | When party did not contest |
| INC_VoteShare | Indian National Congress vote share | Float | 0-100 (percentage) | When party did not contest |
| BJP_VoteShare | Bharatiya Janata Party vote share | Float | 0-100 (percentage) | When party did not contest |
| TRS_VoteShare | Telangana Rashtra Samithi (now BRS) vote share | Float | 0-100 (percentage) | When party did not contest |

### Constituencies

The dataset covers the following Assembly Constituencies (AC) in Hyderabad District:

1. **Bahadurpura** (available from 2014 onwards)
2. **Chandrayangutta**
3. **Charminar**
4. **Malakpet**
5. **Yakutpura**

**Note**: Bahadurpura constituency was created after delimitation and appears in data from 2014 onwards.

## Data Sources

### Primary Source
**Election Commission of India (ECI)**  
Official Website: https://eci.gov.in/  
Statistical Reports: State Assembly Election Results

### Access Method
- Official ECI statistical reports
- State Election Commission, Telangana
- Public domain electoral data

### Collection Date
Data compiled: October 2024  
Last election data: 2023 Assembly Elections

### Verification
All data cross-referenced with:
- Official ECI press releases
- State Election Commission reports
- Media reports from reputable sources (as secondary validation)

## Data Processing Notes

### Missing Values
- Empty cells or null values indicate the party did not field a candidate in that constituency for that election year
- This is a structural feature, not a data quality issue

### Known Anomalies

#### 2004 Malakpet - AIMIM Absence
**Observation**: INC achieved 52.12% vote share in Malakpet (2004)  
**Context**: AIMIM did not contest this constituency in 2004  
**Implication**: INC vote share represents temporary consolidation rather than baseline performance  
**Source**: Supplementary analysis document

### Data Limitations

1. **Vote Share Only**: Dataset contains vote share percentages, not absolute vote counts
2. **Major Parties Only**: Includes only 6 major parties; "Others" category not captured
3. **Constituency Boundaries**: May not reflect boundary changes across years
4. **Turnout Data**: Voter turnout percentages not included in this dataset
5. **Candidate Information**: Individual candidate names and details not included

## Data Quality

### Accuracy
- ✓ Cross-verified with official sources
- ✓ Calculations checked for consistency
- ✓ Anomalies documented and explained

### Completeness
- 6 election years covered
- 5 constituencies (Bahadurpura from 2014)
- 6 major political parties
- Some missing values due to non-contestation (expected)

### Consistency
- Uniform format across all years
- Consistent variable naming
- Standardized percentage representation

## Usage Notes

### Analysis Considerations

1. **Missing Values**: When analyzing trends, account for structural missingness (party non-contestation)
2. **Baseline Comparisons**: The 2004 Malakpet anomaly should be treated separately in trend analysis
3. **Party Name Changes**: TRS became BRS in 2022, but data retains "TRS" label for consistency
4. **Delimitation Effects**: Bahadurpura's creation in 2014 affects temporal comparisons

### Recommended Analyses

- Time series analysis of party vote shares
- Constituency-level comparative analysis
- Volatility and stability metrics
- Growth rate calculations
- Multi-party competition indices

### Citation

When using this data, please cite:

```
Raman, Varna Sri (2024). Hyderabad Electoral Analysis Dataset (1999-2023). 
Pinpoint Ventures. Available at: https://github.com/Varnasr/hyderabad-electoral-analysis
Data source: Election Commission of India.
```

## Updates and Versions

### Version History

- **v1.0** (October 2024): Initial dataset covering 1999-2023
- Future versions will incorporate subsequent election results

### Update Schedule

This dataset will be updated following each Telangana Assembly Election (typically every 5 years).

## Contact

For questions about the data:
- Open an issue on GitHub: https://github.com/Varnasr/hyderabad-electoral-analysis/issues
- Tag with "data" label

For data corrections or additions:
- Submit a pull request with documentation
- See CONTRIBUTING.md for guidelines

## License

The electoral data itself is in the public domain as official government records. The compilation, organization, and supplementary analysis are licensed under MIT License (see repository LICENSE file).

---

**Data Documentation Version**: 1.0  
**Last Updated**: October 2024  
**Maintained by**: Varna Sri Raman, Pinpoint Ventures
