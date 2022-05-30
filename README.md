# Capstone Project

## Abstract
Several studies have shown language used in scientific literature is different from general language. However, the linguistic differences in specific discipline with general language remains a question. This study aims to compare the scientific language across disciplines with a neutral baseline (newspaper) to investigate the differences in the language used in each domain.  The goal of this study is to explore how scientists communicate with each other and how they communicate with the public. It measures the linguistic differences using the information-theoretic measure and cosine similarity with the term frequency-inverse document frequency. The two methods have similar results, showing that the language of disciplines in sciences is the most dissimilar from newspapers, followed by social sciences and humanities. The findings of this investigation reveal that science might be the most difficult for the general public and scientists in other professions to comprehend. However, the essay in social sciences and humanities might be more easily understood by the public since their language is more similar to newspaper articles. This study provides insight into the hierarchy of science in terms of information theory. 

## Dataset
The capstone utilised two datasets. The first dataset is The Semantic Scholar Open Research Corpus ([S2ORC](https://github.com/allenai/s2orc)). The second dataset is CC-News. You need to request access to dowload S2ORC datasets. You can load CC_News directly with the datasets library. 
```properties
from datasets import load_dataset
dataset = load_dataset("cc_news")
``` 
## Documentation
  * Preprocess.ipynb The code to preprocess the CC_News dataset into a list of tokens and lower all the tokens. 
  * S2ORC.ipynb The notebook to read the S2ORC files and pereprocess all scientific papers into list of tokens across each discpline.
  * Lemma_KLD.ipynb The code to convert a list of tokens into probability distribution and measure the KL Diverence for news compared with discplines and discplines compared with news at lexical level. Plot the distribution graph in the file.
  * pos_process.ipynb The notebook measures the KL Divergence at grammatical level. 
  * cosine.ipynb The notebook measures the cosine similarity between the disciplines with the news.
  * graph.ipynb Plot the KL Divergence graphs for each discpline and domains. 
  * distribution folder contains all plots about the distribution of KL Divergence
  * plot folder contains all other graphs including average KL Divergence and WordCloud. 
