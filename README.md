# Uncovering Phenotypes in Sensorineural Hearing Loss: A Systematic Review of Unsupervised Machine Learning Approaches

This repository contains the data and code used for the systematic review on the phenotyping of sensorineural hearing loss (SNHL). The project includes the data generated during the search and review process, as well as the code books used for analysis. The systematic review was undertaken primarily by three reviewers (Lilia Dimitrov, R1; Liam Barrett, R2; Nishchay Mehta, R3).

## Repository Structure

The repository is organized into the following directories and files:

```
├── data/  
│   ├── search_returns/  
│   │   ├── base.csv  
│   │   ├── cinahl.csv  
│   │   ├── github.csv  
│   │   ├── ieee.csv  
│   │   ├── medline.csv
│   │   ├── embase.csv
│   │   ├── psychinfo.csv
│   │   ├── scopus.csv
│   │   └── pubmed_abstracts.txt
│   ├── tiab/
│   │   └── all_results_deduplicated.csv
│   ├── responses/
│   │   ├── LD_response_complete.csv
│   │   ├── LB_response_complete.csv
│   │   └── full_text_reviews.csv
│   ├── appraise-ai/
│   │   ├── APPRAISE-AI (scoring form)-LD.xlsx
│   │   └── APPRAISE-AI (scoring form)-LB.xlsx
│   └── README.md
├── notebooks/
│   ├── search_preproc.ipynb
│   ├── stage_2_title_abstract_screening.ipynb
│   ├── inter_rater_reliabilities.ipynb
│   └── README.md
├── search_results.md
├── third_reviewer_responses.md
├── README.md
└── LICENSE
```

### Directories and Files
For both the `data` and `notebooks` directories, please seee the `README.md` files in each directory for further infomation on the files.

- **search_results.md**: File detailing the search terms input to the databases and the number of retrieved articles.
- **third_reviewer_responses.md**: File detailing where R1 and R2 disagreed during the review process and R3's final decision.
- **README.md**: This file, providing an overview of the project and its structure.
- **LICENSE**: The license for the project, detailing the terms of use.

## How to Use
1. **Data Cleaning**: Use the `search_preproc.ipynb` script to group all search results and drop duplicates. This generates the dataset ready for Title-Abstract review (`all_results_deduplicated.csv`).
2. **Title-Abstract Review**: Use the `stage_2_title_abstract_screening.ipynb` to demo how title-abstract screening was performed by R1 and R2. This generates a responses file for each reviewer which can be used to check for a.) conflicts and b.) inter-rater reliabilites
3. **Inter-rater reliabilities**: Use `inter_rater_reliabilities.ipynb` to reperform the statistical analyses ran to estimate inter-rater reliability for title-abstract screening and full-text review.

## Contact

For any questions or issues, please open an issue in the repository or contact the project maintainers.

Thank you for using the Dimitrov-Systematic-SNHL-Phenotyping repository!
