# Machine-Learning---PyTorch
Work for DSA8021 Module at QUB

## Use

The code imports all issues for HADOOP and puts each issue as an observation in a pandas DataFrame. 

For each issue the description, issue type, priority, resolution, status, summary, components and parent fields are retained. All other information is dropped as it was found to be of negilgable benefit to classificaiton of issues. 

A numerical label is assigned to each issue depending on its issue type, this will be the label used for training neural network and evaluation preformance of network. 

Glove embedding are used for sentiment analysis of the description and summary fields. All other fields are changed to one hot encoding type. 

Each group is balanced using random sampling and data is split into train, validation and test sets (60:20:20 ratio). 

A neural network is then trained on the training data using the PyTorch package.

The optimum network was found to be able to classify the issues with 70% accuracy.
