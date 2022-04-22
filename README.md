# SG-APP: Mobile health for POC testing with multiplexed immunoassay

This software project is/will be composed of the following 3 stages(S):

1. Machine learning and system design for standard mLFA read-outs
2. Features extraction and classification with ML based on SERS-based mLFA reporters
3. Machine learning model for testing strategy based on mLFA supplemented by SERS-based mLFA and disease surveillance

## Machine learning and system design for standard mLFA read-outs
The assays are recognized with object detection techniques based on the dataset collected online and in-lab. For instance, Histogram of oriented gradients (HOG) will be used to define features and an ML algorithm, such as support vector machine (SVM) will subsequently be trained and used to identify the assays. Once the assay is recognized, the test lines will be interpreted using a convolutional neural network (CNN). The dataset will be split into training, validation, and test sets to determine the model parameters with the highest accuracy.

The ML classifier will be integreated within an Phone and Andriod APP, or on a Cloud-based software system with web and database services. Software and toolkits such as  Django, PostgreSQ, Flutter and Tensorflow Lite will be used.
