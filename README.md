# Machine Learning to Predict Lithologies Using Wireline Logs
## 1.1 What is Machine Learning?
Machine Learning (ML) involves the application of programmatic and statistical computer technology to analyze large datasets, leading to new insights. It is a specialized subfield of Artificial Intelligence (AI) that uses a broader set of predictive modeling tools, enabling computer programs to learn by generalizing from examples. For more information, refer to this article: https://www.golder.com/insights/machine-learning-and-the-growing-use-cases-for-geoscience-practices/.

## 1.2 Problem Statement:
Identifying subsurface lithologies or rock types is crucial for geoscientists, especially in the oil and gas industry. Lithology refers to the types of rock forming the subsurface, including sandstone, claystone, marl, limestone, and dolomite. Various subsurface data, such as wireline logs petrophysical data, can be used to identify lithologies. However, this task is often tedious, repetitive, and time-consuming. This project aims to predict lithology from petrophysical logs using machine learning techniques (classification) to address these challenges, as these logs are direct proxies of lithology.

## 1.3 What is Classification in Machine Learning?
The classification algorithm is a supervised learning technique used to identify the category of new observations based on training data. In classification, a program learns from a given dataset or observations and then classifies new observations into several classes or groups. In machine learning, classification refers to a predictive modeling problem where a class label is predicted for a given example of input data.

## 1.4 Wireline Logs Datasets
The dataset consists of 118 wells spanning the South and North Viking graben, covering highly variable geology from Permian evaporites in the south to the deeply buried Brent delta facies in the north. An investigation of the training data shows that the lithologic record offshore Norway is dominated by shales and shaly sediments, followed by sandstones, limestones, marls, and tufts.

The provided dataset contains well logs, interpreted lithofacies, and lithostratigraphy for over 90 released wells from offshore Norway. The well logs include the well name (WELL), the measured depth, and the x, y, z location for the wireline measurement, along with well logs such as CALI, RDEP, RHOB, DHRO, SGR, GR, RMED, RMIC, NPHI, PEF, RSHA, DTC, SP, BS, ROP, DTS, DCAL, and MUDWEIGHT. An explanation of the abbreviations is shown in the figure below.

The LAS files of the petrophysical logs dataset can be found: [here](https://zenodo.org/record/4351156#.YXhFTBrMJPb).

Acknowledgements 
=================
The work presented in these repositories was conducted during a PhD study as part of the Natural Environment Research Council (NERC) Centre for Doctoral Training (CDT) in Oil & Gas. This study was funded 50% through the National Productivity Investment Fund grant number NE/R01051X/1 and 50% by the University of Aberdeen through its PhD Scholarship Scheme. The support from both organisations is gratefully acknowledged. This work relies heavily on Open-Source Python Libraries, specifically NumPy, Matplotlib, Scikit-learn, XGBoost, and Pandas. Appreciation is extended to the contributors of these libraries, as well as Jovian and GitHub, for providing open access hosting of the Python scripts used in this study.

![University of Aberdeen](https://i.imgur.com/PILyj4m.jpg)

![NERC-CDT](https://nerc-cdt-oil-and-gas.ac.uk/wp-content/uploads/news/2015-news-NERC-funding.jpg)

![NERC](https://auracdt.hull.ac.uk/wp-content/uploads/2019/11/UKRI_NER_Council-Logo_Horiz-RGB.png)

![CDT](https://i.imgur.com/QDOhcN3.png)

