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
  - The project is based on a scientific paper from over 10 selected papers.
  - The project can be completed by a team of up to 2 people.
  - The project will be presented using approximately 10 slides during the oral exam.
  - Students can approach the project at different levels of depth:
    - **Basic Level**: Read and understand the techniques presented in the article.
    - **Intermediate Level**: Conduct experiments to verify the assumptions, main properties,  or conclusions.
    - **Advanced Level**: Replicate the results from the article.
    - **Expert Level**: Re-implement the proposed solution, up to improving it by introducing alternative strategies.

#### Midterm Exams 

| Date | Time | Room |
| :------------- | --------: | :--------- |
| 28/10/2024 | 11:00 -- 13:00 | Room C |
| 11/12/2024 | 11:00 -- 13:00 | Room C |

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
| 09/10/2024 | **Inverted Index and Query Processing in Python. (RV)<br><br>In this lecture, we implemented a simple inverted index in Python. The index is built on a portion of the C4 Dataset and supports AND and OR queries implemented with both Term-at-a-time (TAAT) and Document-at-a-time (DAAT) strategies. We experimented with the skipping strategy to speed up AND query with the nextGEQ operation. |

