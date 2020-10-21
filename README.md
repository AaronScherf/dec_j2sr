# Trial effort to link DEC final evaluation reports with the following:
# J2SR Roadmap Metrics, FAE disbursement and obligation data


## Process for replication:

1. Download DEC evaluation reports from API (url) using the following query: (query tbd)
2. Download J2SR metrics from IDEA query tool using the following filters: (filters tbd)
3. Download FAE budget data from FAE download tool
3. Process and join datasets using DEC_J2SR_Join.ipynb
4. Results in dec_j2sr_data.csv
5. This base file can then be used for the following analyses:
6. DEC_Keyword_Analysis.ipynb groups DEC tags into clusters using k-modes
7. FAE_Join.ipynb links the combined DEC_J2SR data with budget data from Foreign Aid Explorer
8. text_extract.ipynb extracts text from PDF files in the DEC and creates summary files for the executive summary
