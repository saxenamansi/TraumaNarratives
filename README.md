# TraumaNarratives
**Title:** 
Understanding Trauma Narratives on Social Media Platforms

On social media, victims of domestic and sexual violence share their narratives. Such narratives can benefit victims by redefining their identity and receiving support from external sources. 

**Problem Statement:**
We address two aspects of such narratives: (1) identifying causal relationships between narrative elements and (2) analyzing the effect of such elements on social support received. This dataset contains personal stories, hence will be shared only to accredited researchers upon request. 

**Data Collection:** 
We extract 5561 victim narratives from Reddit, a popular online platform for support seeking, from the subreddits r/domesticviolence, r/MeToo, r/sexualassault and r/SexualHarassment. 

**Methodology:**
We leverage LLM prompting to perform feature extraction on these narratives. These features are used for our computational approach. 
We then use a Zero-inflated Model to analyze the effect of such features on social support received, and a Directed Acyclic Graph (DAG) to identifying causal effect relationships between narrative elements. 

**Findings:**
To be added. 

Published at the 17th ACM Web Science Conference 2025. Link of the paper will be added soon. 

Contents of this repository:

1. DownloadingData.ipynb: code to download Reddit Archival Data.
2. FilteringPosts.ipynb: Python code to filter posts to retain only those posts made by the victim.
3. SelectedWords.html: Words selected for filtering posts and retain only first-person narratives written by victims. 
4. FeatureExtraction_LLM.ipynb: Python code to extract narrative elements using prompting engineering with Llama 3.1 8B Instruct Mode.
5. ZIPModel.Rmd: R Code to extract feature having highest influence on number of comments using a Zero-inflated Poisson Model
6. CausalEffects.Rmd: R Code to find causal relationships between narrative elements using a Directed Acylic Graph (DAG)
7. CausalEffectResultScores.pdf: Causal Effect results of all causal models, i.e., (cause-effect pairs) we hypothesized, quantified by Z-scores and p-values.
8. NarrativeFeatureDescriptions.pdf: A description of all the trauma narrative features used in this project.
9. DAG.pdf: The hypothesized directed acyclic graph used for the Causal Models. 
