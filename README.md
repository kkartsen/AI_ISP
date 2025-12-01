# AI Bias Mitigation Repository
This document contains an executive summary of the project and a description of each of the files included in the repository.
This project earned an A grade and was completed for 1/6 additional undergraduate credit units in WPI's Introduction to Artificial Intelligence course (worth 1/3 undergraduate credit units), 
bringing the total credits earned for the course to 1/2 undergraduate credits, equivalent to 3 graduate credit-hours.
The credit earned from this ISP (Independent Study Project) and the corresponding course fulfill the "Artificial Intelligence" bin requirement of the Artificial Intelligence MS degree.

  ## Executive Summary
  The purpose of this study was to determine the effectiveness of different bias mitigation strategies for reducing the impact of bias in data. 
  This study was conducted through the implementation of the exponentiated gradient in-process bias mitigation strategy on a decision tree machine learning model when trained on the UCI Adult Income dataset. 
  Bias was measured using the fairness metrics of demographic parity and equalized odds. 
  To produce comprehensive results, these metrics were evaluated both with and without implementing the bias mitigation techniques for three datasets with varying degrees of bias and across both race and gender demographic categories.
  Findings show that mitigating the demographic parity for the targeted demographic tends to produce optimal results, but considerations must be taken for the degree of bias within the dataset and trade-offs with other fairness metrics, as well as accuracy.

  ## Files
<!-- TOC -->
* [AI_Bias_Mitigation_ISP.ipynb](https://github.com/kkartsen/AI_ISP/blob/main/AI_Bias_Mitigation_ISP.ipynb)
  * Project code and documentation formatted as a Jupyter Notebook file.
  * This file in GitHub also contains a link to the [Google Colab](https://colab.research.google.com/drive/1SBVvw_QjsstotJUoRgrwwl3DsxCA1vOt#scrollTo=W4pRGVGdGyHM), which is where the original project was written and which is formatted most optimally.
* [ai_bias_mitigation_isp.py](https://github.com/kkartsen/AI_ISP/blob/main/ai_bias_mitigation_isp.py)
  * Project code and documentation formatted as a Python file.
* [AI ISP Timeline.pdf](https://github.com/kkartsen/AI_ISP/blob/main/AI%20ISP%20Timeline.pdf)
  * Timeline of work to be done and deliverables, created upon approval of project proposal. ChatGPT was used to provide input on task breakdowns and completion time.
  * This timeline is mostly accurate to the actual progression of work, with a few exceptions:
    * Both more-biased and less-biased versions of the original dataset were created, tested, and evaluated; instead of only one modified dataset version.
    * During Week 3, additional time was spent converting calculations for predictive parity to equalized odds. This was done mainly to align evaluated fairness metrics more closely with the in-process bias mitigation technique targets included with the fairness library I used. The available targets included equalized odds, but not predictive parity.
    * A written report was added as a final deliverable along with the Jupyter Notebook.
    * Some tasks took more or less time than predicted.
* [ISP Final Report.pdf](https://github.com/kkartsen/AI_ISP/blob/main/ISP%20Final%20Report.pdf)
  * Written report detailing the project goals, methods, and results.
  * Sections include:
    * Executive Summary
    * Methods
      * Preparing the dataset
      * Altering bias in the dataset
      * Training the model
      * Evaluating the predictions for each model
      * Implementing bias mitigation techniques
      * Evaluating the model predictions after bias mitigation
    * Results
    * Interpretations
    * Generative AI use
    * Glossary
    * Sources Used
