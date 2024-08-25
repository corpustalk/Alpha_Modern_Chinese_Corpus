
# The Alpha Modern Chinese Corpus

Lei Lei, Ning Zhao

Shanghai International Studies University



## Abstract

In this short piece, we introduce our newly developed corpus entitled The Alpha Modern Chinese Corpus (the AMC corpus). The AMC corpus contains texts of four genres, i.e., nonfictions, fictions, scientific articles, and conversations. The corpus is a balanced collection of texts spanning diverse genres, making it a valuable resource for studying modern Chinese. Its applications are wide-ranging, including linguistic research, Chinese language teaching, and Natural Language Processing. The corpus is available at: https://github.com/corpustalk/Alpha_Modern_Chinese_Corpus/

**Download the data at: https://github.com/corpustalk/Alpha_Modern_Chinese_Corpus/releases
**

## 1 Description

The Alpha Modern Chinese Corpus (The AMC Corpus) is a corpus that contains a collection of “clean” modern Chinese sentences. By “clean” sentences, we mean the corpus is comprised of sentences with minimal numbers, non-Chinese alphabets, or special tokens.

The data in the AMC corpus primarily originate from publicly available online data, which is copyrighted. To avoid copyright issues, we intentionally provide only sentences instead of full texts. This allows us to release the entire corpus for research and educational purposes. It is important to emphasize that the corpus is intended solely for research and educational use and cannot be used for commercial purposes.

The sentences in the AMC Corpus are of four genres of texts, i.e., nonfictions, fictions, scientific articles, and conversations. 

To summarize, the AMC corpus is a balanced collection of texts spanning diverse genres, making it a valuable resource for studying modern Chinese. Its applications are wide-ranging, including:

1.	Linguistic research: Analyzing the nuances of the Chinese language.

2.	Language teaching: Providing authentic materials for second/foreign language learners of Chinese.

3.	Natural Language Processing: Training and evaluating algorithms for tasks such as text generation and sentiment analysis.

## 2 Corpus size 


We provide four versions of the AMC corpus of different sizes, i.e., mini, base, standard, and full. The corpus size of each version of the AMC corpus is described in Tables 1-3. 


**Table 1 Corpus size: number of sentences**


|Mini|Base|Standard|Full|

| --- | --- |--- |--- |

|Conversations|100K|500K|1M|2M|

|Fictions|100K|500K|1M|2M|

|Nonfictions|100K|500K|1M|2M|

|Scientific articles|100K|200K|500K|800K|

|Total|400K|1.7M|3.5M|6.8M|


**Table 2 Corpus size: number of characters**

	Mini	Base	Standard	Full
 
Conversations	1,589,381	7,950,279	15,919,381	31,799,521

Fictions	4,156,324	20,758,034	41,558,260	83,150,103

Nonfictions	7,143,168	35,758,578	71,532,808	143,123,338

Scientific articles	6,690,418	13,375,121	15,919,381	53,472,147

Total	19,579,291	77,842,012	144,929,830	311,545,109


**Table 3 Corpus size: number of words**

	Mini	Base	Standard	Full
 
Conversations	1,082,226	5,411,351	10,833,340	21,634,055

Fictions	2,807,601	14,015,800	28,062,666	56,148,142

Nonfictions	4,338,197	21,721,033	43,450,322	86,926,486

Scientific articles	3,732,809	7,463,840	18,665,244	29,830,970

Total	11,960,833	48,612,024	101,011,572	194,539,653



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


##  一、简介
阿尔法现代汉语语料库（The Alpha Modern Chinese Corpus，简称AMC语料库）是一个由“干净”的现代汉语句子组成的语料库。所谓 “干净”的句子，是指该语料库中的句子会尽可能少地包含数字、非汉字字母或特殊符号。

AMC语料库中的数据集主要来源于公开的在线数据，这些数据受版权保护。为了避免版权问题，我们有意仅提供句子而不是完整文本。这使得我们能够发布完整的语料库用于研究和教育之用。需要强调的是，AMC语料库仅限于研究和教育用途，禁止用于任何商业目的。

AMC语料库涵盖四种类型的文本，即非虚构文本、小说、学术论文和对话。

总体来看，AMC语料库一个涵盖多种体裁的平衡语料库，是研究现代汉语的宝贵资源。其应用范围十分广泛，包括：

1.	语言学研究： 用于分析汉语的细微差别。

2.	语言教学：为第二语言/外语学习者提供真实的汉语教学材料。

3.	自然语言处理： 训练和评估文本生成和情感分析等任务的算法。

##  二、语料库大小

我们提供了四个不同大小的 AMC 语料库版本，即迷你版、基础版、标准版和完整版。AMC 语料库每版本库容见表1-3。
 

**表1 AMC语料库库容：句子数**
	迷你版	基础版	标准版	完整版

对话	100K	500K	1M	2M

小说	100K	500K	1M	2M

非虚构	100K	500K	1M	2M

学术文章	100K	200K	500K	800K

总计	400K	1.7M	3.5M	6.8M

**表2 AMC语料库库容：字符数/汉字数(含标点)**

	迷你版	基础版	标准版	完整版

对话	1,589,381	7,950,279	15,919,381	31,799,521

小说	4,156,324	20,758,034	41,558,260	83,150,103

非虚构	7,143,168	35,758,578	71,532,808	143,123,338

学术文章	6,690,418	13,375,121	15,919,381	53,472,147

总计	19,579,291	77,842,012	144,929,830	311,545,109


**表3 AMC语料库库容：单词数(含标点)**

	迷你版	基础版	标准版	完整版

对话	1,082,226	5,411,351	10,833,340	21,634,055

小说	2,807,601	14,015,800	28,062,666	56,148,142

非虚构	4,338,197	21,721,033	43,450,322	86,926,486

学术文章	3,732,809	7,463,840	18,665,244	29,830,970

总计	11,960,833	48,612,024	101,011,572	194,539,653





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


