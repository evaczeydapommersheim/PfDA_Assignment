# PfDA_Assignment - Project 1

***Author: Eva Czeyda-Pommersheim***

## **Introduction**

#### This project has been prepared for the 2022 Winter Semester Course of HDip in Computing in Data Analytics, Programming for Data Analysis module led by Dr. Brian McGinley at Atlantic Technological University. 

## **Assessment Task**:

- Choose a real-world phenomenon that can be measured and for which you could.
- Collect at least one-hundred data points across at least four different variables.
- Investigate the types of variables involved, their likely distributions, and their
relationships with each other.
- Synthesise/simulate a data set as closely matching their properties as possible.
- Detail your research and implement the simulation in a Jupyter notebook – the
data set itself can simply be displayed in an output cell within the notebook.

## **Environment - System Requirement**<p>
---
This project is presented in a Jupyter Notebook 
which is part of this repository.  

There are multiple solution for running the jupyter 
notebook.

*Option A - Installation of the necessary 
environment*<p>

In order to run and/or modify the notebook on a 
local machine, the latest version of Python is 
required.  
An easy way to obtained/install python may be 
achieved by downloading the Anaconda open source 
package.  
> **Anaconda** is a distribution of the Python and 
R programming languages for scientific computing, 
that aims to simplify package management and 
deployment.  
The distribution includes data-science packages 
suitable for Windows, Linux, and macOS.  
It’s also is free to install and offers free 
community support.  

Following the installation of Python the Jupyter 
Notebook may be downloaded to the local machine 
from this repository.  
> **Step 1**<p>
Open your preferred command line on your local 
machine (CMDer for Windows and other built-in 
terminals for Linux and Mac OS)<p>
> **Step 2**<p>
>Navigate to the folder where the jupyter notebook 
was downloaded as 
Normal_Distribution_Project_Winter 2022-23.ipynb<p>
> **Step 3** <p>
> Type command jupyter notebook and press enter 
which should open a new screen with the jupyter 
notebook content.<p>

*Option B - Viewing the notebook in the cloud*

> **nbviewer** is a web application that lets a URL 
to be entered of a Jupyter Notebook file, it 
renders that notebook as a static HTML web page, 
and gives you stable link to that page which then 
can be shared with others. <p> nbviewer is an open 
source project under the larger Project Jupyter 
initiative along with other projects like Jupyter 
Notebook, JupyterLab, and JupyterHub.<p> Here is 
the static link to my Jupyter Notebook:<p> https://nbviewer.org/github/evaczeydapommersheim/PfDA_Assignment/blob/main/PfDA_Assignment.ipynb<p>

> **Binder** is a service provided by the Binder 
Project, which is a member of the Project Jupyter 
open source ecosystem. It allows sharing a public 
Github Repository jupyter notebook file in a static 
manner. The code can be run, but no changes will be 
posted to the file. No collaboration is possible 
with this viewing option.<p>

## **Chosen phenomenon for assessment**:

After researching possible options for this assignment, I decided to explore an area that is related to my current job in the medical device industry. The dataset of my choice can be found in ![Kaggle](https://www.kaggle.com/code/mennatallahnasr/stroke/data). <p> 

<img src="https://media.istockphoto.com/id/1168179082/photo/man-with-brain-stroke-symptoms.jpg?s=612x612&w=0&k=20&c=eYZ9ayO0rR0Su3vN3EU48CxOOnwxUXDgXhpAYb2s7L4=" width="300">

It is called the Stroke Prediction Dataset and has the following attribute information:<p>
1) id: unique identifier
2) gender: "Male", "Female" or "Other"
3) age: age of the patient
4) hypertension: 0 if the patient doesn't have hypertension, 1 if the patient has hypertension
5) heart_disease: 0 if the patient doesn't have any heart diseases, 1 if the patient has a heart disease
6) ever_married: "No" or "Yes"
7) work_type: "children", "Govt_jov", "Never_worked", "Private" or "Self-employed"
8) Residence_type: "Rural" or "Urban"
9) avg_glucose_level: average glucose level in blood
10) bmi: body mass index
11) smoking_status: "formerly smoked", "never smoked", "smokes" or "Unknown" (Unknown meaning that the information was not available for the particular patient)
12) stroke: 1 if the patient had a stroke or 0 if not

About the data:<p>
_According to the World Health Organization (WHO) stroke is the 2nd leading cause of death globally, responsible for approximately 11% of total deaths._<p>
_This dataset is used to predict whether a patient is likely to get stroke based on the input parameters like gender, age, various diseases, and smoking status. Each row in the data provides relavant information about the patient._<p>

## **Table of Content**:

> Libraries<p>
> 1. The Dataset
>> 1.1 Importing dataset<p>
>> 1.2 Exploring the data<p>
>> 1.3 Visualizing data<p>

> 2. Preprocessing<p>
>> 2.1 Encoding categorical features into numeric arrays<p>
>>> 2.1.1 OneHotEncoder()<p>
>>2.2 Normalization of continuous variables
> 3. Balancing<p>
> 4. Modelling<p>
>> 4.1 Fitting and Predicting with alternative methods<p>
> 5. Scoring<p>
> Conclusion

## **References**:

- https://www.anaconda.com/products/distribution 
Accessed  on 16 Nov 2022

- https://en.wikipedia.org/wiki/Markdown Accessed 
on 15 Nov 2022
- https://www.freecodecamp.org/news/
how-to-write-a-good-readme-file/ Accessed on 15 
Nov 2022
- https://www.dataschool.io/
cloud-services-for-jupyter-notebook/ Accessed on 
17 Nov 2022
- https://the-turing-way.netlify.app/communication/binder/zero-to-binder.html Accessed on 27 Nov 2022
- https://scikit-learn.org/stable/modules/preprocessing.html#preprocessing-categorical-features Accessed on 26 Nov 2022
- https://towardsdatascience.com/top-3-python-packages-to-generate-synthetic-data-33a351a5de0c Accessed on 06 Nov 2022
- https://www.youtube.com/watch?v=r-uOLxNrNk8 Accessed on 27 Nov 2022
- https://towardsdatascience.com/synthetic-dataset-generation-for-ml-using-scikit-learn-and-more-beab8cacc8f8 Accessed on 28 Nov 2022

- https://www.simplilearn.com/regression-vs-classification-in-machine-learning-article Accessed on 28 Nov 2022
- https://www.kaggle.com/code/madhurpant/stroke-advanced-eda-with-prediction#7.-Data-Preprocessing Accessed on 01 Nov 2022
- https://www.kaggle.com/code/mennatallahnasr/stroke#split-the-data-:
- https://www.kaggle.com/code/muqarrishzaib/stroke-risk-predictive-analysis Accessed on 21 Nov 2022
- https://towardsai.net/p/data-science/how-when-and-why-should-you-normalize-standardize-rescale-your-data-3f083def38ff Accessed on 25 Nov 2022
- https://www.kdnuggets.com/2017/06/7-techniques-handle-imbalanced-data.html Accessed on 03 Dec 2022
- https://towardsdatascience.com/5-techniques-to-work-with-imbalanced-data-in-machine-learning-80836d45d30c Accessed on 03 Dec 2022
- https://imbalanced-learn.org/stable/references/generated/imblearn.over_sampling.SMOTE.html Accessed on 03 Dec 2022
- https://www.youtube.com/watch?v=gJo0uNL-5Qw Accessed on 03 Dec 2022

## **License**<p>
*This Notebook was released under GNU General Public License v3.0 license*.
