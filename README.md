# Machine Predict Lithologies Using Wireline logs
## 1.1 What is machine learning?
Machine Learning (ML) is the method of applying programmatic and statistical computer technology to analyse large datasets, and as a result, uncover new understandings. It is a focussed sub-section of Artificial Intelligence (AI), where a more extensive set of predictive modelling tools enable a computer program to learn by generalising from examples. For more information read https://www.golder.com/insights/machine-learning-and-the-growing-use-cases-for-geoscience-practices/.

## 1.2 Problem Statement:
Identifying subsurface lithologies or rock types is essential for all geoscientists in order to explore our subsurface resources, particularly in the oil and gas industry. Lithology refers to the type of rock that forms the subsurface, and it is classified into, for instance, sandstone, claystone, marl, limestone, and dolomite. Several subsurface data can be used to identify lithologies, such as wireline logs petrophysical data. However, it is often a tedious, repetitive and time-consuming task. This project will predict lithology from petrophysical logs using machine learning techniques (classification) and add to the solution of these problems since these logs are direct proxies of lithology.

## 1.3 What are the classification in machine learning?
The Classification algorithm is a Supervised Learning technique that is used to identify the category of new observations on the basis of training data. In Classification, a program learns from the given dataset or observations and then classifies new observation into a number of classes or groups. In machine learning, classification refers to a predictive modeling problem where a class label is predicted for a given example of input data.

## 1.4 Wireline Logs Datasets
The data consist of 118 wells dataset spans through the South and North Viking graben and penetrates a highly variable geology from the Permian evaporites in the south the the deeply buried Brent delta facies in the North. An investigation of the provided training data clearly shows that the lithologic record offshore Norway is dominated by shales and shaly sediments. This is followed by sandstones, limestones, marls and the tufts.

The provided dataset contains well logs, interpreted lithofacies and lithostratigraphy for 90+ released wells from offshore Norway. The well logs include the well name (WELL), the measured depth, x,y,z location for the wireline measurement as well as the well logs CALI, RDEP, RHOB, DHRO, SGR,  GR, RMED, RMIC, NPHI, PEF, RSHA, DTC, SP, BS, ROP, DTS, DCAL, MUDWEIGHT. An explanation of the abbreviations is shown in the figure below.

The las files of the petrophysical logs dataset can be found [here](https://zenodo.org/record/4351156#.YXhFTBrMJPb).

## Results

### Well-1
![Well number 1](https://i.imgur.com/XSdNzX3.png)

### Well-2

![Well_number_2](https://i.imgur.com/YOrMKvo.png)

### Well-3

![Well_number_3](https://i.imgur.com/6gUOQew.png)

## Conclusions

Considering this work, the key messages and conclusion of this work could be summarised as follows:
    
1. The project results show that the XGboost and Catboost classifiers recorded higher accuracy on the training and validation datasets.

2. The XGboost was recorded 93.2% on the training dataset and 77.6% on the validation dataset, while the Catboost was recorded 85.6% on the training dataset and 76.7% on the validation data. 

3. We have created the Ridge Classifier model to impute the missing values of the categorical columns. Moreover, we have applied the k-Fold grid and random search to explore the dataset besides exploring the hyperparameters of the decision tree and random forest models.

4. The subsurface prediction of lithology in geoscience engineering deals with sparse petrophysical datasets with tens of features. One approach for feature selection is using entirely data-driven techniques such as selecting the whole data after imputing the missing values. The other approach is to use the data with actual values without filling the missing values. We found here that the Gamma-ray (GR), neutron density () and well location (X_log, Y_log) features carry essential geological information and could be used as an alternative representation of lithology when predicting the lithology from petrophysical wireline logs, especially for the oil and gas industry, for example.

5. The machine learning-based model could provide a very efficient and fast proxy for complex and slow complete physical-based lithology prediction, which in application like optimisation, could be very helpful. However, two areas need further attention:
    
    5.1. When going from a more simplified model to a more complex model, accuracy will be increased. However, the research in ML application must have analysis about the trade-off between speed and accuracy.
    
    5.2. In the ML model developed in this work, it was assumed that the training dataset here is “petrophysical wireline logs” that was fed to the ML to make a prediction about the subsurface lithologies. In fact, that training dataset is the ‘basin-wide sample’ while we are considering making a prediction about the lithology. Here, the challenging statistical question comes that how much training dataset is representative of the subsurface lithology of the dataset?

6. In the framework of decision analysis, in this study, the value of machine learning in a particular predicting subsurface lithologies was analysed. This analysis will be helpful for the companies to predict the lithologies based on their wireline logs data.

## Future Work

• This intensive geological dataset can be used to explore more classic machine learning models with better hyperparameters tuning.

• Apply deep learning methodology to predict the lithology using the same dataset.

• Utilise the free google cloud GPU to model the data using artificial neural networks such as CNN using PyTorch library.

## References

• Machine Predicted Lithology competition  by Force and Xeek 2020 Machine learning .  https://xeek.ai/challenges/force-well-logs/overview
• (Bormann P., et al. 2020). 2020 FORCE Machine Learning Contest. https://github.com/bolgebrygg/Force-2020-Machine-Learning-competition.
• FORCE 2020 Well well log and lithofacies dataset for machine learning competition https://zenodo.org/record/4351156#.YXmi1Z7MJPb.


Acknowledgements 
=================
The work contained in this repositories contains work conducted during a PhD study undertaken as part of the Natural Environment Research Council (NERC) Centre for Doctoral Training (CDT) in Oil & Gas funded 50% through its National Productivity Investment Fund grant number NE/R01051X/1 and 50% by the University of Aberdeen through its PhD Scholarship Scheme. The support of both organisations is gratefully acknowledged. The work is reliant on Open-Source Python Libraries, particularly numpy, matplotlib, Scikit-learn, XGBoost and pandas and contributors to these are thanked, along with Jovian and GitHub for open access hosting of the Python scripts for the study.

![University of Aberdeen](https://pbs.twimg.com/profile_images/1572172791801061377/UPSWmPyN_400x400.jpg)

![NERC-CDT](https://nerc-cdt-oil-and-gas.ac.uk/wp-content/uploads/news/2015-news-NERC-funding.jpg)

![NERC](https://auracdt.hull.ac.uk/wp-content/uploads/2019/11/UKRI_NER_Council-Logo_Horiz-RGB.png)

![CDT](https://i.imgur.com/QDOhcN3.png)

