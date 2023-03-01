# Word Embedding Evalutor
Fork of [cz_corpus](https://github.com/Svobikl/cz_corpus) by Lukas Svoboda. Ported to Python3/Gensim 4.3.0 and adapted model loading for fasttext models - both binary and plain-text.

### Testing corpus with Python and Gensim

Prerequisites: 

- Python >2.7
- Gensim package for word2vec toolkit
- Numpy package

Clone repository and uncompress model: 

 - "git clone https://github.com/jirkoada/embedding_evaluator Evaluator"
 - Download model from following address: "https://github.com/Svobikl/cz_corpus/releases/tag/release1.0/vectors_cz_cbow_dim300uni400_w15n15_iter15.txt.tar.gz" and save it to
folder "models/no_phrase"
 - Alternatively you can download other models from "https://github.com/Svobikl/cz_corpus/releases/tag/release1.0" 
 - You can also download a pretrained fasstext model for Czech language from "https://fasttext.cc/docs/en/crawl-vectors.html"
 - "tar -zxvf Evaluator/models/no_phrase/vectors_cz_cbow_dim300uni400_w15n15_iter15.tar.gz"

Running evaluator:

 - "cd Evaluator"
 - "python Evaluator.py -m ./models/no_phrase/vectors_cz_cbow_dim300uni400_w15n15_iter15.txt"


Settings: 
- "-m" : model path specification
- "-t" : top n similar words,  default is 1.
- "-c" : corpus path specification, default is "./corpus/czech_emb_corpus.txt",
- or you can use "help" command and see all possible argument settings.


