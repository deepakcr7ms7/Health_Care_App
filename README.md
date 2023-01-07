# Health_Care_App

## TABLE OF CONTENTS

* [Background](#background)
* [Objective](#objective)
* [Tools and Packages](#tools)
* [Data Visualization](#data-visualization)
* [Results](#results)
* [References](#references)
* [Challenges and Future Work](#challenges-and-futurework)

<hr>

## BACKGROUND 
Machine learning is a subset of artificial intelligence utilizing mathematical and statistical methods to identify patterns in data in an automated fashion [34]. Numerous aspects of clinical practice lend themselves to computational tools to assess disease pathology, identify anomalies, triage critical patients, and various other tasks, but the scope of this article is limited to supervised learning to constrain the discussion, develop concrete examples, and because it represents the majority of clinical machine learning research.

In the context of supervised machine learning, models are fit to data, thereby learning relationships between input features and output targets. Input data represent digital encodings of, for example, X-rays, lab tests, electrocardiograms, or various other clinical data streams. The output could be a diagnostic label, a region of interest, length of stay, etc. For pedagogical ease, throughout this article, the classification of lung nodules will be used as a reference example.

The inputs to this nodule classifier are computed tomography (CT) images, but other modalities could have been used (e.g., X-ray or ultrasound). Each input image is associated with a two-class binary label (i.e., 0 or 1, indicating the absence or presence of calcified nodules, respectively). There is nothing special about the binary label; in other clinical applications, the label could represent several discrete classes (e.g., different types of lung nodules or disease stages) or be a continuous output as in regression (e.g., length of hospital stay, lab tests with continuous ranges).

Once CT images and associated labels are sourced and validated, a trained model learns relations between the image features (e.g., edges, contours, etc.) and their binary class (i.e., a positive or negative finding). However, this trained model may have also learned idiosyncratic features specific to the provided image and label pairs, which are not generally true in other data from the same modality (in this case, CT images). This generalization brittleness occurs for many reasons, including equipment with different noise sources (across different manufacturers), out-of-calibration effects, selection bias, population differences, and many others. Building generalizable models is paramount to clinical research. After all, the radiologist who developed the training data/labels can go to another hospital and provide the same expertise. At the same time, a working model at one medical center can fail at another. Therefore, it becomes key to understand the issues that might arise during the model training, validation, and testing processes.

<hr>

## Objective
- To build disease classification models using Deep Neural networks and Random Forrest Classifier
- To preprocess images using CV2 and improve model performance
- To integrate trained models and create an app using flask



<hr> 

## TOOLS

<table style="width:100%">
  <tr>
    <th>Task</th>
    <th>Technique</th> 
    <th>Tools/Packages Used</th>
  </tr>
  
  <tr>
    <td>Data Pre-processing and EDA</td>
    <td>Image normaliaztion, Noise removal, Data Creation for Covid  </td> 
    <td>cv2, shutil, sklearn, pandas, numpy</td>
  </tr>
  
  <tr>
    <td>Model Developement </td>
    <td> feature_selection, model_selection, model construction, optimization, neural network tunning, performance evaluation </td> 
    <td> Tensorflow, xgboost, sklearn</td>
  </tr>
  
  
  <tr>
    <td>Data Visualization</td>
    <td>Multi-attribute plots, heatmaps, correlation plots</td> 
    <td>matplotlib, seaborn </td>
  </tr>
  <tr>
    <td>Environments & Platforms</td>
    <td>  </td> 
    <td>MS Excel, Jupyter Notebook, Tensorflow, Pycharm</td>
  </tr>
</table><br>

<hr>

## DATA-VISUALIZATION 

<h4> Brain Tumour </h4>
<p float="left" >
  <img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/BT_Preprocessing.jpg" alt="Preprocessing" height="250"width="500"  />
 
  <img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/BT_2.jpg" alt="Augmented Images" height="250" width="500" />
 
 
</p>
 <img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/BT_3.jpg" alt="Mountains" style="width:100%"/>
  

<h4> Covid Model Performance </h4>
<img height="300" src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/Covid.jpg" style="width:100%"> 
<hr>

<h4> Vaccine Conversation Trends </h4>
<img height="300" src="https://github.com/rashidesai24/Analyzing-Twitter-Trends-On-COVID-19-Vaccinations/blob/main/Images/Topic%20Trends.png" style="width:100%"> 

<hr>

##  Application with Flask
<p float="left" > 
  <img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/app1.jpg" alt="Preprocessing" height="350"width="500"  />
  <img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/app3.jpg" alt="Augmented Images" height="350" width="500" />
</p>  
  
  <br><img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/App2.jpg" alt="Augmented Images" height="350" style="width:80%" />
  
  <p> &nbsp Output </p>
  
  <p float="left" >
  <img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/OIP.jpg" alt="Augmented Images" height="300" width="250" />
  <img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/BT4.jpg" alt="Augmented Images" height="300" width="750" />
  </p>


<hr>

## RESULTS 

<table style="width:100%">
  <tr>
    <th>Disease</th>
    <th>Classifier Type</th>
    <th>Accuracy</th> 
  </tr>
  
  <tr>
    <td> Pneumonia </td>
    <td> CNN </td> 
    <td> 83.17% </td>
  </tr>
  <tr>
    <td> Heart Disease </td>
    <td> XGBoost </td> 
    <td> 86.96% </td>
  </tr>
<tr>
    <td> Diabetes </td>
    <td> Random Forest </td> 
    <td> 89.8% </td>
  </tr>
<tr>
    <td> Alzheimer </td>
    <td> CNN </td> 
    <td> 83.54% </td>
  </tr>
 
<tr>
    <td> Breast Cancer</td>
    <td> Random Forest </td> 
    <td> 91.81% </td>
  </tr>
 
<tr>
    <td> Brain Tumor</td>
    <td> CNN, VGG16 </td> 
    <td> 96.5% </td>
  </tr>
 
<tr>
    <td> COVID-19 </td>
    <td> CNN </td> 
    <td> 93.5% </td>
  </tr>
 
</table>

## CONCLUSION 
Created seven disease classification models with TensorFlow, Random Forest and XGBoost to analyse patients’
medical records, achieving over 90% accuracy.Improved the accuracy of deep neural networks by 30% with image data augmentation and transfer learning

## REFERENCES 
<li> Disease Classification Using Machine
Learning Algorithms - A Comparative
Study S.Leoni Sharmila1,∗
, C.Dharuman2 and P.Venkatesan3 1,2 Department of Mathematics, SRM University,
Ramapuram Campus, Chennai - 600 089, India. </li>
<li> Development of machine learning model for diagnostic disease prediction based on laboratory tests
Dong Jin Park, Min Woo Park, Homin Lee, Young-Jin Kim, Yeongsic Kim & Young Hoon Park</li>
<li>Machine-Learning-Based Disease Diagnosis: A Comprehensive Review
Md Manjurul Ahsan,1, Shahana Akter Luna, and Zahed Siddique </li>
<li>A Review of Challenges and Opportunities in Machine Learning for Health
Marzyeh Ghassemi,, Tristan Naumann, Peter Schulam, Andrew L.
Beam , Irene Y. Chen, Rajesh Ranganath </li>
<hr>

## CHALLENGES-AND-FUTUREWORK 
<b> Challenges </b>: Identifying package for tweet scraping and recognizing limitations on extraction, large execution times and runtime errors due to memory limitation for parts of data modeling. Medical information is difficult to come by. As a result, if the databases were made public, researchers would have access to additional information.</li>
<h4> Future Work </h4>
<li> Explore new models to detect rare diseases </li>
<li> Number of active COVID cases, recoveries and deaths for the three months </li> 
<br><br>
