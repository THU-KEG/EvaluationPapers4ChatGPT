<img src="papers.png" style="zoom:67%;" />

# Evaluation Papers for ChatGPT

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) ![](https://img.shields.io/github/last-commit/THU-KEG/EvaluationPaper4ChatGPT?color=green) ![](https://img.shields.io/badge/PRs-Welcome-red) 


### News

- 2023/03/15: OpenAI released [gpt4](https://arxiv.org/pdf/2303.08774.pdf), which can be accessed on ChatGPT's plus service, we view it as a latest version of ChatGPT.


### Introduction

This repository stores Dataset Resources, Evaluation Papers and Detection Tools for ChatGPT.

* [0. Survey](#0-survey)
* [1. Dataset Resource](#1-dataset-resource)
* [2. Evaluation Papers](#2-evaluation-papers)
  * [2.1 Natural Language Understanding](#21-natural-language-understanding)
  * [2.2 Ethics and Bias](#22-ethics-and-bias)
  * [2.3 Long Text Summarization](#23-long-text-summarization)
  * [2.4 Reasoning](#24-reasoning)
  * [2.5 MultiModal](#25-multimodal)
  * [2.6 Information Extraction](#26-information-extraction)
  * [2.7 Machine Translation](#27-machine-translation)
  * [2.8 Other Domains](#28-other-domains)
* [3. Detection Tools](#3-detection-tools)
  * [3.1 Metrics](#31-metrics)
  * [3.2 Available Tools](#32-available-tools)

## 0. Survey
1. **ChatGPT: A Meta-Analysis after 2.5 Months.**

   *Christoph Leiter, Ran Zhang, Yanran Chen, Jonas Belouadi, Daniil Larionov, Vivian Fresen, Steffen Eger.* [[abs](https://arxiv.org/abs/2302.13795)], 2023.2
   
2. **Summary of ChatGPT/GPT-4 Research and Perspective Towards the Future of Large Language Models.**

   *Yiheng Liu, Tianle Han, Siyuan Ma, Jiayue Zhang, Yuanyuan Yang, Jiaming Tian, Hao He, Antong Li, Mengshen He, Zhengliang Liu, Zihao Wu, Dajiang Zhu, Xiang Li, Ning Qiang, Dingang Shen, Tianming Liu, Bao Ge.* [[abs](https://arxiv.org/abs/2304.01852)], 2023.4


## 1. Dataset Resource

1. **How Close is ChatGPT to Human Experts? Comparison Corpus, Evaluation, and Detection.**

   *Biyang Guo,  Xin Zhang , Ziyuan Wang, Minqi Jiang , Jinran Nie, Yuxuan Ding, Jianwei Yue , Yupeng Wu.* [[abs](https://arxiv.org/abs/2301.07597)],[[github](https://github.com/Hello-SimpleAI/chatgpt-comparison-detection)], 2023.1

2. **ChatGPT: Jack of all trades, master of none.**

   *Jan Kocoń , Igor Cichecki , Oliwier Kaszyca , Mateusz Kochanek , Dominika Szydło , Joanna Baran, Julita Bielaniewicz, Marcin Gruza, Arkadiusz Janz, Kamil Kanclerz, Anna Kocoń, Bartłomiej Koptyra, Wiktoria Mieleszczenko-Kowszewicz, Piotr Miłkowski, Marcin Oleksy, Maciej Piasecki, Łukasz Radliński, Konrad Wojtasik, Stanisław Woźniak and Przemysław Kazienko.* [[abs](https://arxiv.org/abs/2302.10724)],[[github](https://github.com/CLARIN-PL/chatgpt-evaluation-01-2023)], 2023.2

3. **Can ChatGPT Understand Too? A Comparative Study on ChatGPT and Fine-tuned BERT.**

   *Qihuang Zhong, Liang Ding,  Juhua Liu, Bo Du, Dacheng Tao.* [[abs](https://arxiv.org/abs/2302.10198)],[[github](https://github.com/WHU-ZQH/ChatGPT-vs.-BERT)], 2023.2
   
4. **Is ChatGPT A Good Translator? A Preliminary Study.**

   *Wenxiang Jiao, Wenxuan Wang, Jen-tse Huang, Xing Wang, Zhaopeng Tu.* [[abs](https://arxiv.org/abs/2301.08745v2)],[[github](https://github.com/wxjiao/Is-ChatGPT-A-Good-Translator)], 2023.1
   
5. **On the Robustness of ChatGPT: An Adversarial and Out-of-distribution Perspective.**

   *Jindong Wang, Xixu Hu, Wenxin Hou, Hao Chen, Runkai Zheng, Yidong Wang, Linyi Yang, Haojun Huang, Wei Ye, Xiubo Geng, Binxin Jiao, Yue Zhang, Xing Xie
.* [[abs](https://arxiv.org/abs/2302.12095)],[[github](https://github.com/microsoft/robustlearn)], 2023.2

6. **An Independent Evaluation of ChatGPT on Mathematical Word Problems (MWP).**

   *Paulo Shakarian, Abhinav Koyyalamudi, Noel Ngu, Lakshmivihari Mareedu.* [[abs](https://arxiv.org/abs/2302.13814)][[github](https://github.com/lab-v2/ChatGPT_MWP_eval)], 2023.2

7. **Evaluation of ChatGPT as a Question Answering System for Answering Complex Questions.**

   *Yiming Tan, Dehai Min, Yu Li, Wenbo Li, Nan Hu, Yongrui Chen, Guilin Qi.* [[abs](https://arxiv.org/abs/2303.07992)][[github](https://github.com/tan92hl/Complex-Question-Answering-Evaluation-of-ChatGPT)], 2023.3


Data statistics of these resources:

|    Paper with Dataset | Task                          | #Examples
|----------------|-------------------------------|-----------------------------|
|How Close is ChatGPT to Human Experts? Comparison Corpus, Evaluation, and Detection|QA + Dialog           |40,000       |
|ChatGPT: Jack of all trades, master of none         | 25 classification/ QA/reasoning  task|38,000|
|Can ChatGPT Understand Too? A Comparative Study on ChatGPT and Fine-tuned BERT          | sentiment analysis / Paraphrase / NLI         |475          |
|Is ChatGPT A Good Translator? A Preliminary Study       | Translation|5,609|
|On the Robustness of ChatGPT: An Adversarial and Out-of-distribution Perspective     | Robustness|2,237|
|An Independent Evaluation of ChatGPT on Mathematical Word Problems (MWP).     | Reasoning|1,000|
|Evaluation of ChatGPT as a Question Answering System for Answering Complex Questions.     | Complex QA|194,782|



## 2. Evaluation Papers


### 2.1 Natural Language Understanding

1. **Can ChatGPT Understand Too? A Comparative Study on ChatGPT and Fine-tuned BERT.**

   *Qihuang Zhong, Liang Ding,  Juhua Liu, Bo Du, Dacheng Tao.* [[abs](https://arxiv.org/abs/2302.10198)],[[github](https://github.com/WHU-ZQH/ChatGPT-vs.-BERT)], 2023.2

2. **ChatGPT: Jack of all trades, master of none.**

   *Jan Kocoń , Igor Cichecki , Oliwier Kaszyca , Mateusz Kochanek , Dominika Szydło , Joanna Baran, Julita Bielaniewicz, Marcin Gruza, Arkadiusz Janz, Kamil Kanclerz, Anna Kocoń, Bartłomiej Koptyra, Wiktoria Mieleszczenko-Kowszewicz, Piotr Miłkowski, Marcin Oleksy, Maciej Piasecki, Łukasz Radliński, Konrad Wojtasik, Stanisław Woźniak and Przemysław Kazienko.* [[abs](https://arxiv.org/abs/2302.10724)],[[github](https://github.com/CLARIN-PL/chatgpt-evaluation-01-2023)], 2023.2
   
3. **How Robust is GPT-3.5 to Predecessors? A Comprehensive Study on Language Understanding Tasks.**

   *Xuanting Chen, Junjie Ye, Can Zu, Nuo Xu, Rui Zheng, Minlong Peng, Jie Zhou, Tao Gui, Qi Zhang, Xuanjing Huang.* [[abs](https://arxiv.org/abs/2303.00293)], 2023.3
   
4. **Consistency Analysis of ChatGPT.**

   *Myeongjun Jang, Thomas Lukasiewicz.* [[abs](https://arxiv.org/abs/2303.06273)], 2023.3

5. **Does ChatGPT resemble humans in language use?**

   *Zhenguang G. Cai, David A. Haslett, Xufeng Duan, Shuqi Wang, Martin J. Pickering.* [[abs](https://arxiv.org/abs/2303.08014)], 2023.3

6. **A Comprehensive Capability Analysis of GPT-3 and GPT-3.5 Series Models.**

   *Junjie Ye, Xuanting Chen, Nuo Xu, Can Zu, Zekai Shao, Shichun Liu, Yuhan Cui, Zeyang Zhou, Chao Gong, Yang Shen, Jie Zhou, Siming Chen, Tao Gui, Qi Zhang, Xuanjing Huang.* [[abs](https://arxiv.org/abs/2303.10420)], 2023.3

7. **Can we trust the evaluation on ChatGPT?**

   *Rachith Aiyappa, Jisun An, Haewoon Kwak, Yong-Yeol Ahn.* [[abs](https://arxiv.org/abs/2303.12767)], 2023.3

8. **A comprehensive evaluation of ChatGPT's zero-shot Text-to-SQL capability.**

   *Aiwei Liu, Xuming Hu, Lijie Wen, Philip S. Yu.* [[abs](https://arxiv.org/abs/2303.13547)][[github](https://github.com/THU-BPM/chatgpt-sql)], 2023.3

9. **ChatGPT or Grammarly? Evaluating ChatGPT on Grammatical Error Correction Benchmark.**

   *Haoran Wu, Wenxuan Wang, Yuxuan Wan, Wenxiang Jiao, Michael Lyu.* [[abs](https://arxiv.org/abs/2303.13648)], 2023.3

10. **Safety Analysis in the Era of Large Language Models: A Case Study of STPA using ChatGPT.**

    *Tao Fang, Shu Yang, Kaixin Lan, Derek F. Wong, Jinpeng Hu, Lidia S. Chao, Yue Zhang.* [[abs](https://arxiv.org/abs/2304.01746)], 2023.4



### 2.2 Ethics and Bias

1. **Exploring AI Ethics of ChatGPT: A Diagnostic Analysis.**

   *Terry Yue Zhuo, Yujin Huang , Chunyang Chen , Zhenchang Xing.* [[abs](https://arxiv.org/abs/2301.12867)], 2023.2

2. **Is ChatGPT better than Human Annotators? Potential and Limitations of ChatGPT in Explaining Implicit Hate Speech.**

   *Fan Huang, Haewoon Kwak, Jisun An.* [[abs](https://arxiv.org/abs/2302.07736)], 2023.2

3. **ChatGPT Outperforms Crowd-Workers for Text-Annotation Tasks.**
   
    *Fabrizio Gilardi, Meysam Alizadeh, Maël Kubli.* [[abs](https://arxiv.org/abs/2303.15056)], 2023.3

4. **Chinese Intermediate English Learners outdid ChatGPT in deep cohesion: Evidence from English narrative writing.**

   *Tongquan Zhou, Siyi Cao, Siruo Zhou, Yao Zhang, Aijing He.* [[abs](https://arxiv.org/abs/2303.11812)], 2023.3

5. **A Perspectival Mirror of the Elephant: Investigating Language Bias on Google, ChatGPT, Wikipedia, and YouTube.**

   *Queenie Luo, Michael J. Puett, Michael D. Smith.* [[abs](https://arxiv.org/abs/2303.16281)], 2023.3

6. **Assessing Cross-Cultural Alignment between ChatGPT and Human Societies: An Empirical Study.**

   *Yong Cao, Li Zhou, Seolhwa Lee, Laura Cabello, Min Chen, Daniel Hershcovich.* [[abs](https://arxiv.org/abs/2303.17466)], 2023.3

7. **Safety Analysis in the Era of Large Language Models: A Case Study of STPA using ChatGPT.**

   *Yi Qi, Xingyu Zhao, Xiaowei Huang.* [[abs](https://arxiv.org/abs/2304.01246)], 2023.4


### 2.3 Long Text Summarization

1. **Exploring the Limits of ChatGPT for Query or Aspect-based Text Summarization.**

   *Xianjun Yang, Yan Li, Xinlu Zhang, Haifeng Chen, Wei Cheng.* [[abs](https://arxiv.org/abs/2302.08081)], 2023.2

2. **Can ChatGPT Write a Good Boolean Query for Systematic Review Literature Search?**

   *Shuai Wang, Harrisen Scells, Bevan Koopman, Guido Zuccon.* [[abs](https://arxiv.org/abs/2302.03495)], 2023.2
   
3. **ChatGPT Makes Medicine Easy to Swallow: An Exploratory Case Study on Simplified Radiology Reports.**

   *Katharina Jeblick, Balthasar Schachtner, Jakob Dexl, Andreas Mittermeier, Anna Theresa Stüber, Johanna Topalis, Tobias Weber, Philipp Wesp, Bastian Sabel, Jens Ricke, Michael Ingrisch.* [[abs](https://arxiv.org/abs/2212.14882)], 2022.12
   
4. **Cross-Lingual Summarization via ChatGPT.**

   *Jiaan Wang, Yunlong Liang, Fandong Meng, Zhixu Li, Jianfeng Qu, Jie Zhou.* [[abs](https://arxiv.org/abs/2302.14229)], 2023.2

5. **ChatGPT as a Factual Inconsistency Evaluator for Abstractive Text Summarization.**

   *Zheheng Luo, Qianqian Xie, Sophia Ananiadou.* [[abs](https://arxiv.org/abs/2303.15621)], 2023.3     

6. **Assessing Cross-Cultural Alignment between ChatGPT and Human Societies: An Empirical Study.**

   *Yong Cao, Li Zhou, Seolhwa Lee, Laura Cabello, Min Chen, Daniel Hershcovich.* [[abs](https://arxiv.org/abs/2303.17466)], 2023.3     

7. **Comparing Abstractive Summaries Generated by ChatGPT to Real Summaries Through Blinded Reviewers and Text Classification Algorithms.**

   *Mayank Soni, Vincent Wade.* [[abs](https://arxiv.org/abs/2303.17650)], 2023.3     


### 2.4 Reasoning

1. **Mathematical Capabilities of ChatGPT.**

   *Simon Frieder, Luca Pinchetti, Ryan-Rhys Griffiths, Tommaso Salvatori, Thomas Lukasiewicz, Philipp Christian Petersen, Alexis Chevalier, Julius Berner.* [[abs](https://arxiv.org/abs/2301.13867)], 2023.1

2. **Is ChatGPT a General-Purpose Natural Language Processing Task Solver?**

   *Chengwei Qin, Aston Zhang, Zhuosheng Zhang, Jiaao Chen, Michihiro Yasunaga, Diyi Yang.* [[abs](https://arxiv.org/abs/2302.06476)], 2023.2

3. **A Categorical Archive of ChatGPT Failures.**

   *Ali Borji.* [[abs](https://arxiv.org/abs/2302.03494)], 2023.2

4. **An Independent Evaluation of ChatGPT on Mathematical Word Problems (MWP).**

   *Paulo Shakarian, Abhinav Koyyalamudi, Noel Ngu, Lakshmivihari Mareedu.* [[abs](https://arxiv.org/abs/2302.13814)][[github](https://github.com/lab-v2/ChatGPT_MWP_eval)], 2023.2

5. **Mind meets machine: Unravelling GPT-4's cognitive psychology.**

   *Sifatkaur, Manmeet Singh, Vaisakh SB, Neetiraj Malviya.* [[abs](https://arxiv.org/abs/2303.11436)], 2023.3
   
6. **Capabilities of GPT-4 on Medical Challenge Problems.**

   *Harsha Nori, Nicholas King, Scott Mayer McKinney, Dean Carignan, Eric Horvitz.* [[abs](https://arxiv.org/abs/2303.13375)], 2023.3
 
7. **GPT is becoming a Turing machine: Here are some ways to program it.**

   *Ana Jojic, Zhen Wang, Nebojsa Jojic.* [[abs](https://arxiv.org/abs/2303.14310)], 2023.3
 
8. **ChatGPT is a Knowledgeable but Inexperienced Solver: An Investigation of Commonsense Problem in Large Language Models.**

   *Ning Bian, Xianpei Han, Le Sun, Hongyu Lin, Yaojie Lu, Ben He.* [[abs](https://arxiv.org/abs/2303.16421)], 2023.3

9. **Humans in Humans Out: On GPT Converging Toward Common Sense in both Success and Failure.**

   *Philipp Koralus, Vincent Wang-Maścianica.* [[abs](https://arxiv.org/abs/2303.17276)], 2023.3

10. **LLMMaps -- A Visual Metaphor for Stratified Evaluation of Large Language Models.**

    *Patrik Puchert, Poonam Poonam, Christian van Onzenoodt, Timo Ropinski.* [[abs](https://arxiv.org/abs/2304.00457)], 2023.4


### 2.5 Multimodal

1. **A Multitask, Multilingual, Multimodal Evaluation of ChatGPT on Reasoning, Hallucination, and Interactivity.**

   *Yejin Bang, Samuel Cahyawijaya, Nayeon Lee, Wenliang Dai, Dan Su, Bryan Wilie, Holy Lovenia, Ziwei Ji, Tiezheng Yu, Willy Chung, Quyet V. Do, Yan Xu, Pascale Fung.* [[abs](https://arxiv.org/abs/2302.04023)], 2023.2

2. **A Pilot Evaluation of ChatGPT and DALL-E 2 on Decision Making and Spatial Reasoning.**

   *Zhisheng Tang, Mayank Kejriwal.* [[abs](https://arxiv.org/abs/2302.09068)], 2023.2

3. **MM-REACT: Prompting ChatGPT for Multimodal Reasoning and Action.**

   *Zhengyuan Yang, Linjie Li, Jianfeng Wang, Kevin Lin, Ehsan Azarnasab, Faisal Ahmed, Zicheng Liu, Ce Liu, Michael Zeng, Lijuan Wang.* [[abs](https://arxiv.org/abs/2303.11381)], 2023.3

4. **Sparks of Artificial General Intelligence: Early experiments with GPT-4.**

   *Sébastien Bubeck, Varun Chandrasekaran, Ronen Eldan, Johannes Gehrke, Eric Horvitz, Ece Kamar, Peter Lee, Yin Tat Lee, Yuanzhi Li, Scott Lundberg, Harsha Nori, Hamid Palangi, Marco Tulio Ribeiro, Yi Zhang.* [[abs](https://arxiv.org/abs/2303.12712)], 2023.3

5. **GesGPT: Speech Gesture Synthesis With Text Parsing from GPT.**

   *Nan Gao, Zeyu Zhao, Zhi Zeng, Shuwu Zhang, Dongdong Weng.* [[abs](https://arxiv.org/abs/2303.13013)], 2023.3

6. **ChatGPT4PCG Competition: Character-like Level Generation for Science Birds.**

   *Pittawat Taveekitworachai, Febri Abdullah, Mury F. Dewantoro, Ruck Thawonmas, Julian Togelius, Jochen Renz.* [[abs](https://arxiv.org/abs/2303.15662)], 2023.3
   
7. **HuggingGPT: Solving AI Tasks with ChatGPT and its Friends in HuggingFace.**

   *Yongliang Shen, Kaitao Song, Xu Tan, Dongsheng Li, Weiming Lu, Yueting Zhuang.* [[abs](https://arxiv.org/abs/2303.17580)], 2023.3
   
8. **WavCaps: A ChatGPT-Assisted Weakly-Labelled Audio Captioning Dataset for Audio-Language Multimodal Research.**

   *Xinhao Mei, Chutong Meng, Haohe Liu, Qiuqiang Kong, Tom Ko, Chengqi Zhao, Mark D. Plumbley, Yuexian Zou, Wenwu Wang.* [[abs](https://arxiv.org/abs/2303.17395)], 2023.3  
   
### 2.6 Information Extraction

1. **Zero-Shot Information Extraction via Chatting with ChatGPT.**

   *Xiang Wei, Xingyu Cui, Ning Cheng, Xiaobin Wang, Xin Zhang, Shen Huang, Pengjun Xie, Jinan Xu, Yufeng Chen, Meishan Zhang, Yong Jiang, Wenjuan Han.* [[abs](https://arxiv.org/abs/2302.10205)][[github](https://github.com/cocacola-lab/GPT4IE)][[demo](https://cocacola-lab.github.io/GPT4IE/)], 2023.2
   
2. **Exploring the Feasibility of ChatGPT for Event Extraction.**

   *Jun Gao, Huan Zhao, Changlong Yu, Ruifeng Xu.* [[abs](https://arxiv.org/abs/2303.03836)], 2023.3

3. **Extracting Accurate Materials Data from Research Papers with Conversational Language Models and Prompt Engineering -- Example of ChatGPT.**

   *Maciej P. Polak, Dane Morgan.* [[abs](https://arxiv.org/abs/2303.05352)], 2023.3

4. **Is ChatGPT A Good Keyphrase Generator? A Preliminary Study.**

   *Mingyang Song, Haiyun Jiang, Shuming Shi, Songfang Yao, Shilong Lu, Yi Feng, Huafeng Liu, Liping Jing.* [[abs](https://arxiv.org/abs/2303.13001)], 2023.3
   
5. **Yes but.. Can ChatGPT Identify Entities in Historical Documents?**

   *Carlos-Emiliano González-Gallardo, Emanuela Boros, Nancy Girdhar, Ahmed Hamdi, Jose G. Moreno, Antoine Doucet.* [[abs](https://arxiv.org/abs/2303.17322)], 2023.3   
   
   
### 2.7 Machine Translation

1. **Is ChatGPT A Good Translator? A Preliminary Study.**

   *Wenxiang Jiao, Wenxuan Wang, Jen-tse Huang, Xing Wang, Zhaopeng Tu.* [[abs](https://arxiv.org/abs/2301.08745v2)],[[github](https://github.com/wxjiao/Is-ChatGPT-A-Good-Translator)], 2023.1
   
2. **Error Analysis Prompting Enables Human-Like Translation Evaluation in Large Language Models: A Case Study on ChatGPT.**

   *Qingyu Lu, Baopu Qiu, Liang Ding, Liping Xie, Dacheng Tao.* [[abs](https://arxiv.org/abs/2303.13809)],[[github](https://github.com/Coldmist-Lu/ErrorAnalysis_Prompt)], 2023.3

3. **Towards Making the Most of ChatGPT for Machine Translation.**

   *Keqin Peng, Liang Ding, Qihuang Zhong, Li Shen, Xuebo Liu, Min Zhang, Yuanxin Ouyang, Dacheng Tao.* [[abs](https://arxiv.org/abs/2303.13780)],[[github](https://github.com/Romainpkq/ChatGPT4MT)], 2023.3
   
4. **Linguistically Informed ChatGPT Prompts to Enhance Japanese-Chinese Machine Translation: A Case Study on Attributive Clauses.**

   *Wenshi Gu.* [[abs](https://arxiv.org/abs/2303.15587)], 2023.3


### 2.8 Other Domains

#### Education

1. **ChatGPT: The End of Online Exam Integrity?**

   *Teo Susnjak.* [[abs](https://arxiv.org/abs/2212.09292)], 2022.12
   
2. **ChatGPT: Bullshit spewer or the end of traditional assessments in higher education?**

   *Jürgen Rudolph, Samson Tan, Shannon Tan.* [[pdf](https://journals.sfu.ca/jalt/index.php/jalt/article/download/689/539)], 2023.1
   
3. **Will ChatGPT get you caught? Rethinking of Plagiarism Detection.**

   *Mohammad Khalil, Erkan Er.* [[abs](https://arxiv.org/abs/2302.04335)], 2023.2

4. **Seeing ChatGPT Through Students' Eyes: An Analysis of TikTok Data.**

   *Anna-Carolina Haensch, Sarah Ball, Markus Herklotz, Frauke Kreuter.* [[abs](https://arxiv.org/abs/2303.05349)], 2023.3

5. **ChatGPT Participates in a Computer Science Exam.**

   *Sebastian Bordt, Ulrike von Luxburg.* [[abs](https://arxiv.org/abs/2303.09461)][[github](https://github.com/tml-tuebingen/chatgpt-algorithm-exam)], 2023.3
   
6. **Evaluating GPT-3.5 and GPT-4 Models on Brazilian University Admission Exams.**

   *Desnes Nunes, Ricardo Primi, Ramon Pires, Roberto Lotufo, Rodrigo Nogueira.* [[abs](https://arxiv.org/abs/2303.17003)],[[github](https://github.com/piresramon/gpt-4-enem)], 2023.3
   
7. **Can AI Chatbots Pass the Fundamentals of Engineering (FE) and Principles and Practice of Engineering (PE) Structural Exams?**

   *M.Z. Naser, Brandon Ross, Jennier Ogle, Venkatesh Kodur, Rami Hawileh, Jamal Abdalla, Huu-Tai Thai.* [[abs](https://arxiv.org/abs/2303.18149)], 2023.3

#### Biology

1. **How Does ChatGPT Perform on the Medical Licensing Exams? The Implications of Large Language Models for Medical Education and Knowledge Assessment.**

   *Aidan Gilson, Conrad Safranek, Thomas Huang, Vimig Socrates, Ling Chi, R. Andrew Taylor, David Chartash.* [[pdf](https://www.medrxiv.org/content/10.1101/2022.12.23.22283901.full.pdf)], 2022.12
   
2. **Evaluating ChatGPT as an Adjunct for Radiologic Decision-Making.**

   *Arya Rao, John Kim, Meghana Kamineni, Michael Pang, Winston Lie, Marc D. Succi.* [[pdf](https://www.medrxiv.org/content/medrxiv/early/2023/02/07/2023.02.02.23285399.full.pdf)], 2023.2
   
3. **Dr ChatGPT, tell me what I want to hear: How prompt knowledge impacts health answer correctness.**

   *Guido Zuccon, Bevan Koopman.* [[abs](https://arxiv.org/abs/2302.13793)], 2023.2

4. **The utility of ChatGPT for cancer treatment information.**

   *Shan Chen, Benjamin H Kann, Michael B Foote, Hugo JWL Aerts, Guergana K Savova, Raymond H Mak, Danielle S Bitterman.* [[abs](https://www.medrxiv.org/content/10.1101/2023.03.16.23287316v1)],[[github](https://github.com/AIM-Harvard/ChatGPT_NCCN)], 2023.3

5. **Translating Radiology Reports into Plain Language using ChatGPT and GPT-4 with Prompt Learning: Promising Results, Limitations, and Potential.**

   *Qing Lyu, Josh Tan, Mike E. Zapadka, Janardhana Ponnatapuram, Chuang Niu, Ge Wang, Christopher T. Whitlow.* [[abs](https://arxiv.org/abs/2303.09038)], 2023.3

6. **Evaluation of ChatGPT for NLP-based Mental Health Applications.**

   *Bishal Lamichhane.* [[abs](https://arxiv.org/abs/2303.15727)], 2023.3

7. **Evaluating GPT-4 and ChatGPT on Japanese Medical Licensing Examinations.**

   *Jungo Kasai, Yuhei Kasai, Keisuke Sakaguchi, Yutaro Yamada, Dragomir Radev.* [[abs](https://arxiv.org/abs/2303.18027)],[[github](https://github.com/jungokasai/IgakuQA)],  2023.3

8. **Evaluation of GPT and BERT-based models on identifying protein-protein interactions in biomedical text.**

   *Hasin Rehana, Nur Bengisu Çam, Mert Basmaci, Yongqun He, Arzucan Özgür, Junguk Hur.* [[abs](https://arxiv.org/abs/2303.17728)], 2023.3

#### Psychology


1. **Is GPT-3 a Psychopath? Evaluating Large Language Models from a Psychological Perspective.**

   *Xingxuan Li, Yutong Li, Linlin Liu, Lidong Bing, Shafiq Joty.* [[abs](https://arxiv.org/abs/2212.10529)], 2022.12

2. **Theory of Mind May Have Spontaneously Emerged in Large Language Models.**

   *Michal Kosinski.* [[abs](https://arxiv.org/abs/2302.02083)], 2023.2

3. **Can ChatGPT Assess Human Personalities? A General Evaluation Framework.**

   *Haocong Rao, Cyril Leung, Chunyan Miao.* [[abs](https://arxiv.org/abs/2303.01248)][[github](https://github.com/Kali-Hac/ChatGPT-MBTI)], 2023.3
   
4. **Will Affective Computing Emerge from Foundation Models and General AI? A First Evaluation on ChatGPT.**

   *Mostafa M. Amin, Erik Cambria, Björn W. Schuller.* [[abs](https://arxiv.org/abs/2303.03186)], 2023.3

#### Law

1. **Chatgpt goes to law school**

   *Teo Susnjak.* [[abs](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4335905)], 2023


## 3. Detection Tools

### 3.1 Metrics

#### Metrics Before ChatGPT

1. **DetectGPT: Zero-Shot Machine-Generated Text Detection using Probability Curvature.**

   *Eric Mitchell, Yoonho Lee, Alexander Khazatsky, Christopher D. Manning, Chelsea Finn.* [[abs](https://arxiv.org/abs/2301.11305)],[[demo](https://detectgpt.ericmitchell.ai/)], 2023.1

2. **GPTScore: Evaluate as You Desire.**

   *Jinlan Fu, See-Kiong Ng, Zhengbao Jiang, Pengfei Liu.* [[abs](https://arxiv.org/abs/2302.04166)],[[github](https://github.com/jinlanfu/GPTScore)], 2023.2

3. **MAUVE Scores for Generative Models: Theory and Practice.**

   *Krishna Pillutla, Lang Liu, John Thickstun, Sean Welleck, Swabha Swayamdipta, Rowan Zellers, Sewoong Oh, Yejin Choi, Zaid Harchaoui.* [[abs](https://arxiv.org/abs/2212.14578)], 2022.12


#### Using ChatGPT as evaluation metric

1. **Large Language Models Are State-of-the-Art Evaluators of Translation Quality.**

   *Tom Kocmi, Christian Federmann.* [[abs](https://arxiv.org/abs/2302.14520)],[[github](https://github.com/MicrosoftTranslator/GEMBA)], 2023.2

2. **Is ChatGPT a Good NLG Evaluator? A Preliminary Study.**

   *Jiaan Wang, Yunlong Liang, Fandong Meng, Haoxiang Shi, Zhixu Li, Jinan Xu, Jianfeng Qu, Jie Zhou.* [[abs](https://arxiv.org/abs/2303.04048)],[[github](https://github.com/krystalan/chatgpt_as_nlg_evaluator)], 2023.3

3. **Exploring ChatGPT's Ability to Rank Content: A Preliminary Study on Consistency with Human Preferences.**

   *Yunjie Ji, Yan Gong, Yiping Peng, Chao Ni, Peiyan Sun, Dongyu Pan, Baochang Ma, Xiangang Li.* [[abs](https://arxiv.org/abs/2303.07610)], 2023.3

4. **Error Analysis Prompting Enables Human-Like Translation Evaluation in Large Language Models: A Case Study on ChatGPT.**

   *Qingyu Lu, Baopu Qiu, Liang Ding, Liping Xie, Dacheng Tao.* [[abs](https://arxiv.org/abs/2303.13809)],[[github](https://github.com/Coldmist-Lu/ErrorAnalysis_Prompt)], 2023.3

5. **GPTEval: NLG Evaluation using GPT-4 with Better Human Alignment.**

   *Yang Liu, Dan Iter, Yichong Xu, Shuohang Wang, Ruochen Xu, Chenguang Zhu.* [[abs](https://arxiv.org/abs/2303.16634)], 2023.3

6. **Exploring the Use of Large Language Models for Reference-Free Text Quality Evaluation: A Preliminary Empirical Study.**

   *Yi Chen, Rui Wang, Haiyun Jiang, Shuming Shi, Ruifeng Xu.* [[abs](https://arxiv.org/abs/2304.00723)],[[github](https://github.com/MilkWhite/LLMs_for_Reference_Free_Text_Quality_Evaluation)], 2023.4
   
#### Metrics for detecting ChatGPT

1. **AI vs. Human -- Differentiation Analysis of Scientific Content Generation.**

   *Yongqiang Ma, Jiawei Liu, Fan Yi, Qikai Cheng, Yong Huang, Wei Lu, Xiaozhong Liu.* [[abs](https://arxiv.org/abs/2301.10416)], 2023.1


2. **ChatGPT or academic scientist? Distinguishing authorship with over 99% accuracy using off-the-shelf machine learning tools.**

   *Heather Desaire, Aleesa E. Chua, Madeline Isom, Romana Jarosova, David Hua.* [[abs](https://arxiv.org/abs/2303.16352)], 2023.3


### 3.2 Available Tools

1. [**Hello-SimpleAI ChatGPT Detector**](https://hello-simpleai-chatgpt-detector-ling.hf.space/):  An open-source detection project consists of three versions of models to detect text generated with ChatGPT, including [QA version](https://huggingface.co/spaces/Hello-SimpleAI/chatgpt-detector-qa), [Sinlge-text version](https://huggingface.co/spaces/Hello-SimpleAI/chatgpt-detector-single) and [Linguistic version](https://huggingface.co/spaces/Hello-SimpleAI/chatgpt-detector-ling).
2. [**GPTZero**](https://gptzero.me/): A demo to detect writings generated by ChatGPT. The creator has seen that the technology was used by students to cheat on assignments, so he came up with a safeguard. 
3. **[OpenAI Classifier](https://openai.com/blog/new-ai-classifier-for-indicating-ai-written-text/)**: A classifier fine-tuned on a dataset of pairs of human-written text and AI-written text on the same topic.
4. **[Contentatscale AI Content Detector](https://contentatscale.ai/ai-content-detector/)** : A tool that allows users to receive the Human or AI Content score in the text to detect. It provides probability for each sentence.
5. **[Writers AI Content Detector](https://writer.com/ai-content-detector/)**: A tool similar to Contentatscale. It requires either the URL of the page or text to calculate the “Human-Generated Content” score. 



Statistics of these tools:

|    Tool |  Detection Target                          | Language | Input Range (# characters)
|----------------|-------------------------------|-----------------------------|-----------------------------|
|[**Hello-SimpleAI ChatGPT Detector**](https://hello-simpleai-chatgpt-detector-ling.hf.space/)       | ChatGPT       |en/zh          | (0,~1500] (512tokens)|
|[**GPTZero**](https://gptzero.me/)         |LLM       | en|(250，♾️)|
|**[OpenAI Classifier](https://openai.com/blog/new-ai-classifier-for-indicating-ai-written-text/)**      | LLM|en|(0，♾️)|
|**[Contentatscale AI Content Detector](https://contentatscale.ai/ai-content-detector/)**         | AI Content (NLP+SERP)|en|(0，25,000]|
|**[Writers AI Content Detector](https://writer.com/ai-content-detector/)**      | AI Content |en|(0, 1,500]|
