# Information Retrieval

* Teachers: [Franco Maria Nardini](http://hpc.isti.cnr.it/~nardini/) and [Rossano Venturini](http://pages.di.unipi.it/rossano)
* CFU: 6
* Period: First semester
* Language: English
* Telegram group: [here](https://t.me/+h-ZRKyPTw_M1YmQ0)
* Teams group: [here](https://unipiit.sharepoint.com/:u:/r/sites/a__td_62942/SitePages/ClassHome.aspx?csf=1&web=1&share=EXQdcwM1E0pOl7BB2hZ2okkB3XSaeWIfdT6F4QrfaLqAKA&e=DDbwPa)
* Lectures schedule: Monday 11:00-13:00 (Aula Fib C) and Wednesday 11:00-13:00 (Aula Fib C1)
* Question time: After lectures or by appointment. The fastest way to contact us is by email or Telegram. Don't be shy!

### Overview of Course
This Information Retrieval (IR) course focuses on modern techniques and technologies that efficiently retrieve and rank relevant data. It covers both foundational concepts and cutting-edge advancements, providing students with a deep understanding of how to manage and retrieve information in various applications such as search engines, recommendation systems, and data management platforms. Here's a brief look at the course topics:

- **Language Properties and IR Models** – Introduction to how language and text are represented for retrieval, including traditional models (Boolean, vector space, and probabilistic) and modern IR models.
- **Effectiveness Measures** – Evaluation metrics like precision, recall, F1 score, mean reciprocal rank (MRR), and discounted cumulative gain (DCG) to measure IR system performance.
- **Efficiency with Modern CPUs** – Techniques to optimize IR systems to utilize modern CPUs, focusing on query processing and data retrieval speed.
- **Inverted Indexes and Query Processing** – Core indexing structures that allow fast lookups, including construction and optimization of inverted indexes for efficient query processing.
- **Data Compression** – Strategies for compressing indexes and data to save storage space while maintaining retrieval performance.
- **Learning-to-Rank (LTR)** – Machine learning models that rank documents based on relevance to queries. This involves feature extraction and model training to improve search results.
- **Efficient Inference of Learning-to-Rank Models** – Techniques to ensure that LTR models can be applied efficiently in large-scale, real-time environments.
- **Neural Information Retrieval** – Use of deep learning and neural networks to model semantic relevance and improve search capabilities beyond traditional methods.
- **Approximate k Nearest Neighbor (k-NN) Search** – Algorithms for quickly finding approximate nearest neighbors, useful for large-scale vector-based retrieval systems.


### Opportunities
Becoming an expert in Information Retrieval offers numerous career opportunities with major companies that rely on search, ranking, and recommendation systems. This includes roles at search engine giants like Google and Microsoft, e-commerce platforms like Amazon, eBay, and Alibaba, and media streaming services like Netflix and Spotify. Social media companies like Meta and LinkedIn also depend on IR expertise for content delivery and recommendations. 

### Exam
The exam consists of two parts. 

- **Part 1**: Written Exam (up to 22 points)
  - 1-hour written exam covering topics discussed during the course.
  - Questions will assess the understanding of the core course materials.

- **Part 2**: Oral Exam on a Project (up to 8 points)
  - The project is based on a scientific paper you choose from a [selected list of papers](https://github.com/rossanoventurini/IR-unipi/blob/main/papers.md).
  - The project can be completed by a team of up to 2 people.
  - The project will be presented using approximately 10 slides during the oral exam.
  - Students can approach the project at different levels of depth:
    - **Basic Level**: Read and understand the techniques presented in the article.
    - **Intermediate Level**: Conduct experiments to verify the assumptions, main properties,  or conclusions.
    - **Advanced Level**: Replicate the results from the article.
    - **Expert Level**: Re-implement the proposed solution, up to improving it by introducing alternative strategies.

#### Midterm and Final Exams
Registration via Google Form for every midterm is welcome. Check the Telegram channel for Google Form links.  You can take the final term only if your grade on the midterm is 18 or higher. If you fail the midterm, no worries! You can still take any of the exams in January, February, June, July, or September 2025!

| Date | Time | Room | Notes |
| :------------- | --------: | :--------- | :------- |
| 28/10/2024 | 11:00 -- 13:00 | Room C | |
| 11/12/2024 | 11:00 -- 13:00 | Room C | Take the final term only if your grade on the midterm is 18 or higher |

----
### Lectures

| Date | Lecture | 
| -------------: | :------------- |
| 16/09/2024 | **Introduction of the Course**. (FMN, RV)<br><br>Anatomy of a search engine. Main components and their interactions. General overview of the course. Final Exam. Question Time.<br><br>*References*:  *Introduction to Information Retrieval*, Christopher D. Manning, Prabhakar Raghavan and Hinrich Schütze, Cambridge University Press. 2008 ([link](https://nlp.stanford.edu/IR-book/)).|
| 18/09/2024 | **Evaluation in Information Retrieval**. (FMN)<br><br>How do we evaluate an IR system? Methodology and Goal. Relevance Assessment and Annotation Methodology. A bit of history and current efforts. Text REtrieval Conference. Binary evaluation metrics: Precision, Recall, F-Measure. F-Score. Rank-based evaluation metrics: MAP, AP, MRR, MAP@K, AP@K. Beyond Binary Relevance: Graded relevance feedback. DCG, NDCG.<br><br>*References*:  Chapter 8 in *Introduction to Information Retrieval*, Christopher D. Manning, Prabhakar Raghavan and Hinrich Schütze, Cambridge University Press. 2008 ([link](http://nlp.stanford.edu/IR-book/pdf/08eval.pdf)).|
| 23/09/2024 | **Efficient Algorithms for Modern CPUs**. (RV)<br><br>Memory Hierarchy: L1, L2, L3 Caches, RAM and latencies. Temporal and spatial localities. Hardware prefetching. Parallel computing. CPU parallelisms: Pipelining, superscalar processing, and SIMD. Pipeline hazards: structural, data, and control hazards. Branch prediction. Examples.  <br><br>*References*: Sections 3.1, 3.2, 3.3, 3.4, and 3.6 in "CPU Microarchitecture: Performance Analysis and Tuning on Modern CPUs", Denis Bakhvalov, 2024 ([link](https://github.com/dendibakh/perf-book/releases/download/Q2.2024/Performance.Analysis.and.Tuning.on.Modern.CPUs.Q2.2024.pdf)) and/or Sections 3.1, 3.2, 9.1, 9.2, 9.3, 9.6, 10.1, and 10.6 in *Algorithms for Modern Hardware*, Sergey Slotin ([link](https://en.algorithmica.org/hpc/)).|
| 25/09/2024 | **Properties of Natural Language and Text Processing**. (FMN)<br><br>Important properties of Natural Language: Vocabulary, Syntax, Semantic, Sources of Ambiguity, Dinamicity. Natural Language Understanding. AI-completeness. Relations with other data types: tabular data, graphs, image, videos. How do they link together in a modern Web search engine? Concept of Processing Pipeline. Text Processing (in Python): 1) Downloading text from the Web, 2) Extracting text from Web content, 3) NLTK: tokenization, sentence splitting, stemming, lemmatization, stopword removal. Jupyter Notebook #1: Text Processing.<br><br>*References*: Chapters 1 and 3 in *Natural Language Processing with Python* ([link](https://www.nltk.org/book/)).|
| 30/09/2024 | **Text Processing and Vector Space Model**. (FMN)<br><br>Important operations on text collections: stemming, lemmatization, stopword removal. Representations of text: Bag of word (pros and cons), Word N-grams (pros and cons), Character N-grams (pros and cons). Examples in Python. Why do we need a document representation: Vector Space Model. Binary one-hot encoding. Boolean Retrieval (AND, OR). Pros and Cons of Boolean Retrieval. <br><br>*References*: Chapter 1 in *Introduction to Information Retrieval*, Christopher D. Manning, Prabhakar Raghavan and Hinrich Schütze, Cambridge University Press. 2008 ([link](https://nlp.stanford.edu/IR-book/pdf/01bool.pdf)).<br><br>*Notes*: No recording is available for this lessons. Apologies for that.|
| 02/10/2024 | **Scoring, Term Weighting, and the Vector Space Model**. (FMN)<br><br>Limits of Boolean Retrieval. How can we extend it? Ranked retrieval and its evolution. Term-Document Binary Matrix. Jaccard. Pros and Cons of Jaccard. Frequency of terms and how it links to relevance. Term Frequency. Term-Document Count Matrix. Document Frequency. Difference between Document Frequency and Collection Frequency. Rareness of a term and how it links to relevance. Inverse Document Frequency. TF-IDF. How can we build a final Term-Document TF-IDF matrix. Examples.<br><br>*References*: Sections from 6.2 to 6.4.3 in *Introduction to Information Retrieval*, Christopher D. Manning, Prabhakar Raghavan, and Hinrich Schütze, Cambridge University Press. 2008 ([link](https://nlp.stanford.edu/IR-book/pdf/06vect.pdf)).|
| 07/10/2024 | **N-dimensional Vectors and Cosine Similarity, BM25**. (FMN)<br><br>Documents and Queries an N-dimensional vectors. How can we answer a query in the N-dimensional representation? Distance and Similarity: L2, pros and cons. Angle between vectors, dot product, cosine similarity. Examples. BM25: history, intuitions, formula, term frequency smoothing. Best practices on hyper-parameter and their tuning.<br><br>*References*: 1) Sections from 6.2 to 6.4.3 in *Introduction to Information Retrieval*, Christopher D. Manning, Prabhakar Raghavan, and Hinrich Schütze, Cambridge University Press. 2008 ([link](https://nlp.stanford.edu/IR-book/pdf/06vect.pdf)). 2) Stephen Robertson and Hugo Zaragoza. 2009. The Probabilistic Relevance Framework: BM25 and Beyond. Found. Trends Inf. Retr. 3, 4 (April 2009), 333–389. ([DOI](https://www.staff.city.ac.uk/~sbrp622/papers/foundations_bm25_review.pdf)).|
| 09/10/2024 | **Inverted Indexes. TAAT and DAAT**. (RV)<br><br>Inverted indexes for boolean and ranked retrieval. Term-at-a-time (TAAT) and Document-at-a-time (DAAT). NextGEQ operation with binary search and skip pointers. Faster AND query with nextGEQ. Positional Indexes for Phrase queries.<br><br>*Reference*: Sections 1 and 2.2 in *Efficient Query Processing for Scalable Web Search*, Nicola Tonellotto, Craig Macdonald, and Iadh Ounis, Now Foundations and Trends, 2018. ([link](https://arpi.unipi.it/retrieve/e0d6c931-3b36-fcf8-e053-d805fe0aa794/main-nowplain.pdf)) |
| 14/10/2024 | **Inverted Index and Query Processing in Python**. (RV)<br><br>In this lecture, we implemented a simple inverted index in Python. The index is built on a portion of the C4 Dataset and supports AND and OR queries implemented with both Term-at-a-time (TAAT) and Document-at-a-time (DAAT) strategies. We experimented with the skipping strategy to speed up AND query with the nextGEQ operation. |
| 16/10/2024 | **Query Processing**. (RV)<br><br>Top-k retrieval. Simple strategy: Exhaustive OR and Min-Heap. WAND and MaxScore. Intuition of blocking: Block Max-WAND and Block MaxScore.<br><br>*Reference*: Section 3 in *Efficient Query Processing for Scalable Web Search*, Nicola Tonellotto, Craig Macdonald, and Iadh Ounis, Now Foundations and Trends, 2018. ([link](https://arpi.unipi.it/retrieve/e0d6c931-3b36-fcf8-e053-d805fe0aa794/main-nowplain.pdf)) |
| 21/10/2024 | **Data Compression: Integer Encoders**. (RV)<br><br>Sharding in modern search engines. Data compression and time-space trade-offs. Integer encoders and binary representation. Unique decodability and prefix-free codes. Unary code, Elias' gamma and delta codes, and variable-byte.<br><br>*Reference*: Sections 1 and 2 (skip the codes we didn't discuss) in *Techniques for Inverted Index Compression*, Giulio Ermanno Pibiri and Rossano Venturini, ACM Computing Surveys (CSUR), 2021. ([link](https://pages.di.unipi.it/rossano/assets/pdf/papers/CSUR21.pdf)) |
| 23/10/2024 | **Data Compression: List Encoders**. (RV)<br><br>Encoding entire lists vs single integers. Combinatorial lower bound. Simple9 and Simple16. Patched Frame of Reference (PFor). Binary Interpolative Coding. Rank/Select queries on a binary vector. Elias-Fano representation and Partitioned Elias-Fano. <br><br>*Reference*: Section 3 (skip the codes we didn't discuss) in *Techniques for Inverted Index Compression*, Giulio Ermanno Pibiri and Rossano Venturini, ACM Computing Surveys (CSUR), 2021. ([link](https://pages.di.unipi.it/rossano/assets/pdf/papers/CSUR21.pdf)) |
| 28/10/2024 | **Midterm**. |
| 30/10/2024 | **Learning to Rank I**. (FMN)<br><br>A generalized framework for ranking. How can machine learning help in the ranking? A gentle yet short introduction to machine learning. Terminology alignment. A general machine learning framework. How can we map learning a ranking function in a general machine learning framework. Pointwise/Pairwise/Listwise approaches for Learning to Rank.<br><br>*Reference*: Section 2 in *Efficient and Effective Tree-based and Neural Learning to Rank*, Sebastian Bruch, Claudio Lucchese, and Franco Maria Nardini. Foundations and Trends® in Information Retrieval. 2023. ([link](https://arxiv.org/pdf/2305.08680)) |
| 06/11/2024 | **Learning to Rank II**. (FMN)<br><br>A learning to rank pipeline. How can we learn a classifier to predict the relevance of a query-document pair for ad-hoc search? Learning to rank approaches: a more precise formulation. Extending BM25 to BM25F. Pros and cons. How can we cast optimizing BM25F to a learning-to-rank problem? Pros and Cons. A learning to rank formulation of BM25F parameter tuning. Grid search vs. Gradient descent.<br><br>*Reference*: Section 2 in *Efficient and Effective Tree-based and Neural Learning to Rank*, Sebastian Bruch, Claudio Lucchese, and Franco Maria Nardini. Foundations and Trends® in Information Retrieval. 2023. ([link](https://arxiv.org/pdf/2305.08680)), and *The Probabilistic Relevance Framework: BM25 and Beyond*, Stephen Robertson, Hugo Zaragoza. Foundations and Trends® in Information Retrieval. 2009. ([link](https://www.staff.city.ac.uk/~sbrp622/papers/foundations_bm25_review.pdf))|
| 11/11/2024 | **Learning to Rank III**. (FMN)<br><br>Problems with learning the ranking. Gradient Boosted Regression Tree. What is a regression tree? How to fit a regression tree? How can we adapt fitting a regression tree for ranking documents? An example. What does it mean to optimize using the gradient in pointwise learning-to-rank methods?<br><br>*Reference*: 1) Section 2 in *Efficient and Effective Tree-based and Neural Learning to Rank*, Sebastian Bruch, Claudio Lucchese, and Franco Maria Nardini. Foundations and Trends® in Information Retrieval. 2023. ([link](https://arxiv.org/pdf/2305.08680)), and *Greedy function approximation: a gradient boosting machine*,  J. H. Friedman, Annals of Statistics, 1189-1232, 2001. ([link](https://jerryfriedman.su.domains/ftp/trebst.pdf))|
| 14/11/2024 | **Efficient Training of Ensembles of Decision Trees**. (RV)<br><br>Gradient Boosting Machine (GBM): overview, details, and example. Evaluating a Decision Tree. XGBoost and LightGBM: overview. Exact Greedy Algorithm for Split Finding. Histogram-based Split Finding. Number of Bins vs Training Time. Gradient-based One-side Sampling (GOSS). Exclusive Feature Bundling (EFB).<br><br>*References*: *XGBoost: A Scalable Tree Boosting System*, Tianqi Chen, Carlos Guestrin, KDD, 2016 ([link](https://arxiv.org/abs/1603.02754)), *LightGBM: A Highly Efficient Gradient Boosting Decision Tree*, Guolin Ke, Qi Meng, Thomas Finley, Taifeng Wang, Wei Chen, Weidong Ma, Qiwei Ye, Tie-Yan Liu, NIPS, 2017 ([link](https://proceedings.neurips.cc/paper/6907-lightgbm-a-highly-efficient-gradient-boosting-decision-tree.pdf)), and *An Experimental Evaluation of Large Scale GBDT Systems*, Fangcheng Fu, Jiawei Jiang, Yingxia Shao, Bin Cui, pVLDB, 2019. ([link](https://arxiv.org/abs/1907.01882)).|
| 18/11/2024 | **Efficient Inference of Ensembles of Decision Trees**. (RV)<br><br>How to efficiently traverse a forest of decision trees? Pros and Cons of three solutions: Struct+, If-then-else, and VPred. Two main ingredients of QuickScorer: 1) Alternative traversal of a single tree, and 2) Process the whole forest at once. Use of false nodes’ masks and interleaved tree traversals. Few experimental results.<br><br>*Reference*: *Fast Ranking with Additive Ensembles of Oblivious and Non-Oblivious Regression Trees*, Domenico Dato, Claudio Lucchese, Franco Maria Nardini, and Salvatore Orlando, Raffaele Perego, Nicola Tonellotto, Rossano Venturini, ACM Transactions on Information Systems (TOIS), 2016 ([link](https://pages.di.unipi.it/rossano/assets/pdf/papers/TOIS16.pdf)).|
| 20/11/2024 | **Language Models I**. (FMN)<br><br>What is a Language model: from the general formulation to specific statistical instances: unigram, bigram. Neural networks. How can we learn language models? Task, loss, training instances. Word2Vec. SkipGram and CBoW. The concept of embedding as a byproduct of the learning process. Pros and Cons of Word2Vec. Out-of-vocabulary problem and how to overcome it. FastText, Doc2Vec. Properties of the embedding space. Retrieval over learned representations as finding k-nearest neighbors (kNN) in the learned space. Exact vs. approximate kNN retrieval.<br><br>*References*: *Efficient Estimation of Word Representations in Vector Space*, Tomas Mikolov, Kai Chen, Greg Corrado, Jeffrey Dean, ICLR, 2013 ([link](https://arxiv.org/pdf/1301.3781)), and *Distributed Representations of Sentences and Documents*, Quoc V. Le, Tomas Mikolov, ICML, 2014 ([link](https://arxiv.org/abs/1405.4053)).|
| 25/11/2024 | **Efficient  Approximate k-Nearest neighbors retrieval I**. (RV)<br><br>Similarity Search. k-Nearest Neighbour Search. The 1D and 2D cases. The Curse of Dimensionality. Approximate k-NN Retrieval: Tree-based solutions, clustering-based solutions, hashing-based solutions, and proximity graphs. In Vitro Simulation of HNSW. NSW: Navigable Small World. NSW: Greedy Search. HNSW: Introduce a Hierarchy. Pugh's skip lists for 1D. Graph-based approaches: Open Problems.<br><br>*Reference*: *Efficient and robust approximate nearest neighbor search using Hierarchical Navigable Small World graphs*, Y. Malkov, D. Yashunin, IEEE Transactions on Pattern Analysis and Machine Intelligence, 2016 ([link](https://arxiv.org/abs/1603.09320)).|
| 27/11/2024 | **Efficient  Approximate k-Nearest neighbors retrieval II**. (RV)<br><br>Lossy Compression. Product Quantization: main intuition, encoding, distance computation, and experimental results. Neural Information Retrieval. Approximated kNN on sparse vectors. Seismic: concentration of importance, pruning, blocking, summaries, and experimental results.<br><br>*References*: *Product quantization for nearest neighbor search*, Hervé Jégou, Matthijs Douze, Cordelia Schmid, IEEE Transactions on Pattern Analysis and Machine Intelligence, 2011 ([link](https://inria.hal.science/inria-00514462v2/document)) and *Efficient Inverted Indexes for Approximate Retrieval over Learned Sparse Representations*, Sebastian Bruch, Franco Maria Nardini, Cosimo Rulli, Rossano Venturini, SIGIR, 2024 ([link](https://arxiv.org/abs/2404.18812)).|
| 02/12/2024 | **Language Models II**. (FMN)<br><br>Bidirectional Encoder Representations from Transformers (BERT). Attention and Transformer layer as building blocks of BERT. Network internals: tasks, special tokens, input embeddings, self-supervised training. The importance of BERT for finetuning specific down-stream tasks. Neural approaches in IR: interaction-based methods vs. representation-based methods. Pros and Cons. An example of interaction-based method: MonoBERT as a pointwise/pairwise fine-tuning of BERT for ranking queries and passages. Representation-based methods: dense (single-vector and multi-vector) learned representations vs. sparse learned representations. What does it mean to learn a dense representation: training pairs/triples, positive and negative examples. The importance of negative sampling. Static vs. Dynamic sampling. Two learned dense representation techniques: ANCE and ColBERT. How do they work?<br><br>*References*: Section 7 in *Efficient and Effective Tree-based and Neural Learning to Rank*, Sebastian Bruch, Claudio Lucchese, and Franco Maria Nardini. Foundations and Trends® in Information Retrieval. 2023. ([link](https://arxiv.org/pdf/2305.08680)) and specific papers reported in the slide deck of the lesson. |
| 04/12/2024 | **Project Discussion & Guest Speaker**. (FMN, RV)<br><be> Finalized assignments for projects (Part 2, final exam). Guest Speaker: Roberto Esposito (Weaviate).|
