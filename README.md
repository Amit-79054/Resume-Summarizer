# Resume-Summarizer

For the given problem statement I have used Named Entity Recognition(NER)  approach and trained my model against 200 resume which is in a pickle format.

Training a model -

I have used python’s spaCy module for training the NER model. I have used the Dropout technique to improve the learning results and it is set a dropout rate, a rate at which to randomly “drop” individual features and representations. This makes it harder for the model to memorize the training data. For example, a 0.25 dropout means that each feature or internal representation has a 1/4 likelihood of being dropped. I have trained my model for 10 epochs and keep the dropout rate as 0.2.

After training my model, I have loaded it to “nlp_model” then I have applied my trained model to the resume which is at the 0 indexes of my training data.

After that using Fitz I have applied my trained model to the resumes in PDF format and extracted the required data.
