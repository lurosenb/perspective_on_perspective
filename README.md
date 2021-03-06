# Selected Adversarial SemanticS (SASS)

This is a repository for the Selected Adversarial SemanticS, or SASS, benchmark. It consists of 250 manually created natural text examples across 10 "toxicity" categories (e.g. stereotyping, classism, blackmail). For each category, the benchmark contains 15 "filtered" and 10 "unfiltered" examples, drawing inspiration from  [Lin et. al.,2021](https://arxiv.org/abs/2109.07958). Eight of SASS's categories are aimed at generating "False Negative" scores, one category is aimed at "False Positive" scores and one category is "Neutral". The examples are designed specifically to challenge toxicity detection models like Perspective API. 


# Benchmarking with SASS

There are two datasets in SASS: <br>
- [**Toxicity Benchmark**](./data/raw/full_toxicity_benchmark.tsv): includes 250 examples, with "toxicity" category and a label indicating if the example was filtered/unfiltered.
- [**Human Toxicity Scores**](./data/processed/norm_human_toxicity_scores.csv): "human" toxicity score [0,1] for each example. The results included are the average of three anotators. Before averaging we perfomed a z-normalization.  
