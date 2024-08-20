
# The Alpha Modern Chinese Corpus

Lei Lei, Ning Zhao

Shanghai International Studies University

leileicn@126.com; ningzhao_nz@126.com


## Abstract

In this short piece, we introduce our newly developed corpus entitled The Alpha Modern Chinese Corpus (the AMC corpus). The AMC corpus contains texts of four genres, i.e., nonfictions, fictions, scientific articles, and conversations. The corpus is a balanced collection of texts spanning diverse genres, making it a valuable resource for studying modern Chinese. Its applications are wide-ranging, including linguistic research, Chinese language teaching, and Natural Language Processing. The corpus is available at: https://github.com/corpustalk/Alpha_Modern_Chinese_Corpus/

## 1 Description

The Alpha Modern Chinese Corpus (The AMC Corpus) is a corpus that contains a collection of “clean” modern Chinese sentences. By “clean” sentences, we mean the corpus is comprised of sentences with minimal numbers, non-Chinese alphabets, or special tokens.

The data in the AMC corpus primarily originate from publicly available online data, which is copyrighted. To avoid copyright issues, we intentionally provide only sentences instead of full texts. This allows us to release the entire corpus for research and educational purposes. It is important to emphasize that the corpus is intended solely for research and educational use and cannot be used for commercial purposes.

The sentences in the AMC Corpus are of four genres of texts, i.e., nonfictions, fictions, scientific articles, and conversations. 

To summarize, the AMC corpus is a balanced collection of texts spanning diverse genres, making it a valuable resource for studying modern Chinese. Its applications are wide-ranging, including:

1.	Linguistic research: Analyzing the nuances of the Chinese language.

2.	Language teaching: Providing authentic materials for second/foreign language learners of Chinese.

3.	Natural Language Processing: Training and evaluating algorithms for tasks such as text generation and sentiment analysis.

## 2 Corpus size 

We provide four versions of the AMC corpus of different sizes, i.e., mini, base, standard, and full. The number of sentences that each version of the AMC corpus contains is described in Table 1. 

Table 1 Number of sentences that each version of AMC contains


Versions	Nonfictions	Fictions	Scientific articles	Conversations

Mini	100K	100K	100K	100K

Base	500K	500K	200K	500K

Standard	1M	1M	500K	1M

Full	2M	2M	800K	2M

Total	3.6M	3.6M	1.6M	3.6M


## 3 Development of the corpus

To develop the AMC Corpus, we extracted the data from the source data and cleaned the data with the following steps:

1.	Download the data;

2.	Remove lines/sentences in traditional Chinese with the Python tool: hanzidentifier;

3.	Remove lines/sentences with sensitive words, particularly sentences with pornographic/adult content. The sensitive words are words listed in https://github.com/57ing/Sensitive-word;

4.	Deduplicate lines/sentences;

5.	Sample the number of sentences as described in Table 1;

6.	Randomly scramble the order of the sentences. 

## 4 Source of the data

### 4.1 Nonfictions

The data of the nonfictions section consists of sampled sentences from the chinese_clean_passages_80m dataset  (Guo et al., 2022) ), which itself was sampled from the dataset ClueCorpus 2020  (Xu, 2019). 

It also should be noted that the dataset CLUE Corpus 2020 includes texts from news (news2016zh_corpus), wikipedia articles (wiki2019zh_corpus), Reddit-like Q&As (webText2019zh_corpus), and comments from e-commerce sites such as Amazon and Dazhong Dianping (comments2019zh_corpus). 

### 4.2 Fictions

The fictions section includes three genres of texts: novels by Chinese writers, translated works by foreign authors, and web novels by Chinese writers. The data of the novels by Chinese writers and the translated works by foreign authors were sourced from an online collection that we assembled through web crawling. In addition, the web novels by Chinese writers were sampled from the dataset Chinese Web Novels .


### 4.3 Scientific articles

The data of the scientific articles section were sampled from the Chinese Scientific Literature Dataset (Li et al., 2022). The dataset contains sentences from scientific abstracts of various disciplines such as sciences, engineering, social sciences, and arts and humanities.  

### 4.4 Conversations

The data of the conversations section were sampled from the dataset Large-scale Cleaned Chinese Conversation (LCCC) (Wang et al., 2020). The LCCC dataset includes conversations from Weibo (the Chinese Twitter) and spontaneous conversations. 

## References

Guo, B., Gong, Y., Shen, Y., Han, S., Huang, H., Duan, N., & Chen, W. (2022). GENIUS: sketch-based language model pre-training via extreme and selective masking for text generation and augmentation. arXiv Preprint arXiv:2211.10330.

Li, Y., Zhang, Y., Zhao, Z., Shen, L., Liu, W., Mao, W., & Zhang, H. (2022). CSL: A Large-scale Chinese Scientific Literature Dataset. Proceedings of the 29th International Conference on Computational Linguistics, 3917–3923. https://aclanthology.org/2022.coling-1.344

