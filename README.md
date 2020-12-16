# Deep learning based language identification in code mixed social media corpora
## Objective
Word level language identification in indian social media from facebook, twitter, whatsapp that exhibit code-mixing in english-hindi, english-telugu and english-hindi-telugu. The performance of deep learning on this task is compared to feature-based learning ie.,recursive neural networks techniques Bi-LSTM is contrasted to CRF classifier.
## Corpus Collection
Code mixed dataset for language identification is taken from 12th international conference on nlp ICON-2015. Data is collected from leading social-media websites like facebook, whatsapp, twitter. The dataset is comprised of facebook posts and comments, tweets and whatsapp chat conversations.

Out of total data 30% data is kept for testing and remaining data is used for training the
model.
## Models used
CRF model is implemented using sklearn-crfsuite on our data set. 
Data is retrieved as messages containing details of word, label and postag. CRF model is built using sklearn-crfsuite and default algorithm L-bfgs is used. Flat classification report from metrics is used to provide precision and F1-score for all labels
respectively.

Bi-lstm is implemented using Tensorflow and Keras. The proposed model for deep learning was trained using word embeddings. 
Data is retrieved as messages containing details of word, label and postag. Padding is necessary as model cannot take messages with different lengths.
## Conclusion
CRF classifier outperform LSTM only on English- Hindi dataset. The results show the deep learners outscoring the CRF, with the bidirectional LSTM demonstrating the best language identification performance. Deep learning-based approach to the task of language identification is achieved at a reasonable accuracy levels compared to a supervised approach such as CRF.
