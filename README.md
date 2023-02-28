# Evaluation Papers for ChatGPT

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) ![](https://img.shields.io/github/last-commit/THU-KEG/EvaluationPaper4ChatGPT?color=green) ![](https://img.shields.io/badge/PRs-Welcome-red) 



### Introduction

This repository stores Dataset Resources, Evaluation Papers and Detection Tools or Tools for ChatGPT

* [0. Survey](#0-survey)
* [1. Dataset Resource](#1-dataset-resource)
* [2. Evaluation Papers](#2-evaluation-papers)
  * [2.1 Metrics](#21-metrics)
  * [2.2 Open-ended Generation](#22-open-ended-generation)
  * [2.3 Long Text Summarization](#23-long-text-summarization)
  * [2.4 Reasoning](#24-reasoning)
  * [2.5 MultiModal](#25-multimodal)
  * [2.6 Other Domains](#26-other-domains)
* [3. Detection Tools](#3-detection-tools)

## 0. Survey
1. **The Utility of ChatGPT as an Example of Large Language Models in Healthcare Education, Research and Practice: Systematic Review on the Future Perspectives and Potential Limitations.**

   *Malik Sallam.* [[pdf](https://www.medrxiv.org/content/medrxiv/early/2023/02/21/2023.02.19.23286155.full.pdf)], 2023.2


## 1. Dataset Resource

1. **How Close is ChatGPT to Human Experts? Comparison Corpus, Evaluation, and Detection.**

   *Biyang Guo,  Xin Zhang , Ziyuan Wang, Minqi Jiang , Jinran Nie, Yuxuan Ding, Jianwei Yue , Yupeng Wu.* [[abs](https://arxiv.org/abs/2301.07597)],[[github](https://github.com/Hello-SimpleAI/chatgpt-comparison-detection)], 2023.1

2. **ChatGPT: Jack of all trades, master of none.**

   *Jan Kocoń , Igor Cichecki , Oliwier Kaszyca , Mateusz Kochanek , Dominika Szydło , Joanna Baran, Julita Bielaniewicz, Marcin Gruza, Arkadiusz Janz, Kamil Kanclerz, Anna Kocoń, Bartłomiej Koptyra, Wiktoria Mieleszczenko-Kowszewicz, Piotr Miłkowski, Marcin Oleksy, Maciej Piasecki, Łukasz Radliński, Konrad Wojtasik, Stanisław Woźniak and Przemysław Kazienko.* [[abs](https://arxiv.org/abs/2302.10724)],[[github](https://github.com/CLARIN-PL/chatgpt-evaluation-01-2023)], 2023.2

3. **Can ChatGPT Understand Too? A Comparative Study on ChatGPT and Fine-tuned BERT.**

   *Qihuang Zhong, Liang Ding,  Juhua Liu, Bo Du, Dacheng Tao.* [[abs](https://arxiv.org/abs/2302.10198)],[[github](https://github.com/WHU-ZQH/ChatGPT-vs.-BERT)], 2023.2
   
4. **Is ChatGPT A Good Translator? A Preliminary Study.**

   *Wenxiang Jiao, Wenxuan Wang, Jen-tse Huang, Xing Wang, Zhaopeng Tu.* [[abs](https://arxiv.org/abs/2301.08745v2)],[[github](https://github.com/wxjiao/Is-ChatGPT-A-Good-Translator)], 2023.1
   

Data statistics of these resources:

|    Paper with Dataset | Task                          | #Examples
|----------------|-------------------------------|-----------------------------|
|How Close is ChatGPT to Human Experts? Comparison Corpus, Evaluation, and Detection|QA + Dialog           |40,000       |
|Can ChatGPT Understand Too? A Comparative Study on ChatGPT and Fine-tuned BERT          | sentiment analysis / Paraphrase / NLI         |475          |
|ChatGPT: Jack of all trades, master of none         | 25 classification/ QA/reasoning  task|38,000|
|Is ChatGPT A Good Translator? A Preliminary Study       | Translation|5,609|

 



## 2. Evaluation Papers


### 2.1 Metrics

#### Before ChatGPT, metrics using GPT3

1. **DetectGPT: Zero-Shot Machine-Generated Text Detection using Probability Curvature.**

   *Eric Mitchell, Yoonho Lee, Alexander Khazatsky, Christopher D. Manning, Chelsea Finn.* [[abs](https://arxiv.org/abs/2301.11305)],[[demo](https://detectgpt.ericmitchell.ai/)], 2023.1

2. **GPTScore: Evaluate as You Desire.**

   *Jinlan Fu, See-Kiong Ng, Zhengbao Jiang, Pengfei Liu.* [[abs](https://arxiv.org/abs/2302.04166)],[[github](https://github.com/jinlanfu/GPTScore)], 2023.2


### 2.2 Open-ended Generation

1. **Exploring AI Ethics of ChatGPT: A Diagnostic Analysis.**

   *Terry Yue Zhuo, Yujin Huang , Chunyang Chen , Zhenchang Xing.* [[abs](https://arxiv.org/abs/2301.12867)], 2023.2


### 2.3 Long Text Summarization
   
1. **Exploring the Limits of ChatGPT for Query or Aspect-based Text Summarization.**

   *Xianjun Yang, Yan Li, Xinlu Zhang, Haifeng Chen, Wei Cheng.* [[abs](https://arxiv.org/abs/2302.08081)], 2023.2

2. **Can ChatGPT Write a Good Boolean Query for Systematic Review Literature Search?**

   *Shuai Wang, Harrisen Scells, Bevan Koopman, Guido Zuccon.* [[abs](https://arxiv.org/abs/2302.03495)], 2023.2

### 2.4 Reasoning

1. **Mathematical Capabilities of ChatGPT.**

   *Simon Frieder, Luca Pinchetti, Ryan-Rhys Griffiths, Tommaso Salvatori, Thomas Lukasiewicz, Philipp Christian Petersen, Alexis Chevalier, Julius Berner.* [[abs](https://arxiv.org/abs/2301.13867)], 2023.1

2. **Is ChatGPT a General-Purpose Natural Language Processing Task Solver?**

   *Chengwei Qin, Aston Zhang, Zhuosheng Zhang, Jiaao Chen, Michihiro Yasunaga, Diyi Yang.* [[abs](https://arxiv.org/abs/2302.06476)], 2023.2


### 2.5 Multimodal

1. **A Multitask, Multilingual, Multimodal Evaluation of ChatGPT on Reasoning, Hallucination, and Interactivity.**

   *Yejin Bang, Samuel Cahyawijaya, Nayeon Lee, Wenliang Dai, Dan Su, Bryan Wilie, Holy Lovenia, Ziwei Ji, Tiezheng Yu, Willy Chung, Quyet V. Do, Yan Xu, Pascale Fung.* [[abs](https://arxiv.org/abs/2302.04023)], 2023.2




### 2.6 Other Domains

#### Education

1. **ChatGPT: Bullshit spewer or the end of traditional assessments in higher education?**

   *Jürgen Rudolph, Samson Tan, Shannon Tan.* [[pdf](https://journals.sfu.ca/jalt/index.php/jalt/article/download/689/539)], 2023.1
   
2. **Will ChatGPT get you caught? Rethinking of Plagiarism Detection**

   *Mohammad Khalil, Erkan Er.* [[abs](https://arxiv.org/abs/2302.04335)], 2023.2

 

#### Biology

1. **How Does ChatGPT Perform on the Medical Licensing Exams? The Implications of Large Language Models for Medical Education and Knowledge Assessment.**

   *Aidan Gilson, Conrad Safranek, Thomas Huang, Vimig Socrates, Ling Chi, R. Andrew Taylor, David Chartash.* [[pdf](https://www.medrxiv.org/content/10.1101/2022.12.23.22283901.full.pdf)], 2022.12


## 3. Detection Tools

1. [**GPTZero**](https://gptzero.me/): A demo to detect writings generated by ChatGPT. The creator has seen that the technology was used by students to cheat on assignments, so he came up with a safeguard. 
2. [**Hello-SimpleAI ChatGPT Detector**](https://hello-simpleai-chatgpt-detector-ling.hf.space/):  An open-source detection project consists of three versions of models to detect text generated with ChatGPT, including [QA version](https://huggingface.co/spaces/Hello-SimpleAI/chatgpt-detector-qa), [Sinlge-text version](https://huggingface.co/spaces/Hello-SimpleAI/chatgpt-detector-single) and [Linguistic version](https://huggingface.co/spaces/Hello-SimpleAI/chatgpt-detector-ling).
3. **[Contentatscale AI Content Detector](https://contentatscale.ai/ai-content-detector/)** : A tool that allows users to receive the Human or AI Content score in the text to detect. It provides probability for each sentence.
4. **[Writers AI Content Detector](https://writer.com/ai-content-detector/)**: A tool similar to Contentatscale. It requires either the URL of the page or text to calculate the “Human-Generated Content” score. 
5. **[OpenAI Classifier](https://openai.com/blog/new-ai-classifier-for-indicating-ai-written-text/)**: A classifier fine-tuned on a dataset of pairs of human-written text and AI-written text on the same topic.


Statistics of these tools:

|    Tool |  Detection Target                          | Language | Input Range (# characters)
|----------------|-------------------------------|-----------------------------|-----------------------------|
|[**Hello-SimpleAI ChatGPT Detector**](https://hello-simpleai-chatgpt-detector-ling.hf.space/)       | ChatGPT       |en/zh          | (0,~1500] (512tokens)|
|[**GPTZero**](https://gptzero.me/)         |LLM       | en|(250，♾️)|
|**[OpenAI Classifier](https://openai.com/blog/new-ai-classifier-for-indicating-ai-written-text/)**      | LLM|en|(0，25,000]|
|**[Contentatscale AI Content Detector](https://contentatscale.ai/ai-content-detector/)**         | AI Content (NLP+SERP)|en|(0, 1,500]|
|**[Writers AI Content Detector](https://writer.com/ai-content-detector/)**      | AI Content |en|(0，♾️)|
