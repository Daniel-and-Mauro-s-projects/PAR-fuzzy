# Fuzzy Expert System to Detect Phishing in Websites

**Authors:** Dániel MÁCSAI, Ismael RUIZ GARCÍA, Mauro VÁZQUEZ CHAS  
**Master in Artificial Intelligence - Planning and Approximate Reasoning**  
**Delivery 3 - 15th December 2024**

## Overview
This project presents a fuzzy expert system for detecting phishing websites. Using fuzzy logic, the system evaluates websites based on URL characteristics, content analysis, and external features. The result is a classification of the website’s phishing risk, ranging from safe to phishing.

## Linguistic Variables
The system uses fuzzy variables derived from three categories of features:

- **URL-Based Features:** Phish Hints (suspicious words in URL), Domain Age
- **Content Features:** Ratio of External Hyperlinks
- **External Features:** Google Index, Google Toolbar Rank (GTR)

## Fuzzy Rules
The system uses a set of rules based on the selected features to classify the phishing risk. For example:
- A website with a high ratio of external hyperlinks and a low GTR is more likely to be phishing.
- A new domain with numerous external links raises the phishing risk.

## Implementation
The system is implemented in MATLAB using the **Mamdani fuzzy inference method**. The Fuzzy Logic Toolbox is used to define membership functions, fuzzy rules, and to perform the defuzzification process using the Center of Area (CoA) method.

## Testing
Test cases were created with both phishing and legitimate websites. The system successfully classified most websites, although a false positive was detected for a legitimate educational site.

## References
1. Ali Aljofey et al. “An effective detection approach for phishing websites using URL and HTML features” (2022).
2. Zuochao Dou et al. “Systematization of Knowledge (SoK): A Systematic Review of Software-Based Web Phishing Detection” (2017).
3. Abdelhakim Hannousse and Salima Yahiouche. “Towards benchmark datasets for machine learning-based website phishing detection” (2021).
