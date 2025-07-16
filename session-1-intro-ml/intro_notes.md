Machine Learning is training software (called a model) to make predictions/ generate  content from data
Traditional approach vs ML approach: generally traditional approach is much more difficult and ML is easier because its training a second brain to do the hard stuff for you.
4 Types of ML Systems: Supervised learning, unsupervised learning, reinforcement learning, and generative AI
Supervised learning: sees data w correct answers and then makes predictions by figruing out the connects between the elements in the data. Kinda like a student studying for exams
Regression Models and Classification = supervised learning. Regression Models predict numeric values (future house prices, future ride times, amount of rain). Classification models have binary clasification (yes/no) and multiclass classification (a,b,c, or d)
Unsupervised learning: predictions through data that doesn't have correct answers, comes up with its own rules. Technique called clustering (finding data points and coming up with clusters w natural demarcations). 
Reinforcement learning: models predict by getting rewards/ penalties based on actions performed. Train robots on tasks w this.
Generative AI: models that create content from user input: unique images, music, jokes, summarize articles. Gen AI can take different types of inputs to generate different types of outputs. Some examples are Text-Text, Text-Image, Text-Code, Text-Speech
Gen AI imitate oters by observing repeated behaviors in different categories. 

Supervised ML
5 concepts: Data, Model, Training, Evaluation, Inference
Data = words, numbers in tables or pixels and waveforms. Dataset = cats, housing prices, weather info etc. Label = what all the features are measuring. Measure = what data you feed in to the ML model and its category. An ideal dataset has a large size and a lot of diversity to prevent the model from having biases. Evaluate a ML model by comparing its predictions to the actual values

Linear Regression: stat technique to find relationships between variable (feature and label for ML)
ML model takes the dataset, plots it , and finds a best fit line to go through the curve. In the training of the set, the model calculates the weight and bias that produce the best model. The general formula is y' = b + w1x1. b is bias and w1x1 is the feature. for each additional feature you add a wx expression to the formula. x is the feature and w is the weight of the feature. b and w and caluculated from the training of the model.

Loss: how wrong a model's predictions are. Lines indicate the distance of the actual value to the model line, focused on distance. L2 loss is calculatedc by taking the actual value - the predicted value and then squaring that. 4 types of loss: L1 (actual val - predicted val) Mean absolute error (1/n * sum actual val - predicted val), L2 loss (sum of actual val - predicted, squared), and mean squared error (1/n sum actual - predicted squared). 
MSE vs MAE: which to use? MSE will bring the model closer to the outliers and MAE won't.

Gradient Descent: model starts and 0 0 for bias and wieght and then gradually adjusts itself by determing what direction the curve needs to move in to be more accurate. Then after the loss is reduced, it repeats these steps until it acieves a model with the lowest loss
Loss Curves show when the model converges and after how many iterations it does this. Loss functions for linear model -> convex surface. Models never find the exact minimum for each weight/bias but they get close

Hyperparameters: 3 parameters, learning rate, batch size and epochs. Learning rate = a number you set that changes how quickly model converges. Too low = longer time for model to converge. Too high = model never converges but bounces around the minimum. The ideal Learning rate depends on each problem

Batch Size: number of examples a model uses before updating weight and bias. Stochastic gradient descent and mini8-batch stochastic gradient descent = common techniques to get the right gradient on avg
SGD: a single example per iteration but more likely to have loss curve oscillate at parts (noisy graph)
mini-batch SGD: compromise between full-batch and SGD. For N data points, batch size > 1 but les than N. The # of examples is random. small batch sizes = similar to sgd and larger batch size = full batch gradient descent.
Epoch: model has processed every example in the training set once. Ex: 1000 examples and a mini-batch of 100 ex - > 10 iterations = 1 epoch. typically needs many epochs for training. # of epochs is a hyperparameter you can experiment w to figure out how many it takes to converge. more = better but more time to train.
