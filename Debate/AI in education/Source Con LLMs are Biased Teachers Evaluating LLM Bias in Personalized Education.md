Title: LLMs are Biased Teachers: Evaluating LLM Bias in Personalized Education
Link: https://arxiv.org/abs/2410.14012
Citation:
> [!note] Citation
> ## Weissburg et al. 2024
> Weissburg, Iain, Sathvika Anand, Sharon Levy, and Haewon Jeong. “LLMs Are Biased Teachers: Evaluating LLM Bias in Personalized Education.” arXiv, October 17, 2024. [https://doi.org/10.48550/arXiv.2410.14012](https://doi.org/10.48550/arXiv.2410.14012).

# Abstract
With the increasing adoption of large language models (LLMs) in education, concerns about inherent biases in these models have gained prominence. We evaluate LLMs for bias in the personalized educational setting, specifically focusing on the models' roles as "teachers". We reveal significant biases in how models generate and select educational content tailored to different demographic groups, including race, ethnicity, sex, gender, disability status, income, and national origin. We introduce and apply two bias score metrics--Mean Absolute Bias (MAB) and Maximum Difference Bias (MDB)--to analyze 9 open and closed state-of-the-art LLMs. Our experiments, which utilize over 17,000 educational explanations across multiple difficulty levels and topics, uncover that **models perpetuate both typical and inverted harmful stereotypes**.

# Some interesting stuff

![[Pasted image 20241101225133.png]]

5.1 RQ1: Bias in Educational Text Selection
Our analysis of the ranking experiments reveals significant biases across all demographic subgroups when LLMs select educational texts. We observe consistent patterns across different datasets for each model, suggesting that these biases are inherent in
the models’ decision-making processes.

Stereotype and Reverse Bias. Within subgroups, biases manifest as either (a) stereotype bias, which perpetuates generally held stereotypes, or (b) reverse bias, which contradicts them. This phenomenon has been studied in previous work (Ganguli et al., 2023; Hofmann et al., 2024). We note that both types of bias are harmful in our setting.

As shown in Figure 2a, both types of bias can manifest for a single model and dataset. For example, in the Sex/Gender subgroup, we observe alignment with common stereotypes: “female” students are scored significantly lower than “male.” In contrast, the Disability subgroup reverses the stereotype (Gupta et al., 2023): “physically disabled” and “neurodivergent” students are scored higher than “able-bodied” and “neurotypical” ones.

Overall Patterns. Across all datasets and models, we find statistically significant bias in how LLMs assign educational content to different demographic groups. The Friedman test results (p < 0.001 for all subgroups)6 indicate that these differences are unlikely to occur by chance.

For the primary models listed in Section 4.4, we observe the following overall patterns in ranking, with some variation depending on dataset. For Gemini 1.5 Pro and Llama 3.1 405B, we observe reverse biases across all subgroups. For GPT 4o (Figure 2a), we observe reverse biases in the Disability subgroup, while the results for Race/Ethnicity, Sex/Gender, and Religion are neither fully stereotypical nor reverse biased (e.g. male is scored higher than female, but not highest overall).

![[Pasted image 20241101225345.png]]

Bias chart for GPT4o

GPT4o has many biases:
- Recommended higher-level sources for physically disabled and neurodivergent people and lower-level sources for able-bodied people
- Recommended higher-level sources for  Christians, Muslims, Jewish, and Hindu, while recommending lower-level sources for agnostic people
- Recommending lower-level sources for low-income people while recommending higher-level sources for middle-income people. 