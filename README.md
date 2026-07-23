Skin Cancer Classification using Convolutional Neural Networks (CNN)

Project Overview
This project implements a Convolutional Neural Network (CNN) for automated skin lesion classification using the HAM10000 ("Human Against Machine with 10,000 Training Images") dataset. The model classifies dermoscopic images into seven different skin lesion categories, supporting computer-aided diagnosis in dermatology.
The project covers the complete deep learning workflow, including dataset acquisition, image preprocessing, exploratory data analysis, data augmentation, CNN model development, performance evaluation, and model persistence.

Objectives
Develop a CNN-based skin lesion classifier. 
Classify dermoscopic images into seven diagnostic categories. 
Apply image preprocessing and normalization. 
Improve model generalization using data augmentation. 
Evaluate classification performance with confusion matrix and classification report. 
Save the trained model for future inference. 

Dataset
Dataset: HAM10000 – Human Against Machine with 10,000 Training Images
The dataset contains dermoscopic images of skin lesions belonging to seven diagnostic classes:
Actinic Keratoses (akiec) 
Basal Cell Carcinoma (bcc) 
Benign Keratosis-like Lesions (bkl) 
Dermatofibroma (df) 
Melanoma (mel) 
Melanocytic Nevi (nv) 
Vascular Lesions (vasc) 
Dataset Source:
Kaggle: Skin Cancer MNIST: HAM10000 


Features
Automatic image loading 
Image preprocessing 
RGB image conversion 
Image resizing 
Label encoding 
Image normalization 
Data augmentation 
CNN-based image classification 
Batch normalization 
Dropout regularization 
Multi-class classification 
Accuracy visualization 
Confusion matrix 
Classification report 
Trained model saving 

Data Preprocessing
The preprocessing pipeline includes:
Reading metadata 
Loading dermoscopic images 
RGB color conversion 
Image resizing to 128 × 128 
Label encoding 
One-hot encoding 
Pixel normalization 
Train-test split 

Exploratory Data Analysis (EDA)
The project performs:
Class distribution visualization 
Lesion category frequency analysis 
This helps identify class imbalance within the dataset.

Data Augmentation
To improve model generalization, the following augmentation techniques are applied:
Random rotation 
Width shifting 
Height shifting 
Horizontal flipping 
Vertical flipping 
Random zoom 

Deep Learning Model
Convolutional Neural Network (CNN)
Architecture
The CNN consists of:
3 Convolutional Layers 
Batch Normalization 
Max Pooling Layers 
Dropout Layers 
Flatten Layer 
Fully Connected Dense Layer 
Softmax Output Layer 
Optimizer
Adam 
Learning Rate
0.0001 
Loss Function
Categorical Crossentropy 
Output Classes
7 Skin Lesion Categories 

Technologies Used
Python 
TensorFlow 
Keras 
OpenCV 
NumPy 
Pandas 
Matplotlib 
Seaborn 
Scikit-learn 
Kaggle API 
Google Colab 

Evaluation Metrics
The model is evaluated using:
Test Accuracy 
Training Accuracy 
Validation Accuracy 
Confusion Matrix 
Classification Report 
Precision 
Recall 
F1-Score 

Output
The project generates:
Trained CNN model 
Training history 
Accuracy curves 
Validation accuracy plots 
Confusion matrix 
Classification report 
Saved .h5 model file 

Installation
pip install tensorflow
pip install keras
pip install opencv-python
pip install pandas
pip install numpy
pip install matplotlib
pip install seaborn
pip install scikit-learn
pip install tqdm



Applications
This project can be applied to:
Medical image classification 
Skin cancer screening 
Clinical decision support 
Dermatology research 
AI-assisted healthcare 
Computer-aided diagnosis (CAD) 
Deep learning in medical imaging 

Future Improvements
Train for more epochs with early stopping and learning rate scheduling. 
Use transfer learning models such as ResNet50, EfficientNet, DenseNet, or MobileNetV2 for improved performance. 
Address class imbalance using class weighting or oversampling techniques. 
Integrate Grad-CAM or other explainable AI methods to visualize regions influencing predictions. 
Deploy the model as a web application using Streamlit or Flask for real-time skin lesion classification. 

Learning Outcomes
This project demonstrates practical knowledge of:
Deep Learning 
Convolutional Neural Networks (CNNs) 
Medical Image Analysis 
Computer Vision 
Image Classification 
Data Augmentation 
Multi-class Classification 
TensorFlow/Keras 
Model Evaluation 
AI in Healthcare
