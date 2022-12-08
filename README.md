### Breast_Cancer_statistical_analysis


## Final project for UTSA Data Visualization Boot Camp

**Identify the problem:**

Breast cancer is the most common malignancy among women, accounting for nearly 1 in 3 cancers diagnosed among women in the United States, and it is the second leading cause of cancer death among women. Breast Cancer occurs because of abnormal growth of cells in the breast tissue, commonly referred to as a Tumor. A tumor does not mean cancer - tumors can be benign (not cancerous), pre-malignant (pre-cancerous), or malignant (cancerous). Tests such as MRI, mammogram, ultrasound, and biopsy are commonly used to diagnose breast cancer performed.
1.1 Expected outcome
Given breast cancer results from breast fine needle aspiration (FNA) test (is a quick and simple procedure to perform, which removes some fluid or cells from a breast lesion or cyst (a lump, sore or swelling) with a fine needle similar to a blood sample needle). Since this build a model that can classify a breast cancer tumor using two training classification:

•	1= Malignant 
•	0= Benign 

**1.2 Objective**
Since the labels in the data are discrete, the predication falls into two categories, (i.e. Malignant or benign). In machine learning this is a classification problem.
Thus, the goal is to classify whether the breast cancer is benign or malignant and predict the recurrence and non-recurrence of malignant cases after a certain period. To achieve this we have used machine learning classification methods to fit a function that can predict the discrete class of new input.
1.3 Identify data sources
•	The first two columns in the dataset store the unique ID numbers of the samples and the corresponding diagnosis (M=malignant, B=benign), respectively.
•	The columns 3-32 contain 30 real-value features that have been computed from digitized images of the cell nuclei, which can be used to build a model to predict whether a tumor is benign or malignant.


**Getting Started**

Load Dataset:

First, we download and load the .CSV file using Pandas.read_csv function.

**Inspecting the data**

**The first step is to visually inspect the new data set. There are multiple ways to achieve this:**

The easiest being to request the first few records using the DataFrame data.head()* method. By default, “df.head()” returns the first 5 rows from the DataFrame object df (excluding the header row).

**Data Analysis**

Now that we have a good intuitive sense of the data, Next step involves taking a closer look at attributes and data values. In this section, We are getting familiar with the data, which will provide useful knowledge for data pre-processing.

Data Exploration an important step which takes place after engineering features and acquiring data. This is an important step data scientists to be able to understand the nature of the data. 
The results of data exploration are used to understanf the structure of the data, the distribution and presence normal versus extreme values and identify interrelationships within the data set.

From the the visualizations, we can see that radius_mean, perimeter_mean, area_mean, concavity_mean and concave_points_mean are useful in predicting cancer type due to the distinct grouping between malignant and benign cancer types in these features. We can also see that area_worst and perimeter_worst are also quite useful.


Check encoding confirm the coversion of diagnosis categorical data into numeric, where:

•	Malignant = 1
•	Benign = 0 

**Observation**

357 observations indicating the absence of cancer cells and 212 show absence of cancerous cells

**Data Visualizations**

One of the main goals of visualizing the data here is to observe which features are most helpful in predicting malignant or benign cancer. The other is to see general trends that might help with selection of a model and other parameters.

Tableau Link : https://public.tableau.com/app/profile/loraine.gomez/viz/BreastCancerAnalysis_16704027941520/BOXA



**Machine Learning**

Introduction:

We used the clean dataset and checked the headings, dropped Unnamed = 0 column
Assessing Model Accuracy: Split data into training and test sets
The simplest method to evaluate the performance of a machine learning algorithm is to use different training and testing datasets. Here our group will:


•	Split the available data into a training set and a testing set. (70% training, 30% test)
•	Train the algorithm
•	make predictions 
•	use confusion matrix
•	evaluate the predictions against the expected results.

**Building Models**


Logistic Regression:

Decision Tree:

Random Forest Classifiers(3 models):




Data Source : (https://archivebeta.ics.uci.edu/dataset/17/breast+cancer+wisconsin+diagnostic)



























