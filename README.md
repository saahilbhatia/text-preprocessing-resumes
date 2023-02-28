# text-preprocessing-resumes
## Description
This notebook preprocesses a set of resume files and generates a sparse representation of the resumes. The dataset contains 250 resumes, which includes information of the applicants like contact details, skills, work experience, educational background, hobbies, etc.

The resumes containting the information of the applicants were loaded and any duplicate resumes were excluded from the analysis. Text pre-processing was performed on the resume files in the dataset. The pre-processing included case normalization, tokenization, removal of stopwords and stemming. Additionally, the most frequent and rare tokens were removed, the tokens with length less than 3 were removed, and the first 200 meaningful bigrams were added to the vocabulary. The capital tokens appearing in the middle of a sentence/line were not normalized to lower case because of the hypothesis that these tokens are likely to have a different meaning than their lower case counterparts.

The notebook concludes with the generation of the lexical vocabulary and the count vector sparse representations of the resumes. The vocabulary and vector representations are written to files, which can be used as input to various recommender-systems and information retrieval algorithms.

## Packages required
* nltk (https://pypi.org/project/nltk/)
* numpy (https://pypi.org/project/numpy/)
