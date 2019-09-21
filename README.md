# Training-Neural-Network-with-imbalanced-class-data

As deep learning is taking its place in almost all sectors to solve various domain related problems,In this repo health diagnosis with pneumonia detection using chest X-ray is addressed with deep learning. When dealing such dataset, the data is not equally avalilable for both the normal and pneumonia affected X-rays. In the real world scenario, the data for normal X-rays are more compared to X-rays with pneumonia affected X-rays. So, while training a neural network with such an imbalanced dataset, the model tends to be biased towards the class with more data. To tackle such problems, class weights are added to the model to make model less biased and improve the classification rate.   

**Steps**
	Obtain the dataset	(https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)
	Adapt transfer learning with inceptionV3 to extract features from the X-ray images (https://medium.com/@sh.tsang/review-inception-v3-1st-runner-up-image-classification-in-ilsvrc-2015-17915421f77c)
	Train a dense network on top of inceptionV3 using our class labels by adding class weights.
	
**Findings and Results**

**Without Class Weights:** 

Validation Accuracy: 93%
Testing Accuracy: 64%

![image](https://user-images.githubusercontent.com/44360746/65369451-7b5a8d00-dc7f-11e9-9cdd-7595baeed72a.png)


**With Class Weights:**

Validaion Accuracy: 94%
Testing Accuracy: 80%



**Conclusion**

Adding class weights to the model improves the model performance to some extent. 
	