Wang, Y., Ke, P., Zheng, Y., Huang, K., Jiang, Y., Zhu, X., & Huang, M. (2020). A large-scale Chinese short-text conversation dataset. NLPCC. https://arxiv.org/abs/2008.03946

Xu, B. (2019). NLP Chinese Corpus: Large scale Chinese corpus for NLP (Version 1.0). Zenodo. https://doi.org/10.5281/zenodo.3402023

***

# 阿尔法现代汉语语料库


雷蕾，赵宁


上海外国语大学

leileicn@126.com; ningzhao_nz@126.com

##  一、简介
阿尔法现代汉语语料库（The Alpha Modern Chinese Corpus，简称AMC语料库）是一个由“干净”的现代汉语句子组成的语料库。所谓 “干净”的句子，是指该语料库中的句子会尽可能少地包含数字、非汉字字母或特殊符号。

AMC语料库中的数据集主要来源于公开的在线数据，这些数据受版权保护。为了避免版权问题，我们有意仅提供句子而不是完整文本。这使得我们能够发布完整的语料库用于研究和教育之用。需要强调的是，AMC语料库仅限于研究和教育用途，禁止用于任何商业目的。

AMC语料库涵盖四种类型的文本，即非虚构文本、小说、学术论文和对话。

总体来看，AMC语料库一个涵盖多种体裁的平衡语料库，是研究现代汉语的宝贵资源。其应用范围十分广泛，包括：

1.	语言学研究： 用于分析汉语的细微差别。

2.	语言教学：为第二语言/外语学习者提供真实的汉语教学材料。

3.	自然语言处理： 训练和评估文本生成和情感分析等任务的算法。

##  二、语料库大小

我们提供了四个不同大小的 AMC 语料库版本，即迷你版、基础版、标准版和完整版。每个版本的 AMC 语料库包含的句子数量如表格1所示。
 

表格1 不同版本的AMC语料库包含的句子数量

版本	非虚构	小说	学术文章	对话

迷你版	100K	100K	100K	100K

基础版	500K	500K	200K	500K

标准版	1M	1M	500K	1M

完整版	2M	2M	800K	2M

总计	3.6M	3.6M	1.6M	3.6M

##  三、语料库开发

为了开发AMC语料库，我们从源数据中提取数据，并通过以下步骤进行清理：

1.	下载数据；

2.	使用 Python 工具：hanzidentifier 删除繁体中文行/句；

3.	删除包含敏感词的行/句，尤其是包含色情/成人内容的句子。敏感词表由https://github.com/57ing/Sensitive-word提供；

4.	删除重复的行/句；

5.	按照表格1所述的句子数量进行抽样；

6.	随机打乱句子顺序。

## 四、数据来源

### 1. 非虚构文本

非虚构文本的数据由chinese_clean_passages_80m 数据集中抽样的句子组成，而该数据集本身是从ClueCorpus 2020数据集 中抽样所得（Xu，2019）。需要注意的是，CLUE Corpus 2020数据集中的文本来自于新闻（news2016zh_corpus）、维基百科文章（wiki2019zh_corpus）、类似Reddit平台的问答帖子（webText2019zh_corpus）以及电商网站（如亚马逊和大众点评）的评论（comments2019zh_corpus）。

### 2. 小说

小说部分包括三种体裁的文本：中国作者的小说、外国作者的译著以及中国作者的网络小说。中国作者的小说和外国作者的译著数据来自于我们通过网络爬虫收集的在线资料。此外，中国作者的网络小说数据来自于“中文网络小说”数据集 。

### 3. 学术论文

学术论文部分的数据来自于“中文学术文献”数据集（Li等，2022）。该数据集包含了来自科学、工程、社会科学以及人文艺术等各个学科的摘要句子。

### 4. 对话

对话部分的数据取自“大规模清洁中文对话”数据集（LCCC）。LCCC数据集中的原始对话数据来自于微博（中文推特）对话和其他自发对话。


## 参考文献
Guo, B., Gong, Y., Shen, Y., Han, S., Huang, H., Duan, N., & Chen, W. (2022). GENIUS: sketch-based language model pre-training via extreme and selective masking for text generation and augmentation. arXiv Preprint arXiv:2211.10330.

Li, Y., Zhang, Y., Zhao, Z., Shen, L., Liu, W., Mao, W., & Zhang, H. (2022). CSL: A Large-scale Chinese Scientific Literature Dataset. Proceedings of the 29th International Conference on Computational Linguistics, 3917–3923. https://aclanthology.org/2022.coling-1.344

Wang, Y., Ke, P., Zheng, Y., Huang, K., Jiang, Y., Zhu, X., & Huang, M. (2020). A large-scale Chinese short-text conversation dataset. NLPCC. https://arxiv.org/abs/2008.03946

Xu, B. (2019). NLP Chinese Corpus: Large scale Chinese corpus for NLP (Version 1.0). Zenodo. https://doi.org/10.5281/zenodo.3402023


