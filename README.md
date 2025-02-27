# TraumaNarratives
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

1. Downloading Data.ipynb: code to download Reddit Archival Data.
2. FilteringPosts.ipynb: Python code to filter posts to retain only those posts made by the victim.
3. SelectedWords.html:List of relevant words used for filtering posts. 
4. FeatureExtraction_LLM.ipynb: Python code to extract narrative elements using prompting engineering with Llama 3.1 8B Instruct Mode.
5. ZIP Model: R Code to extract feature having highest influence on number of comments using a Zero-inflated Poisson Model
6. Causal Effects Model: R Code to find causal relationships between narrative elements using a Directed Acylic Graph (DAG)
