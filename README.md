## Python & SAS – A Powerful Duo in Predicting Peanut Allergy
Summer 2024 Intern Expo project.

## Description
Combining power of open-source language (Python) and SAS Viya to aid in a data science project.
Cleaned data in Python.
Created machine learning models for prediction of peanut allergy in infants from clinical data (LEAP study) using SAS Model Studio and Python, compared/contrasted results.
Established CAS connection to SAS server in Python to run SAS ModelStudio generated score code.

## Installation

Python dependencies used:
- pandas
- numpy
- sklearn
- seaborn
- matplotlib.pyplot
- requests
- json
- os
- base64

Jupyer Notebooks were ran in VSCode.

Navigating this repository:
- In order to run final_data_prep_gl.ipynb, the Excel workbooks basophil_activation_gl.xlsx and primary_outcome_peanut_challenge_gl.xlsx must be downloaded and stored in the same directory, otherwise filenames/paths must be tweaked in the code.
- final_data_prep_gl.ipynb is used to produce the dataset final_data_cleaned.xlsx. This dataset is used to train and test the machine learning models found in peanut_ML_for_comparison_gl.ipynb.
- In order to run connect_to_SAS_gl.ipynb, the file score_code_LR_fwd_gl must be downloaded and its filepath must be specified in the connect_to_sas_gl.ipynb code.
- The scoring code automatically generated in connect_to_SAS_gl_ipynb requires some tweaks to run effectively. The modified version can be found in SAS_to_python_scorecode_modified_gl.ipynb.
- Open_source_node_LR_gl.ipynb and open_source_node_tree_gl.ipynb can be pasted into the Open Source Code node in SAS Model Studio (after moving it to the Supervised Learning category). They will run a Python logistic regression and decision tree, respectively. The results will appear in the Model Comparison node along with the SAS-generated models.

Note:
- You may notice all file names are followed by _gl. This is to distinguish the GitLab versions, which are commented to facilitate third-party use, from my personal versions.

## Support
Please email aklissouras@unc.edu with any questions or concerns.

## Authors and acknowledgment

Thank you to Christa Cody, PhD for her guidance and assistance in establishing project scope, debugging code, advice on best data science practices.

The code to establish a connection to the SAS server was found [here](https://rndconfluence.sas.com/display/SSE/SSEMonthly+Connections). <br />
The code to build the scoring code in python swat was found [here](https://github.com/sassoftware/sas-scoring-wrapper-python). <br />
Thank you to the contributors of the above code/instructions.


The [original datasets](https://www.itntrialshare.org/project/Studies/ITN032ADPUBLIC/Study%20Data/begin.view?pageId=study.DATA_ANALYSIS) are part of the LEAP study. <br />
Thank you to those involved in the LEAP study for their research contributions and data.

## References

1. Sever ML, Calatroni A, Roberts G, et al. Developing a Prediction Model for Determination of Peanut Allergy Status in the Learning Early About Peanut Allergy (LEAP) Studies. The Journal of Allergy and Clinical Immunology: In Practice. 2023;11(7):2217-2227.e9. doi:10.1016/j.jaip.2023.04.032<br />
2. Gryak J, Georgievska A, Zhang J, et al. Prediction of pediatric peanut oral food challenge outcomes using machine learning. Journal of Allergy and Clinical Immunology: Global. 2024;3(3):100252. doi:10.1016/j.jacig.2024.100252<br />
3. Cottel N, Saf S, Bourgoin-Heck M, et al. Two Different Composite Markers Predict Severity and Threshold Dose in Peanut Allergy. The Journal of Allergy and Clinical Immunology: In Practice. 2021;9(1):275-282.e1. doi:10.1016/j.jaip.2020.09.043<br />
4. Koplin JJ, Peters RL, Dharmage SC, et al. Understanding the feasibility and implications of implementing early peanut introduction for prevention of peanut allergy. Journal of Allergy and Clinical Immunology. 2016;138(4):1131-1141.e2. doi:10.1016/j.jaci.2016.04.011

