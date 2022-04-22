# SG-APP: Mobile health for POC testing with multiplexed immunoassay

This software project is/will be composed of the following 3 stages (S):

1. Machine learning and system design for standard mLFA read-outs
2. Features extraction and classification with ML based on SERS-based mLFA reporters
3. Machine learning model for testing strategy based on mLFA supplemented by SERS-based mLFA and disease surveillance

<img src="https://github.com/hcng10/SG-APP/blob/main/sgapp_dstn.png" width="800">

### S1: Machine learning and system design for standard mLFA read-outs
The assays are recognized with object detection techniques based on the dataset collected online and in-lab. For instance, 
- Histogram of oriented gradients (HOG) will be used to define features and an ML algorithm, such as support vector machine (SVM) will subsequently be trained and used to identify the assays. 
- Once the assay is recognized, the test lines will be interpreted using a convolutional neural network (CNN). The dataset will be split into training, validation, and test sets to determine the model parameters with the highest accuracy.

The ML classifier will be integreated within an Phone and Andriod APP, or on a Cloud-based software system with web and database services. Software and toolkits such as  Django, PostgreSQ, Flutter and Tensorflow Lite will be used.

### S2: Features extraction and classification with ML based on SERS-based mLFA reporters
DNN architecture such as an autoencoder and 3D-CNN will be used to classify the hyperspectral signals received from the low-cost reader for SERS-based mLFA. The corresponding accuracy will be evaluated with biofluid samples.

The ML model can significantly reduce the user expertise and domain knowledge in SERS for POC diagnostics, particularly in low-resource settings.

### S3: Machine learning model for testing strategy based on mLFA supplemented by SERS-based mLFA and disease surveillance
Smartphone APP and software systems will rely on robust models to inform testing strategy (choice of standard or SERS-based mLFA) and provide monitoring of the infectious disease. There will be three steps to deduce the final models: 

- SIR model is first studied to understand how infectious disease, such as COVID-19 is spread in a community.
- Gaussian process will then be studied and applied to the recorded data where each data dimension is considered to be a multi-variant Gaussian. The final classification takes the form of class probabilities which are useful to guide the testing strategy.
- A deep learning approach, such as recurrent neural network (RNN) architecture, will finally be investigated as it can capture the temporal occurrence of events.

## Project organization

    .
    ├── ml                    # Machine learning related files
    ├── app                   # Flutter code for APP (to be added)
    ├── services              # Cloud services (to be added)
