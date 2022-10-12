Based on: https://github.com/enriqueav/lstm_lyrics

Word-level text generation via an RNN

A rough list of used libraries and versions can be found in the corresponding thesis.

train_basic.py is used to train the model. The data used for training, as well as the save locations for example sequences generated during training and the vocabulary created during training must be specified as the first, second and third paramater of the script respectively when executing. General training parameters can be altered using variables within the script. The model saves checkpoints during training when an epoch has achieved sufficient training success.

Training data can be obtained from the MailFilter repository

generate_basic.py can be used to load previously trained models and to generate new sequences of text. A number of parameters can be adjusted here.
-n specifies the location of the network to be loaded.
-v specifies the location of the vocabulary created during the models training.
-s specifies the input sequence used to generate the text.
-d specifies the temperature value used for sampling.
