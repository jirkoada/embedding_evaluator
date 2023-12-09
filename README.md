# Word Embedding Evaluator
Fork of [cz_corpus](https://github.com/Svobikl/cz_corpus) by Lukas Svoboda. Ported to Python3/Gensim 4.3.0, adapted model loading for fasttext models - both binary and plain-text, as well as compressed models.

### Testing corpus with Python and Gensim

Prerequisites: 

- Python >= 3.10
- Gensim package for word2vec toolkit
- Numpy package
- [compress-fasttext](https://github.com/avidale/compress-fasttext) (optional)

Clone the repository and obtain models: 

 - "git clone https://github.com/jirkoada/embedding_evaluator Evaluator"
 - You can download a pre-trained fasstext model for the Czech language from "https://fasttext.cc/docs/en/crawl-vectors.html"
 - Visit the original [repo](https://github.com/Svobikl/cz_corpus) to explore models released alongside it

Running the evaluator:

 - "cd Evaluator"
 - "python Evaluator.py -m /path/to/model/model_name.bin"


Settings: 
- "-m" : model path specification
- "-t" : top n similar words, default is 1.
- "-c" : corpus path specification, default is "./corpus/diacritics/czech_emb_corpus.txt",
- "--compressed": Indicate the evaluated model was compressed with [compress-fasttext](https://github.com/avidale/compress-fasttext)
- or you can use "help" command and see all possible argument settings.


