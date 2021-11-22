# Brain Tumor Detection

In this project I used a dataset of brain MRI images. This dataset contained two classes, one class belongs to images which are healthy brains. The other class belongs to images of brains with tumor.  
![image](https://user-images.githubusercontent.com/67642255/142821150-b37ecd92-7524-4c3b-b5eb-34b352440971.png)
![image](https://user-images.githubusercontent.com/67642255/142821244-3ace089f-8d81-4216-be67-45d959c5aa0e.png)

I dowloaded the dataset from link bellow:  
adress: https://www.kaggle.com/navoneel/brain-mri-images-for-brain-tumor-detection  
The class of healthy brains contained 154 images.   
The class of images with tumor contained 155 images.  
![image](https://user-images.githubusercontent.com/67642255/142820589-4cd2b8f6-9284-40ba-95d5-46e3ba14b8b0.png)

I used a CNN neural network to make a binary classifier. 
At first, I trained the model for 10 epochs:
![image](https://user-images.githubusercontent.com/67642255/142822153-c94ce3df-7094-4d40-8b38-f391232e60a8.png)
  
and I fined tuned it for 30 more epochs.  
![image](https://user-images.githubusercontent.com/67642255/142822230-cfba7bff-9d0c-4e29-a7a8-10c5c0df5939.png)

I reached the value accuracy=0.92  

#Model with Augmented Images 

I augmented images by:
- rotating  
- width and height shifting
- horizontal fliping  
- shearing  
- zooming    
An example of this augmentation is placed bellow:   

![image](https://user-images.githubusercontent.com/67642255/142823136-1e05c013-7f42-4e24-a05e-b18f2b1e0948.png)
![image](https://user-images.githubusercontent.com/67642255/142823191-6aea2873-5106-4922-95ca-1d622a25ade3.png)    

![image](https://user-images.githubusercontent.com/67642255/142823235-ef9b0f49-c318-469a-a898-365e95757b26.png)
![image](https://user-images.githubusercontent.com/67642255/142823262-f5f5cf73-dba1-4263-bf16-933ecf37d130.png)   


Then I repeated the model training:    

![image](https://user-images.githubusercontent.com/67642255/142823541-1f9c6eb6-0b0c-4e8f-8884-e55f9807395a.png)    

# Use a Pretrained Architecture VGG16

I used a pretrained model, VGG16, I freezed it and then I added one dense layer and a sigmoid classifier layer. 
I trined it for 100 epochs.   

![image](https://user-images.githubusercontent.com/67642255/142824937-fee4065f-e2ee-48cd-9c79-4f22b56bab15.png)    

The best achieved accuracy for validation during training was 0.94







