# Whalehumpback_Siamese
Siamese CNN for Whalehumback identification  Kaggle (https://www.kaggle.com/c/humpback-whale-identification/leaderboard)

Dataset can be found here: https://www.kaggle.com/c/6818/download-all
Siamese neural networks were introduced in the early 1990s by Bromley and LeCun. 
A paper by Gregory Koch, Richard Zemel and Ruslan Salakhutdinov where Siamese CNN are used for One-Shot image Recognition can be found here: https://www.cs.cmu.edu/~rsalakhu/papers/oneshot1.pdf




This repository consists of 3 python files: 
  > Whale_Siamese_test.py
  > Whale_Siamese_train.py
  > siamese_utils.py

> Whale_Siamese_train.py trains A Siamese CNN for the train dataset of Whalehumpback Identification challenge. Fold 0 denotes train in the whole dataset while Folds 1-5 train the NN in the respective data of the train dataset used for cross-validation.
> Whale_Siamese_test.py evaluates the NN on the test dataset/ folds 1-5 of the train dataset. Its output is "prediction_fold[0-5].csv" which contains the predictions for the corresponding fold (test dataset corresponds to fold 0). The NN predicts the top 5 labels for each image evaluated.
> siamese_utils.py contains the parameters of the NN (layers, loss function, etc.)
