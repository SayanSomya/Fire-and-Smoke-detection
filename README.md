# 🔥Fire-and-Smoke🌫️
<h3>Fire and Smoke Detection ⛑️ using AI and ML</h3>
This project aims to develop a model that can automatically detect fire and smoke in images and videos using artificial intelligence and machine learning techniques. The project is supervised by Assistant Professor <a href="https://www.iitg.ac.in/iitg_faculty_details?name=Manish-Bhatt&fac=T1kyemJyQ0pPN1I3blVENllFWjQ5dz09">Manish Bhatt</a> of IIT Guwahati.

<h4>Motivation</h4>
Fire and smoke are common hazards that can cause severe damage to life and property. Early detection of fire and smoke can help in preventing or mitigating the consequences of such disasters. However, traditional fire and smoke detection methods, such as sensors and alarms, may not be effective in some scenarios, such as outdoor environments, large areas, or complex scenes. Therefore, there is a need for a system that can use the power of computer vision and deep learning to analyze visual data and identify fire and smoke events in real time.

<h4>Objectives</h4>
The main objectives of this project are:
<ul>
<li>To collect and annotate a large-scale dataset of fire and smoke images and videos from various sources and scenarios.</li>
<li>To design and implement a deep neural network model that can accurately classify fire and smoke in random images and videos.</li>
<li>To evaluate the performance of the model on various metrics, such as Precision, Recall, Mean Average Precision, F1 score, Confidence etc. and curves formed using these parameters</li>
<li>To provide real-time fire and smoke detection from camera feeds or user uploads.</li>
</ul>

<h4>Methodology</h4>
The methodology of this project consists of the following steps:

<h6>1️⃣Data collection:</h6> We collected fire and smoke images and videos from IndianAI.gov and Roboflow public datasets.

<h6>2️⃣Data annotation:</h6> We manually labelled the collected data (fire, smoke and firefighters) using bounding boxes (for localization) with the help of tools such as Makesense.ai to facilitate the annotation process.

<h6>3️⃣Data preprocessing:</h6> We performed data augmentation techniques, such as cropping, resizing, flipping, rotating, etc., to increase the diversity and robustness of the data. We also normalized the data to have zero mean and unit variance.

<h6>4️⃣Model development:</h6> We designed and implemented a deep neural network model that can perform fire and smoke detection in images and videos. We used frameworks such as TensorFlow or PyTorch to build the model. We explored different architectures, such as convolutional neural networks (CNNs), recurrent neural networks (RNNs), or attention mechanisms, to achieve the best results.

<h6>5️⃣Model training:</h6> We trained the model on the preprocessed data using a suitable loss function, such as binary cross-entropy or mean squared error. We will use optimization algorithms, such as stochastic gradient descent (SGD) or Adam, to update the model parameters. We will also use regularization techniques, such as dropout or batch normalization, to prevent overfitting.

<h6>6️⃣Model evaluation:</h6> We evaluated the model's performance on a separate test set using various metrics, such as accuracy, precision, recall, F1-score, etc. We also compared the model with other various models to demonstrate its effectiveness.

<h4>Results</h4>
link of the videos 
<table>
  <thead>
    <td>
      YOLO v5
    </td>
    <td>
      YOLO v8
    </td>
  </thead>
  <tr>
    <td>
      <img src="">
    </td>
    <td>
      <img src="">
    </td>
  </tr>
</table>

<h4>Challenges</h4>

The initial challenge we encountered was selecting the most appropriate model for small base object detection models using around <500 images as a dataset, which we discovered to be YOLO as the best among the open source models.
<br>
Subsequently, we experienced many false detections and inaccurate results, which we attempted to minimize by creating more refined labels. After successfully training the model on Fire and Smoke we decided to add new labels such as Fire Alarm, Fire Exit, Fire Extinguishers, FireMen, etc. in the model, but the False detection of the video increased dramatically. 
<br>
We tried to train the model individually on these new labels and figured that the Fire Extinguisher dataset caused the problem until we removed it from the dataset.


<h4>References</h4>
The list of all the references used for this project is as follows:
<h6>For Raw images</h6>
<ul>
  <li>https://indiaai.gov.in/datasets</li>
   <li>https://universe.roboflow.com/data2/fire-smoke-detection-ua3dm</li>
</ul>
<h6>For Final Dataset</h6>
<ul>
  <li>
    https://drive.google.com/file/d/1hwAQrt2xWMPOOMpGlzmTrURxe2gwbs9c/view?usp=sharing
  </li>
</ul>
<h6>Google Collab</h6>
<ul>
  <li>https://colab.research.google.com/drive/1D1uFjpw30_WDdpEfAjQSMmGJG9i1NrJO?usp=sharing</li>
  <li>https://colab.research.google.com/drive/1vE8Q7X86zDfqxH06n0Nlg7uhrTI0Fusc?authuser=1#scrollTo=nbl9gNVukXMJ</li>
</ul>
<h6>MATLAB code</h6>
<ul>
  <li>https://docs.google.com/document/d/1fnWQKwwOqb8XOkdg5-w5d4uHXZQMF-pOFun8s1F3OPQ/edit</li>
</ul>

