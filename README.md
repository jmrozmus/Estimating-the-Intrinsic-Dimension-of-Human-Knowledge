# Estimating the Intrinsic Dimension of Human Knowledge

### Background and Motivation

The Dewey Decimal System, still used in most libraries, maps human knowledge into a single numerical dimension. But it is easy to find books on complex or interdisciplinary topics that could logically map to multiple distinct numbers on that single dimension. Ideally, human knowledge would be indexed with a finite set of numbers that would optimally locate each chunk of knowledge in proximity to related information. But what is the minimum size of that set of numbers? Using mathematical terminology, the answer to this question is called the intrinsic dimension of all human knowledge.

Modern large language models (LLM’s) use sets of thousands to tens of thousands of floating-point numbers to encode human knowledge in their scope of understanding. Data scientists call these “vector embeddings”. But when a human being is thinking, he or she is mapping thought into the three-dimensional space of the human brain. This strongly suggests that the intrinsic dimension of human knowledge is much lower than thousands. There would seem to be a lot of room for improvement in modern LLM’s!

I have pondered the intrinsic dimension of human knowledge for decades. Algorithms to measure intrinsic dimension of large sets of high-dimensional vectors have been available for quite a while. But high-dimensional vectors to represent a large sample of human knowledge have not – until now! The vector embeddings of LLM’s provide just that.

### Method and Results

Cohere published a dataset of 35 million+ vector embeddings of paragraphs in Wikipedia in 2022: https://huggingface.co/datasets/Cohere/wikipedia-22-12-en-embeddings?ref=cohere-ai.ghost.io. I downloaded this dataset. Then I used the scikit-dimension Python package from https://github.com/scikit-learn-contrib/scikit-dimension to measure the intrinsic dimension of this set of vectors by a method called correlation dimension (https://en.wikipedia.org/wiki/Correlation_dimension). I used several random samplings of 0.1% of the 35 million+ vectors and several ranges for the distances between vectors (a required input to the correlation dimension algorithm). The intrinsic dimension of the sample sets consistently measures to be 7.6 to 7.8. (See IntrinsicDimResults_20250610.txt) Therefore, **I propose that a good first estimate of the intrinsic dimension of all human knowledge is eight (8).**

### Implications

The implications of this discovery for AI efficiency and interpretability – and much more – are profound. Claude Sonnet 4 tells me: “The implications could reshape not just AI technology, but our understanding of cognition, learning, and knowledge representation across all domains.” (I used Claude Sonnet 4 as my assistant throughout this research in the past few weeks. You may see our rich throeretical and practical dialog at https://claude.ai/share/d9f163d7-381c-47e0-af15-de0e05292633. I also used Claude Sonnet 4 to speed my Python coding.)

### Acknowledgement

I offer my heartfelt thanks and compliments to the Anthropic team for the very impressive Claude Sonnet 4 and to Jonathan Bac et al for recognizing the value of exploring intrinsic dimension and making the scikit-dimension package to enable that exploration. 
