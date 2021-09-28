# Face-Mask-Detector
Soft Computing Assignment

# 1.1 Introduction
In the 20th century, COVID-19 has now become a huge concern as it has affected the world badly. Studies have proved that wearing a face mask is one of the precautions to reduce the risk of viral transmission. Various measures are conducted to fight against COVID-19, and one of them is to raise the awareness of the importance of masks and encourage mask wearing in public places. Many public places as well as public service providers require customers to use the service and place only if they wear mask correctly. However, it is not possible to manually track the customer from time to time, whether they are wearing mask and wearing mask correctly or not. That is why this technology holds the key here to fight COVID-19. Many face mask detection models have been deployed using several algorithms and techniques. The proposed approach in this paper is using Caffe Model, MobileNetV2 and self-defined fully connected layers to train and test on images and video stream of people’s faces with mask, without mask or incorrectly worn mask. 

# 1.2	Objectives
The main objective of this Face Mask Detection Model Project is to provide some effective technology for preventing the spread of COVID-19 virus. The proposed model are solving a Multiclass Classification Problems where the labels are either (“Mask”, “No Mask” or “Incorrectly Mask”). Primary objectives behind the development of this model are to identify whether the mask are applied or not applied and to identify whether the mask are applied correctly or incorrectly.


# 1.3	Data Source
## 1.3.1	Correctly Masked Face Dataset (CMFD) 
Consists of high-quality images of datasets of human faces wearing the mask correctly. This is the dataset for Mask labels.
> For the CMFD datasets, the credit goes to the author of the Github link below:
https://github.com/cabani/MaskedFace-Net 
## 1.3.2	Incorrectly Masked Face Dataset (IMFD)
Consists of high-quality images of datasets of human faces wearing the mask incorrectly. This is the dataset for No Mask labels
> For the IMFD datasets, the credit goes to the author of the Github link below:
https://github.com/cabani/MaskedFace-Net  
## 1.3.3	FFHQ Dataset
A high-quality dataset of human faces, originally created as a benchmark for Generative Adversarial Networks (GAN). This is the dataset for Incorrectly Mask labels
> For the above dataset, the credit goes to the respective authors from the Github link below: https://github.com/NVlabs/ffhq-dataset 

# 1.4 Code Reference:
- https://github.com/pydeveloperashish/Mask-Detection-and-Recognition-using-Deep-Learning-Keras
- https://www.pyimagesearch.com/2020/05/04/covid-19-face-mask-detector-with-opencv-keras-tensorflow-and-deep-learning/

# 1.5 Project Details
Transfer learning is used in training the face mask model. We are utilizing the MobileNetV2 to train the mask classifier. This system or model consists of a Face Detector (Caffe Model) and Mask Detector using transfer learning with MobileNetV2 as base model. In the MobileNetV2 model, we construct the head of the model that will be placed on top of the base model. Training and evaluation are done using clasification metrics.

## Results
![image](https://user-images.githubusercontent.com/63900253/135062573-f815408e-0517-4665-8799-ec477d9b8323.png)


## Sample Input and Output
![2in1_2](https://user-images.githubusercontent.com/63900253/135061251-81c69349-cfb7-4749-b83a-be5573c5cb92.PNG)
![2in1_4](https://user-images.githubusercontent.com/63900253/135061337-92b98834-db27-449d-9621-1b645fe1b03e.PNG)
![2in1_3](https://user-images.githubusercontent.com/63900253/135061351-d5a42ac6-5942-49de-91a4-bc89946302bb.PNG)

# 2.0	Strengths and Limitations
After looking at the sample inputs and outputs given by the model. The following summarize the strengths and the limitations faced in the development of the project:
| Strengths      | Limitations |
| ----------- | ----------- |
| Performance are good in terms of number of faces detected and correctly classified. Accuracy of the model achieve a good result of 98% on testing.      | If the color of the mask varies, the model might not be able to classify whether the person is wearing a mask or not, or correctly or incorrectly wearing a mask.       |
| The model is able to identify faces that are clear enough and classify them accordingly with high-confidence.    | Missed out some faces that maybe not clear or in incorrect position or in a crowd.        |
| Support real time video stream by using imutils and OpenCV libraries.| |

# 3.0 Conclusion
Future research and works can be done to understand more about the model and other facial detection model like Haar Cascade, MTCNN and etc. In addition, it is worth a try to deploy several models using different network other than CNN, we can make more comparisons on the results between various Face Mask Detection Model and make use of the knowledge gained in near future.  

