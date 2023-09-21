# EHR_2_vec
Experiences to develop EHR2vec : make a patient cohort pre selection based on clinical notes

---

The data on which we based our experiments comes from a healthcare database, and is therefore not shareable. 

Two methods can be tested and implemented for patient pre-selection: 

1. a document-oriented method: documents are translated into vector representation by 3 different models: 
- the classic TFIDF model, which the user can implement with the `tfidf_expe1.ipynb` and `tfidf_expe2.ipynb` notebooks
- the doc2vec model, for use with the `doc2vec_expe2.ipynb` and `doc2vec_expe2.ipynb` notebooks
- the docBERT model, for use with notebooks `docbert_expe1.ipynb` and `docbert_expe1.ipynb`

2. A query expansion method : 
- Firstly, by creating a list of synonyms using the CODER model via the notebook: `CODER_synonym.ipynb` and, for example, the query proposed in the `query_4types.txt` file.
- then by searching for documents containing these terms after creating the list of synonyms in the notebook `word_search_doc.ipynb`.


All codes are available after installation of `requirements.txt`

