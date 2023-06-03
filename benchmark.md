# NLP-benchamark-and-literature

# 1.Deep learning based text classification: A comprehensive review
## 1. Text classification <br>
      can be manual annotation or automatic labeling
      For the automatic labeling, the approaches can be grouped into two categories: 
      1) Rule-based methods: Rule-based methods classify text into different categories using a set of pre-defined rules, and require a deep domain knowledge.  
      2)Machine learning (data-driven) based methods:machine learning based approaches learn to classify text based on observations of data.
        For machine learning,follow the two-step procedure. 
        1st, some hand-crafted features are extracted from the documents (or any other textual unit). e.g. BOW
        2nd, those features are fed to a classifier to make a prediction. e.g. SVM, HMM, gradient boosting trees, RF
        Drawback:  
        1) the hand-crafted features requires tedious feature engineering and analysis to obtain good performance. 
        2).the dependence on domain knowledge makes the method difficult to generalize to new tasks. 
        3) cannot take full advantage of large amounts of training data because the features (or feature templates) are pre-defined.
      
## Models
   1. Word2Vec
   2. Elmo (3-layer LSTM)
   3. Transformer: GPT, BERT, GShard
   4. neuro-symbolic hybrid models

## TC tasks
   1. Sentiment Analysis.
   2. News Categorization. 
   3. Topic Analysis : identify the theme or topics of a text 
   4. Question Answering (QA) : two types of QA tasks: extractive and generative. Extractive QA is a TC task: Given a question and a set of candidate answers, a system classifies each candidate answer as correct or not. Generative QA is a text generation task since it requires generating answers on the fly. 
   5.Natural language inference (NLI): recognizing textual entailment (RTE), predicts whether the meaning of one text can be inferred from another. An NLI system needs to assign to a pair of text units a label such as entailment, contradiction, and neutral.
   
   
 
 ## TC models
 • Feed-forward networks view text as a bag of words 
 • RNN-based models view text as a sequence of words, and are intended to capture word dependencies and text structures 
 • CNN-based models are trained to recognize patterns in text, such as key phrases, for TC 
 • Capsule networks address the information loss problem suffered by the pooling operations of CNNs, andrecently have been applied to TC.
 • The attention mechanism is effective to identify correlated words in text, and has become a useful tool in developing DL models.
 • Memory-augmented networks combine neural networks with a form of external memory, which the models
can read from and write to (Section 2.6).
 • Graph neural networks are designed to capture internal graph structures of natural language, such as
syntactic and semantic parse trees (Section 2.7).
 • Siamese Neural Networks are designed for text matching, a special case of TC (Section 2.8) .
 • Hybrid models combine attention, RNNs, CNNs, etc. to capture local and global features of sentences and
documents (Section 2.9).
 • Transformers allow for much more parallelization than RNNs, making it possible to efficiently (pre-)train
very big language models using GPUs (Section 2.10).

Penn Treebank Dataset
