# Health_Care_App

# Background
Machine learning is one of the most common forms of artificial intelligence in healthcare. It is a
broad technique at the core of many approaches to AI and healthcare technology and there are many versions of it.

Using artificial intelligence in healthcare, the most widespread utilization of traditional machine
learning is precision medicine. Being able to predict what treatment procedures are likely to be
successful
with patients based on their make-up and the treatment framework is a huge leap forward for many
healthcare organizations. The majority of AI in healthcare that uses machine learning and precision
medicine applications require data for training, for which the end result is known. This is known as
supervised learning.

Artificial intelligence in healthcare that uses deep learning is also used for speech recognition in
theform of natural language processing (NLP). Features in deep learning models typically have little
meaning to human observers and therefore the model's results may be challenging to delineate without
proper interpretation.

## Objectives
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
 
  <img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/BT_3.jpg" alt="Mountains" style="width:100%"/>
  
</p>

<h4> Covid Model Performance </h4>
<img height="300" src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/Covid.jpg" style="width:100%"> 
<hr>

<h4> Vaccine Conversation Trends </h4>
<img height="300" src="https://github.com/rashidesai24/Analyzing-Twitter-Trends-On-COVID-19-Vaccinations/blob/main/Images/Topic%20Trends.png" style="width:100%"> 
<hr>

<h4> Application With Flask  </h4>
<p float="left" > 
  <img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/app1.jpg" alt="Preprocessing" height="350"width="500"  />
  <img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/app3.jpg" alt="Augmented Images" height="350" width="500" />
  
  <br><img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/App2.jpg" alt="Augmented Images" height="350" style="width:80%" />
  <p> &nbsp Result</p>
  <p float="left" >
  <img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/OIP.jpg" alt="Augmented Images" height="350" width="250" />
  <img src="https://github.com/deepakcr7ms7/Health_Care_App/blob/master/images/BT4.jpg" alt="Augmented Images" height="350" width="750" />
</p>
</p>

## Model Accuracy

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
