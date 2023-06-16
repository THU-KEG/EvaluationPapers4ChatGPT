<img src="papers.png" style="zoom:67%;" />

# Evaluation Papers for ChatGPT

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT) ![](https://img.shields.io/github/last-commit/THU-KEG/EvaluationPaper4ChatGPT?color=green) ![](https://img.shields.io/badge/PRs-Welcome-red) 


### News

- 2023/03/15: OpenAI released [gpt4](https://arxiv.org/pdf/2303.08774.pdf), which can be accessed on ChatGPT's plus service, we view it as a latest version of ChatGPT.
- 2023/04/28: We are maintaining a dataset [ChatLog](https://github.com/THU-KEG/ChatLog), which collects ChatGPT responses everyday from 2023-03-05 to now. We evaluate ChatGPT's performance on 21 benchmarks across time and find that previous evaluation results may change at new dates. Based on the colleted data, we build [OpenChatLog](https://github.com/ShangQingTu/OpenChatLog), a search engine for LLM generated texts. Try our [website](http://103.238.162.37:9621/) (If your ip is in China).
- 2023/06/08: We propose [Language-Model-as-an-Examiner](https://arxiv.org/abs/2306.04181), a novel benchmarking framework where the LM serves as a knowledgeable examiner that formulates questions based on its knowledge and evaluates responses in a reference-free manner. Try our dataset LMExamQA and benchmarking result at [here](https://lmexam.com).
- 2023/06/16: We are delighted to announce the official release of [*KoLA*](https://arxiv.org/abs/2306.09296), a continuously evolving world knowledge evaluation platform that encompasses a 4-layer cognitive structure and 19 tasks. Our goal is to provide unbiased evaluation results to assist in enhancing the capabilities of knowledge systems and large models. You can participate in the evaluation or provide feedback through the platform at https://kola.xlore.cn/ or via [GitHub](https://github.com/THU-KEG/KoLA).
 
### Introduction

This repository stores Dataset Resources, Evaluation Papers and Detection Tools for ChatGPT.

* [0. Survey](#0-survey)
* [1. Dataset Resource](#1-dataset-resource)
* [2. Evaluation Papers](#2-evaluation-papers)
  * [2.1 Natural Language Understanding](#21-natural-language-understanding)
  * [2.2 Ethics and Bias](#22-ethics-and-bias)
  * [2.3 Long Text Summarization and Information Retrieval](#23-long-text-summarization-and-information-retrieval)
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

3. **Harnessing the Power of LLMs in Practice: A Survey on ChatGPT and Beyond.**

   *Jingfeng Yang, Hongye Jin, Ruixiang Tang, Xiaotian Han, Qizhang Feng, Haoming Jiang, Bing Yin, Xia Hu.* [[abs](https://arxiv.org/abs/2304.13712)], 2023.4


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

8. **Instruction Tuning with GPT-4.**

   *Baolin Peng, Chunyuan Li, Pengcheng He, Michel Galley, Jianfeng Gao.* [[abs](https://arxiv.org/abs/2304.03277)][[github](https://instruction-tuning-with-gpt-4.github.io/)], 2023.4
   
9. **medAlpaca: Finetuned Large Language Models for Medical Question Answering.**

   *Keno Bressem, Tianyu Han, Shan Chen, et al.* [[github](https://github.com/kbressem/medAlpaca)], 2023.4

10. **ChatLog: Recording and Analyzing ChatGPT Across Time.**

    *Shangqing Tu, Chunyang Li, Jifan Yu, Xiaozhi Wang, Lei Hou, Juanzi Li.* [[abs](https://arxiv.org/abs/2304.14106)][[github](https://github.com/THU-KEG/ChatLog)], 2023.4
    
11. **Can LLM Already Serve as A Database Interface? A BIg Bench for Large-Scale Database Grounded Text-to-SQLs.**

    *Jinyang Li, Binyuan Hui, Ge Qu, Binhua Li, Jiaxi Yang, Bowen Li, Bailin Wang, Bowen Qin, Rongyu Cao, Ruiying Geng, Nan Huo, Chenhao Ma, Kevin C.C. Chang, Fei Huang, Reynold Cheng, Yongbin Li.* [[abs](https://arxiv.org/abs/2305.03111)][[github](https://github.com/AlibabaResearch/DAMO-ConvAI/tree/main/bird)], 2023.5
    
12. **A Systematic Study and Comprehensive Evaluation of ChatGPT on Benchmark Datasets.**

    *Md Tahmid Rahman Laskar, M Saiful Bari, Mizanur Rahman, Md Amran Hossen Bhuiyan, Shafiq Joty, Jimmy Xiangji Huang.* [[abs](https://arxiv.org/abs/2305.18486)][[github](https://github.com/ntunlp/ChatGPT_Eval)], 2023.5


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
|Instruction Tuning with GPT-4.     | Instruction Following|172,000|
|medAlpaca: Finetuned Large Language Models for Medical Question Answering.     | Medical QA|1.5 million|
|ChatLog: Recording and Analyzing ChatGPT Across Time.     | 21 NLU and NLG tasks|73,730 (growing everyday) |
|ArguGPT: evaluating, understanding and identifying argumentative essays generated by GPT models.     | Essay Writing | 9,647 |
|Can LLM Already Serve as A Database Interface? A BIg Bench for Large-Scale Database Grounded Text-to-SQLs.     | Text-to-SQL | 12,751 |
|A Systematic Study and Comprehensive Evaluation of ChatGPT on Benchmark Datasets.     | NLP Benchmarks | 255K |


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

11. **Is ChatGPT a Good Sentiment Analyzer? A Preliminary Study.**

    *Zengzhi Wang, Qiming Xie, Zixiang Ding, Yi Feng, Rui Xia.* [[abs](https://arxiv.org/abs/2304.04339)], 2023.4

12. **A Preliminary Evaluation of ChatGPT for Zero-shot Dialogue Understanding.**

    *Wenbo Pan, Qiguang Chen, Xiao Xu, Wanxiang Che, Libo Qin.* [[abs](https://arxiv.org/abs/2304.04256)], 2023.4

13. **Zero-shot Temporal Relation Extraction with ChatGPT.**

    *Chenhan Yuan, Qianqian Xie, Sophia Ananiadou.* [[abs](https://arxiv.org/abs/2304.05454)], 2023.4

14. **Can ChatGPT Reproduce Human-Generated Labels? A Study of Social Computing Tasks.**

    *Yiming Zhu, Peixian Zhang, Ehsan-Ul Haq, Pan Hui, Gareth Tyson.* [[abs](https://arxiv.org/abs/2304.10145)], 2023.4

15. **ChatGraph: Interpretable Text Classification by Converting ChatGPT Knowledge to Graphs.**

    *Yucheng Shi, Hehuan Ma, Wenliang Zhong, Gengchen Mai, Xiang Li, Tianming Liu, Junzhou Huang.* [[abs](https://arxiv.org/abs/2305.03513)], 2023.5

16. **Uncovering the Potential of ChatGPT for Discourse Analysis in Dialogue: An Empirical Study.**

    *Yaxin Fan, Feng Jiang.* [[abs](https://arxiv.org/abs/2305.08391)], 2023.5

17. **Evaluating ChatGPT's Performance for Multilingual and Emoji-based Hate Speech Detection.**

    *Mithun Das, Saurabh Kumar Pandey, Animesh Mukherjee.* [[abs](https://arxiv.org/abs/2305.13276)], 2023.5

18. **Distilling ChatGPT for Explainable Automated Student Answer Assessment.**

    *Jiazheng Li, Lin Gui, Yuxiang Zhou, David West, Cesare Aloisi, Yulan He.* [[abs](https://arxiv.org/abs/2305.12962)], 2023.5
    
19. **A Systematic Study and Comprehensive Evaluation of ChatGPT on Benchmark Datasets.**

    *Md Tahmid Rahman Laskar, M Saiful Bari, Mizanur Rahman, Md Amran Hossen Bhuiyan, Shafiq Joty, Jimmy Xiangji Huang.* [[abs](https://arxiv.org/abs/2305.18486)], 2023.5

20. **Sentiment Analysis in the Era of Large Language Models: A Reality Check.**

    *Wenxuan Zhang, Yue Deng, Bing Liu, Sinno Jialin Pan, Lidong Bing.* [[abs](https://arxiv.org/abs/2305.15005)], 2023.5

21. **The Two Word Test: A Semantic Benchmark for Large Language Models.**

    *Nicholas Riccardi, Rutvik H. Desai.* [[abs](https://arxiv.org/abs/2306.04610)], [[github](https://github.com/NickRiccardi/two-word-test)], 2023.6

22. **Xiezhi: An Ever-Updating Benchmark for Holistic Domain Knowledge Evaluation.**

    *Zhouhong Gu, Xiaoxuan Zhu, Haoning Ye, Lin Zhang, Jianchen Wang, Sihang Jiang, Zhuozhi Xiong, Zihan Li, Qianyu He, Rui Xu, Wenhao Huang, Zili Wang, Shusen Wang, Weiguo Zheng, Hongwei Feng, Yanghua Xiao.* [[abs](https://arxiv.org/abs/2306.05783)], [[github](https://github.com/MikeGu721/XiezhiBenchmark)], 2023.6

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

8. **Investigating Chain-of-thought with ChatGPT for Stance Detection on Social Media.**

   *Bowen Zhang, Xianghua Fu, Daijun Ding, Hu Huang, Yangyang Li, Liwen Jing.* [[abs](https://arxiv.org/abs/2304.03087)], 2023.4

9. **Should ChatGPT be Biased? Challenges and Risks of Bias in Large Language Models.**

   *Emilio Ferrara.* [[abs](https://arxiv.org/abs/2304.03738)], 2023.4

10. **Multi-step Jailbreaking Privacy Attacks on ChatGPT.**

    *Haoran Li, Dadi Guo, Wei Fan, Mingshi Xu, Yangqiu Song.* [[abs](https://arxiv.org/abs/2304.05197)], 2023.4

11. **Toxicity in ChatGPT: Analyzing Persona-assigned Language Models.**

    *Ameet Deshpande, Vishvak Murahari, Tanmay Rajpurohit, Ashwin Kalyan, Karthik Narasimhan.* [[abs](https://arxiv.org/abs/2304.05335)], 2023.4

12. **The Self-Perception and Political Biases of ChatGPT.**

    *Jérôme Rutinowski, Sven Franke, Jan Endendyk, Ina Dormuth, Markus Pauly.* [[abs](https://arxiv.org/abs/2304.07333)], 2023.4

13. **Speak, Memory: An Archaeology of Books Known to ChatGPT/GPT-4.**

    *Kent K. Chang, Mackenzie Cramer, Sandeep Soni, David Bamman.* [[abs](https://arxiv.org/abs/2305.00118)], 2023.5

14. **ChatGPT Needs SPADE (Sustainability, PrivAcy, Digital divide, and Ethics) Evaluation: A Review.**

    *Sunder Ali Khowaja, Parus Khuwaja, Kapal Dev.* [[abs](https://arxiv.org/abs/2305.03123)], 2023.5

15. **Not All Languages Are Created Equal in LLMs: Improving Multilingual Capability by Cross-Lingual-Thought Prompting.**

    *Haoyang Huang, Tianyi Tang, Dongdong Zhang, Wayne Xin Zhao, Ting Song, Yan Xia, Furu Wei.* [[abs](https://arxiv.org/abs/2305.07004)], 2023.5

16. **Is ChatGPT Fair for Recommendation? Evaluating Fairness in Large Language Model Recommendation.**

    *Jizhi Zhang, Keqin Bao, Yang Zhang, Wenjie Wang, Fuli Feng, Xiangnan He.* [[abs](https://arxiv.org/abs/2305.07609)], [[github]](https://github.com/jizhi-zhang/FaiRLLM), 2023.5

17. **BAD: BiAs Detection for Large Language Models in the context of candidate screening.**

    *Nam Ho Koh, Joseph Plata, Joyce Chai.* [[abs](https://arxiv.org/abs/2305.10407)], 2023.5

18. **Knowledge of cultural moral norms in large language models.**

    *Aida Ramezani, Yang Xu.* [[abs](https://arxiv.org/abs/2306.01857)], 2023.6


### 2.3 Long Text Summarization and Information Retrieval

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

8. **Comparative Analysis of CHATGPT and the evolution of language models.**

   *Oluwatosin Ogundare, Gustavo Quiros Araya.* [[abs](https://arxiv.org/abs/2304.02468)], 2023.4

9. **Extractive Summarization via ChatGPT for Faithful Summary Generation.**

   *Haopeng Zhang, Xiao Liu, Jiawei Zhang.* [[abs](https://arxiv.org/abs/2304.04193)], 2023.4
   
10. **Is ChatGPT Good at Search? Investigating Large Language Models as Re-Ranking Agent.**
 
    *Weiwei Sun, Lingyong Yan, Xinyu Ma, Pengjie Ren, Dawei Yin, Zhaochun Ren.* [[abs](https://arxiv.org/abs/2304.09542)], [[github](https://github.com/sunnweiwei/RankGPT)], 2023.4

11. **BIM-GPT: a Prompt-Based Virtual Assistant Framework for BIM Information Retrieval.**
 
    *Junwen Zheng, Martin Fischer.* [[abs](https://arxiv.org/abs/2304.09333)], 2023.4

12. **Uncovering ChatGPT's Capabilities in Recommender Systems.**
 
    *Sunhao Dai, Ninglu Shao, Haiyuan Zhao, Weijie Yu, Zihua Si, Chen Xu, Zhongxiang Sun, Xiao Zhang, Jun Xu.* [[abs](https://arxiv.org/abs/2305.02182)], [[github](https://github.com/rainym00d/LLM4RS)], 2023.5

13. **A First Look at LLM-Powered Generative News Recommendation.**
 
    *Qijiong Liu, Nuo Chen, Tetsuya Sakai, Xiao-Ming Wu.* [[abs](https://arxiv.org/abs/2305.06566)], 2023.5

14. **HaluEval: A Large-Scale Hallucination Evaluation Benchmark for Large Language Models.**
 
    *Junyi Li, Xiaoxue Cheng, Wayne Xin Zhao, Jian-Yun Nie, Ji-Rong Wen.* [[abs](https://arxiv.org/abs/2305.11747)], 2023.5

15. **RecurrentGPT: Interactive Generation of (Arbitrarily) Long Text.**
 
    *Wangchunshu Zhou, Yuchen Eleanor Jiang, Peng Cui, Tiannan Wang, Zhenxin Xiao, Yifan Hou, Ryan Cotterell, Mrinmaya Sachan.* [[abs](https://arxiv.org/abs/2305.13304)], [[github](https://github.com/aiwaves-cn/RecurrentGPT)], 2023.5

16. **PokemonChat: Auditing ChatGPT for Pokémon Universe Knowledge.**
 
    *Laura Cabello, Jiaang Li, Ilias Chalkidis.* [[abs](https://arxiv.org/abs/2306.03024)], 2023.6

17. **Hybrid Long Document Summarization using C2F-FAR and ChatGPT: A Practical Study.**
 
    *Guang Lu, Sylvia B. Larcher, Tu Tran.* [[abs](https://arxiv.org/abs/2306.01169)], 2023.6

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
    
11. **How well do Large Language Models perform in Arithmetic tasks?**
 
    *Zheng Yuan, Hongyi Yuan, Chuanqi Tan, Wei Wang, Songfang Huang.* [[abs](https://arxiv.org/abs/2304.02015)], 2023.4

12. **Evaluating the Logical Reasoning Ability of ChatGPT and GPT-4.**
 
    *Hanmeng Liu, Ruoxi Ning, Zhiyang Teng, Jian Liu, Qiji Zhou, Yue Zhang.* [[abs](https://arxiv.org/abs/2304.03439)], 2023.4

13. **ChatGPT-Crawler: Find out if ChatGPT really knows what it's talking about.**
 
    *Aman Rangapur, Haoran Wang.* [[abs](https://arxiv.org/abs/2304.03325)], [[github](https://github.com/IIT-NLP-RESEARCH/ChatGPT-Crawler)] 2023.4

14. **ChatABL: Abductive Learning via Natural Language Interaction with ChatGPT.**
 
    *Tianyang Zhong, Yaonai Wei, Li Yang, Zihao Wu, Zhengliang Liu, Xiaozheng Wei, Wenjun Li, Junjie Yao, Chong Ma, Xiang Li, Dajiang Zhu, Xi Jiang, Junwei Han, Dinggang Shen, Tianming Liu, Tuo Zhang.* [[abs](https://arxiv.org/abs/2304.11107)], 2023.4

15. **Is ChatGPT a Good Causal Reasoner? A Comprehensive Evaluation.**
 
    *Jinglong Gao, Xiao Ding, Bing Qin, Ting Liu.* [[abs](https://arxiv.org/abs/2305.07375)],[[github](https://github.com/ArrogantL/ChatGPT4CausalReasoning)] 2023.5

16. **StructGPT: A General Framework for Large Language Model to Reason over Structured Data.**
 
    *Jinhao Jiang, Kun Zhou, Zican Dong, Keming Ye, Wayne Xin Zhao, Ji-Rong Wen.* [[abs](https://arxiv.org/abs/2305.09645)], 2023.5

17. **Chain-of-Symbol Prompting Elicits Planning in Large Langauge Models.**
 
    *Hanxu Hu, Hongyuan Lu, Huajian Zhang, Wai Lam, Yue Zhang.* [[abs](https://arxiv.org/abs/2305.10276)], 2023.5

18. **Tree of Thoughts: Deliberate Problem Solving with Large Language Models.**
 
    *Shunyu Yao, Dian Yu, Jeffrey Zhao, Izhak Shafran, Thomas L. Griffiths, Yuan Cao, Karthik Narasimhan.* [[abs](https://arxiv.org/abs/2305.10276)],[[github](https://github.com/ysymyth/tree-of-thought-llm)] 2023.5

19. **Chain of Knowledge: A Framework for Grounding Large Language Models with Structured Knowledge Bases.**
 
    *Xingxuan Li, Ruochen Zhao, Yew Ken Chia, Bosheng Ding, Lidong Bing, Shafiq Joty, Soujanya Poria.* [[abs](https://arxiv.org/abs/2305.13269)], 2023.5

20. **Adaptive Chameleon or Stubborn Sloth: Unraveling the Behavior of Large Language Models in Knowledge Conflicts.**
 
    *Jian Xie, Kai Zhang, Jiangjie Chen, Renze Lou, Yu Su.* [[abs](https://arxiv.org/abs/2305.13300)], 2023.5

21. **Can ChatGPT Defend the Truth? Automatic Dialectical Evaluation Elicits LLMs' Deficiencies in Reasoning.**
 
    *Boshi Wang, Xiang Yue, Huan Sun.* [[abs](https://arxiv.org/abs/2305.13160)], 2023.5

22. **GPT-3.5 vs GPT-4: Evaluating ChatGPT's Reasoning Performance in Zero-shot Learning.**
 
    *Jessica López Espejel, El Hassane Ettifouri, Mahaman Sanoussi Yahaya Alassan, El Mehdi Chouham, Walid Dahhane.* [[abs](https://arxiv.org/abs/2305.12477)], 2023.5

23. **LogiCoT: Logical Chain-of-Thought Instruction-Tuning Data Collection with GPT-4.**
 
    *Hanmeng Liu, Zhiyang Teng, Leyang Cui, Chaoli Zhang, Qiji Zhou, Yue Zhang.* [[abs](https://arxiv.org/abs/2305.12147)], 2023.5

24. **Enabling Large Language Models to Generate Text with Citations.**
 
    *Tianyu Gao, Howard Yen, Jiatong Yu, Danqi Chen.* [[abs](https://arxiv.org/abs/2305.14627)],[[github](https://github.com/princeton-nlp/ALCE)] 2023.5

25. **Why Does ChatGPT Fall Short in Providing Truthful Answers?**
 
    *Shen Zheng, Jie Huang, Kevin Chen-Chuan Chang.* [[abs](https://arxiv.org/abs/2304.10513)], 2023.4
    
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
   
9. **How does ChatGPT rate sound semantics?**

   *Kai Siedenburg, Charalampos Saitis.* [[abs](https://arxiv.org/abs/2304.07830)], 2023.4

10. **MultiModal-GPT: A Vision and Language Model for Dialogue with Humans.**

    *Tao Gong, Chengqi Lyu, Shilong Zhang, Yudong Wang, Miao Zheng, Qian Zhao, Kuikun Liu, Wenwei Zhang, Ping Luo, Kai Chen.* [[abs](https://arxiv.org/abs/2305.04790)], [[github](https://github.com/open-mmlab/Multimodal-GPT)], 2023.5
 
11. **LLMScore: Unveiling the Power of Large Language Models in Text-to-Image Synthesis Evaluation.**

    *Yujie Lu, Xianjun Yang, Xiujun Li, Xin Eric Wang, William Yang Wang.* [[abs](https://arxiv.org/abs/2305.11116)], [[github](https://github.com/YujieLu10/LLMScore)], 2023.5

12. **ChatBridge: Bridging Modalities with Large Language Model as a Language Catalyst.**

    *Zijia Zhao, Longteng Guo, Tongtian Yue, Sihan Chen, Shuai Shao, Xinxin Zhu, Zehuan Yuan, Jing Liu.* [[abs](https://arxiv.org/abs/2305.16103)], [[github](https://iva-chatbridge.github.io/)], 2023.5
    
13. **GPT4GEO: How a Language Model Sees the World's Geography.**

    *Jonathan Roberts, Timo Lüddecke, Sowmen Das, Kai Han, Samuel Albanie.* [[abs](https://arxiv.org/abs/2306.00020)], 2023.6
    
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

6. **ChatGPT vs State-of-the-Art Models: A Benchmarking Study in Keyphrase Generation Task.**

   *Roberto Martínez-Cruz, Alvaro J. López-López, José Portela.* [[abs](https://arxiv.org/abs/2304.14177)], 2023.4

7. **Evaluating ChatGPT's Information Extraction Capabilities: An Assessment of Performance, Explainability, Calibration, and Faithfulness.**

   *Bo Li, Gexiang Fang, Yang Yang, Quansen Wang, Wei Ye, Wen Zhao, Shikun Zhang.* [[abs](https://arxiv.org/abs/2304.11633)], 2023.4

8. **ChatGPT Evaluation on Sentence Level Relations: A Focus on Temporal, Causal, and Discourse Relations.**

   *Chunkit Chan, Jiayang Cheng, Weiqi Wang, Yuxin Jiang, Tianqing Fang, Xin Liu, Yangqiu Song.* [[abs](https://arxiv.org/abs/2304.14827)], 2023.4
   
9. **Using ChatGPT for Entity Matching.**

   *Ralph Peeters, Christian Bizer.* [[abs](https://arxiv.org/abs/2305.03423)], 2023.5

10. **LLMs for Knowledge Graph Construction and Reasoning: Recent Capabilities and Future Opportunities.**

    *Yuqi Zhu, Xiaohan Wang, Jing Chen, Shuofei Qiao, Yixin Ou, Yunzhi Yao, Shumin Deng, Huajun Chen, Ningyu Zhang.* [[abs](https://arxiv.org/abs/2305.13168)], [[github](https://github.com/zjunlp/AutoKG)], 2023.5

11. **Prompt ChatGPT In MNER: Improved multimodal named entity recognition method based on auxiliary refining knowledge from ChatGPT.**

    *Jinyuan Li, Han Li, Zhuo Pan, Gang Pan.* [[abs](https://arxiv.org/abs/2305.12212)], 2023.5

12. **STAR: Boosting Low-Resource Event Extraction by Structure-to-Text Data Generation with Large Language Models.**

    *Mingyu Derek Ma, Xiaoxuan Wang, Po-Nien Kung, P. Jeffrey Brantingham, Nanyun Peng, Wei Wang.* [[abs](https://arxiv.org/abs/2305.15090)]  2023.5

13. **Aligning Instruction Tasks Unlocks Large Language Models as Zero-Shot Relation Extractors.**

    *Kai Zhang, Bernal Jiménez Gutiérrez, Yu Su.* [[abs](https://arxiv.org/abs/2305.11159)], 2023.5

### 2.7 Machine Translation

1. **Is ChatGPT A Good Translator? A Preliminary Study.**

   *Wenxiang Jiao, Wenxuan Wang, Jen-tse Huang, Xing Wang, Zhaopeng Tu.* [[abs](https://arxiv.org/abs/2301.08745v2)],[[github](https://github.com/wxjiao/Is-ChatGPT-A-Good-Translator)], 2023.1
   
2. **Error Analysis Prompting Enables Human-Like Translation Evaluation in Large Language Models: A Case Study on ChatGPT.**

   *Qingyu Lu, Baopu Qiu, Liang Ding, Liping Xie, Dacheng Tao.* [[abs](https://arxiv.org/abs/2303.13809)],[[github](https://github.com/Coldmist-Lu/ErrorAnalysis_Prompt)], 2023.3

3. **Towards Making the Most of ChatGPT for Machine Translation.**

   *Keqin Peng, Liang Ding, Qihuang Zhong, Li Shen, Xuebo Liu, Min Zhang, Yuanxin Ouyang, Dacheng Tao.* [[abs](https://arxiv.org/abs/2303.13780)],[[github](https://github.com/Romainpkq/ChatGPT4MT)], 2023.3
   
4. **Linguistically Informed ChatGPT Prompts to Enhance Japanese-Chinese Machine Translation: A Case Study on Attributive Clauses.**

   *Wenshi Gu.* [[abs](https://arxiv.org/abs/2303.15587)], 2023.3

5. **Unleashing the Power of ChatGPT for Translation: An Empirical Study.**

   *Yuan Gao, Ruili Wang, Feng Hou.* [[abs](https://arxiv.org/abs/2304.02182)], 2023.4

6. **Large language models effectively leverage document-level context for literary translation, but critical errors persist.**

   *Marzena Karpinska, Mohit Iyyer.* [[abs](https://arxiv.org/abs/2304.03245)],[[github](https://github.com/marzenakrp/LiteraryTranslation)], 2023.4

7. **ChatGPT Beyond English: Towards a Comprehensive Evaluation of Large Language Models in Multilingual Learning.**

   *Viet Dac Lai, Nghia Trung Ngo, Amir Pouran Ben Veyseh, Hieu Man, Franck Dernoncourt, Trung Bui, Thien Huu Nguyen.* [[abs](https://arxiv.org/abs/2304.05613)], 2023.4

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

9. **Evaluation of ChatGPT Family of Models for Biomedical Reasoning and Classification.**

   *Shan Chen, Yingya Li, Sheng Lu, Hoang Van, Hugo JWL Aerts, Guergana K. Savova, Danielle S. Bitterman.* [[abs](https://arxiv.org/abs/2304.02496#)], 2023.4


10. **ChatGPT for Shaping the Future of Dentistry: The Potential of Multi-Modal Large Language Model.**

    *Hanyao Huang, Ou Zheng, Dongdong Wang, Jiayi Yin, Zijin Wang, Shengxuan Ding, Heng Yin, Chuan Xu, Renjie Yang, Qian Zheng, Bing Shi.* [[abs](https://arxiv.org/abs/2304.03086)], 2023.4

11. **On the Evaluations of ChatGPT and Emotion-enhanced Prompting for Mental Health Analysis.**

    *Kailai Yang, Shaoxiong Ji, Tianlin Zhang, Qianqian Xie, Sophia Ananiadou.* [[abs](https://arxiv.org/abs/2304.03347)], 2023.4

12. **ImpressionGPT: An Iterative Optimizing Framework for Radiology Report Summarization with ChatGPT.**

    *Chong Ma, Zihao Wu, Jiaqi Wang, Shaochen Xu, Yaonai Wei, Zhengliang Liu, Lei Guo, Xiaoyan Cai, Shu Zhang, Tuo Zhang, Dajiang Zhu, Dinggang Shen, Tianming Liu, Xiang Li.* [[abs](https://arxiv.org/abs/2304.08448)], 2023.4

13. **Evaluation of GPT-3.5 and GPT-4 for supporting real-world information needs in healthcare delivery.**

    *Debadutta Dash, Rahul Thapa, Juan M. Banda, Akshay Swaminathan, Morgan Cheatham, Mehr Kashyap, Nikesh Kotecha, Jonathan H. Chen, Saurabh Gombar, Lance Downing, Rachel Pedreira, Ethan Goh, Angel Arnaout, Garret Kenn Morris, Honor Magon, Matthew P Lungren, Eric Horvitz, Nigam H. Shah.* [[abs](https://arxiv.org/abs/2304.13714)], 2023.4

14. **Retrieval Augmented Chest X-Ray Report Generation using OpenAI GPT models.**

    *Mercy Ranjit, Gopinath Ganapathy, Ranjit Manuel, Tanuja Ganu.* [[abs](https://arxiv.org/abs/2305.03660)], 2023.5

15. **MedGPTEval: A Dataset and Benchmark to Evaluate Responses of Large Language Models in Medicine.**

    *Jie Xu, Lu Lu, Sen Yang, Bilin Liang, Xinwei Peng, Jiali Pang, Jinru Ding, Xiaoming Shi, Lingrui Yang, Huan Song, Kang Li, Xin Sun, Shaoting Zhang.* [[abs](https://arxiv.org/abs/2305.07340)], 2023.5

16. **HuatuoGPT, towards Taming Language Model to Be a Doctor.**

    *Hongbo Zhang, Junying Chen, Feng Jiang, Fei Yu, Zhihong Chen, Jianquan Li, Guiming Chen, Xiangbo Wu, Zhiyi Zhang, Qingying Xiao, Xiang Wan, Benyou Wang, Haizhou Li.* [[abs](https://arxiv.org/abs/2305.15075)], [[github](https://github.com/FreedomIntelligence/HuatuoGPT)], 2023.5

17. **Empowering Molecule Discovery for Molecule-Caption Translation with Large Language Models: A ChatGPT Perspective.**

    *Jiatong Li, Yunqing Liu, Wenqi Fan, Xiao-Yong Wei, Hui Liu, Jiliang Tang, Qing Li.* [[abs](https://arxiv.org/abs/2306.06615)],[[github](https://github.com/phenixace/MolReGPT)] 2023.6

#### Psychology


1. **Is GPT-3 a Psychopath? Evaluating Large Language Models from a Psychological Perspective.**

   *Xingxuan Li, Yutong Li, Linlin Liu, Lidong Bing, Shafiq Joty.* [[abs](https://arxiv.org/abs/2212.10529)], 2022.12

2. **Theory of Mind May Have Spontaneously Emerged in Large Language Models.**

   *Michal Kosinski.* [[abs](https://arxiv.org/abs/2302.02083)], 2023.2

3. **Can ChatGPT Assess Human Personalities? A General Evaluation Framework.**

   *Haocong Rao, Cyril Leung, Chunyan Miao.* [[abs](https://arxiv.org/abs/2303.01248)][[github](https://github.com/Kali-Hac/ChatGPT-MBTI)], 2023.3
   
4. **Will Affective Computing Emerge from Foundation Models and General AI? A First Evaluation on ChatGPT.**

   *Mostafa M. Amin, Erik Cambria, Björn W. Schuller.* [[abs](https://arxiv.org/abs/2303.03186)], 2023.3
   
5. **What does ChatGPT return about human values? Exploring value bias in ChatGPT using a descriptive value theory.**

   *Ronald Fischer, Markus Luczak-Roesch, Johannes A Karl.* [[abs](https://arxiv.org/abs/2304.03612)], 2023.4

6. **Is ChatGPT Equipped with Emotional Dialogue Capabilities?**

   *Weixiang Zhao, Yanyan Zhao, Xin Lu, Shilong Wang, Yanpeng Tong, Bing Qin.* [[abs](https://arxiv.org/abs/2304.09582)], 2023.4

7. **Assessing Working Memory Capacity of ChatGPT.**

   *Dongyu Gong.* [[abs](https://arxiv.org/abs/2305.03731)], 2023.5

8. **Do Large Language Models Show Decision Heuristics Similar to Humans? A Case Study Using GPT-3.5.**

   *Gaurav Suri, Lily R. Slater, Ali Ziaee, Morgan Nguyen.* [[abs](https://arxiv.org/abs/2305.04400)], 2023.5

9. **ChatGPT is fun, but it is not funny! Humor is still challenging Large Language Models.**

   *Sophie Jentzsch, Kristian Kersting.* [[abs](https://arxiv.org/abs/2306.04563)], 2023.6

10. **Can LLMs like GPT-4 outperform traditional AI tools in dementia diagnosis? Maybe, but not today.**
 
    *Zhuo Wang, Rongzhen Li, Bowen Dong, Jie Wang, Xiuxing Li, Ning Liu, Chenhui Mao, Wei Zhang, Liling Dong, Jing Gao, Jianyong Wang.* [[abs](https://arxiv.org/abs/2306.01499)], 2023.6

#### Code

1. **SelfEvolve: A Code Evolution Framework via Large Language Models.**

   *Shuyang Jiang, Yuhao Wang, Yu Wang.* [[abs](https://arxiv.org/abs/2306.02907)], 2023.6

#### Finance

1. **FinGPT: Open-Source Financial Large Language Models.**

   *Hongyang Yang, Xiao-Yang Liu, Christina Dan Wang.* [[abs](https://arxiv.org/abs/2306.06031)],[[github](https://github.com/AI4Finance-Foundation/FinGPT)], 2023.6
   
#### Law

1. **Chatgpt goes to law school.**

   *Teo Susnjak.* [[abs](https://papers.ssrn.com/sol3/papers.cfm?abstract_id=4335905)], 2023


#### Game

1. **Can Large Language Models Play Text Games Well? Current State-of-the-Art and Open Questions.**

   *Chen Feng Tsai, Xiaochen Zhou, Sierra S. Liu, Jing Li, Mo Yu, Hongyuan Mei.* [[abs](https://arxiv.org/abs/2304.02868)], 2023.4


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
   
7. **Human-like Summarization Evaluation with ChatGPT.**

   *Mingqi Gao, Jie Ruan, Renliang Sun, Xunjian Yin, Shiping Yang, Xiaojun Wan.* [[abs](https://arxiv.org/abs/2304.02554)], 2023.4

8. **Can ChatGPT and Bard Generate Aligned Assessment Items? A Reliability Analysis against Human Performance.**

   *Abdolvahab Khademi.* [[abs](https://arxiv.org/abs/2304.05372)], 2023.4
 
9. **Multidimensional Evaluation for Text Style Transfer Using ChatGPT.**

   *Huiyuan Lai, Antonio Toral, Malvina Nissim.* [[abs](https://arxiv.org/abs/2304.13462)], 2023.4

10. **Re-visiting Automated Topic Model Evaluation with Large Language Models.**

    *Dominik Stammbach, Vilém Zouhar, Alexander Hoyle, Mrinmaya Sachan, Elliott Ash.* [[abs](https://arxiv.org/abs/2305.12152)],[[github](https://github.com/dominiksinsaarland/evaluating-topic-model-output)], 2023.5
 
11. **Benchmarking Foundation Models with Language-Model-as-an-Examiner.**

    *Yushi Bai, Jiahao Ying, Yixin Cao, Xin Lv, Yuze He, Xiaozhi Wang, Jifan Yu, Kaisheng Zeng, Yijia Xiao, Haozhe Lyu, Jiayin Zhang, Juanzi Li, Lei Hou.* [[abs](https://arxiv.org/abs/2306.04181)],[[website](https://lmexam.com/)], 2023.6
    
#### Metrics for detecting ChatGPT

1. **AI vs. Human -- Differentiation Analysis of Scientific Content Generation.**

   *Yongqiang Ma, Jiawei Liu, Fan Yi, Qikai Cheng, Yong Huang, Wei Lu, Xiaozhong Liu.* [[abs](https://arxiv.org/abs/2301.10416)], 2023.1


2. **ChatGPT or academic scientist? Distinguishing authorship with over 99% accuracy using off-the-shelf machine learning tools.**

   *Heather Desaire, Aleesa E. Chua, Madeline Isom, Romana Jarosova, David Hua.* [[abs](https://arxiv.org/abs/2303.16352)], 2023.3


3. **Distinguishing ChatGPT(-3.5, -4)-generated and human-written papers through Japanese stylometric analysis.**

   *Wataru Zaitsu, Mingzhe Jin.* [[abs](https://arxiv.org/abs/2304.05534)], 2023.4

4. **ArguGPT: evaluating, understanding and identifying argumentative essays generated by GPT models.**

   *Yikang Liu, Ziyin Zhang, Wanyang Zhang, Shisen Yue, Xiaojing Zhao, Xinyuan Cheng, Yiwen Zhang, Hai Hu.* [[abs](https://arxiv.org/abs/2304.07666)],[[github](https://github.com/huhailinguist/ArguGPT)],[[data](https://github.com/huhailinguist/ArguGPT/tree/main/data/argugpt)], 2023.4
   
5. **Origin Tracing and Detecting of LLMs.**

   *Linyang Li, Pengyu Wang, Ke Ren, Tianxiang Sun, Xipeng Qiu.* [[abs](https://arxiv.org/abs/2304.14072)], 2023.4

6. **AI, write an essay for me: A large-scale comparison of human-written versus ChatGPT-generated essays.**

   *Steffen Herbold, Annette Hautli-Janisz, Ute Heuer, Zlata Kikteva, Alexander Trautsch.* [[abs](https://arxiv.org/abs/2304.14276)], 2023.4
   
7. **CHEAT: A Large-scale Dataset for Detecting ChatGPT-writtEn AbsTracts.**

   *Peipeng Yu, Jiahan Chen, Xuan Feng, Zhihua Xia.* [[abs](https://arxiv.org/abs/2304.12008)], 2023.4

8. **Differentiate ChatGPT-generated and Human-written Medical Texts.**

   *Wenxiong Liao, Zhengliang Liu, Haixing Dai, Shaochen Xu, Zihao Wu, Yiyang Zhang, Xiaoke Huang, Dajiang Zhu, Hongmin Cai, Tianming Liu, Xiang Li.* [[abs](https://arxiv.org/abs/2304.11567)], 2023.4
   
9. **Bot or Human? Detecting ChatGPT Imposters with A Single Question.**

   *Hong Wang, Xuan Luo, Weizhi Wang, Xifeng Yan.* [[abs](https://arxiv.org/abs/2305.06424)],[[github](https://github.com/hongwang600/FLAIR)], 2023.5
 
10. **GPT-Sentinel: Distinguishing Human and ChatGPT Generated Content.**

    *Yutian Chen, Hao Kang, Vivian Zhai, Liangze Li, Rita Singh, Bhiksha Ramakrishnan.* [[abs](https://arxiv.org/abs/2305.07969)], 2023.5

11. **Large Language Models can be Guided to Evade AI-Generated Text Detection.**

    *Ning Lu, Shengcai Liu, Rui He, Ke Tang.* [[abs](https://arxiv.org/abs/2305.10847)], 2023.5

12. **G3Detector: General GPT-Generated Text Detector.**

    *Haolan Zhan, Xuanli He, Qiongkai Xu, Yuxiang Wu, Pontus Stenetorp.* [[abs](https://arxiv.org/abs/2305.12680)], 2023.5

13. **GPT Paternity Test: GPT Generated Text Detection with GPT Genetic Inheritance.**

    *Xiao Yu, Yuang Qi, Kejiang Chen, Guoqiang Chen, Xi Yang, Pengyuan Zhu, Weiming Zhang, Nenghai Yu.* [[abs](https://arxiv.org/abs/2305.12519)], 2023.5

14. **On the Reliability of Watermarks for Large Language Models.**

    *John Kirchenbauer, Jonas Geiping, Yuxin Wen, Manli Shu, Khalid Saifullah, Kezhi Kong, Kasun Fernando, Aniruddha Saha, Micah Goldblum, Tom Goldstein.* [[abs](https://arxiv.org/abs/2306.04634)], 2023.6

15. **Implementing BERT and fine-tuned RobertA to detect AI generated news by ChatGPT.**

    *Zecong Wang, Jiaxi Cheng, Chen Cui, Chenhao Yu.* [[abs](https://arxiv.org/abs/2306.07401)], 2023.6

16. **Towards a Robust Detection of Language Model Generated Text: Is ChatGPT that Easy to Detect?**

    *Wissam Antoun, Virginie Mouilleron, Benoît Sagot, Djamé Seddah.* [[abs](https://arxiv.org/abs/2306.05871)], 2023.6


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
