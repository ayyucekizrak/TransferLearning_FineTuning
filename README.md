📌[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ayyucekizrak/Udemy_DerinOgrenmeyeGiris/blob/master/TransferOgrenme_FineTuning/Fine_Tune_TransferOgrenme.ipynb) **Google Colab Not Defteri**

📌[![Open In Jupyter](https://github.com/jupyter/notebook/blob/master/docs/resources/icon_32x32.svg)](https://nbviewer.jupyter.org/github/ayyucekizrak/Udemy_DerinOgrenmeyeGiris/blob/master/TransferOgrenme_FineTuning/Fine_Tune_TransferOgrenme.ipynb) **Jupyter Not Defteri** 
---
# What is Fine-Tuning and Transfer Learning? 👽

---
For a moment, let's take a small step back from the nitty-gritty details of EfficientNet.🕊Imagine that a bird could pass on to you what it has learned. Or what you have learned you could pass to a fish-sounds crazy, right? 
Let's just say, I have learned since I was born and from my ancestors to recognize a glass. There are simple features (edge, corner, shape, material structure, etc.). Turns out, something happens when machines learn-they transfer what they know and learn to other machines, skipping  the full learning process. 

 
**Let us start with a computer vision problem, but I am talking about a method that can be applied to many types of data and problems. So there is a dataset inside the object you want to recognize, but the dataset is too big (this is awesome 😃), the model is also very successful (again, which is awesome 🤗), but it will take days and weeks to train that model for that dataset. It's trained here though!**  🧐
 

---
 
 ![](https://a4.pbase.com/o4/98/367898/1/59218520.tn_Braintransferwatercolor.jpg)
 
You've been solving a new problem by taking advantage of what an artificial learning model has learned before. You do this by transferring all or part of what the model has learned. I mean the weights. That's exactly why it's called **Transfer Learning**. Sometimes if you just make adjustments to learn the basic features for your model, this time it's called **Fine-Tuning**. Another version, for example, contains images of *dogs* of *Golden and Husky* genres and *human* images of *men and women*. Here you can do *Dog-Human* classification with the model, as well as *Female-Male* or *Golden-Husky* classification, which is called **Multi-Task Learning**.
 
![](https://github.com/ayyucekizrak/TransferLearning_FineTuning/blob/master/TL_FT.png)

---

🎯 **#1 Version:** Yalnızca bu parametreleri model için kullandığımızda test işlemini yaparak yeni bir sinir ağı tasarımı yapmayız. Tüm eğitilmiş modeli test için kullanabiliriz. Özellikle mobil ve gerçek zamanlı öğrenme gerektirmeyen uç noktada çalışacak sistemlerde bu yöntem uygulanmaktadır. Belli periyotlarla eğitim işlemi daha geniş verilerle tekrarlanıp sistem performansı artırılabilir.

When we use these parameters only for the model, we do not make a new neural network design by testing. We can use the entire trained model for testing. This method is used especially in mobile and real-time learning systems that do not require real-time learning. Periodic training can be repeated with larger data and system performance can be improved.


🎯 **#2 Version:**  Eğitilmiş modelin bir kısmını alıp devamında veri kümesinde bulunmayan kendi problemimize ait veriler için eğitiriz. Böyle yaptığımızda Paratmetre hesabı yani işlem yükünü azaltmış oluyoruz ve zamandan da kazanmış oluyoruz. Aynı zamanda kendi problemimiz için verilerimiz kısıtlı olsa dahi bu yöntemle büyük veri setlerinde öğrenilen temel öznitelikler açısından da daha yüksek bir başarıya ulaşılmış olur. Fakat bu yöntemi uygularkan de dikkat etmemiz gereken stratejiler var. 

We take a part of the trained model and then train it for the data of our own problem which is not in the data set. When we do this, we reduce the Parameter account, that is, the transaction load and we save time. At the same time, even if our data is limited for our own problem, this method achieves a higher achievement in terms of the basic features learned in large data sets. But there are strategies that we need to pay attention to when applying this method.

> * How similar or different the data we use to the data set of the pre-trained model

> * Size of the data we will use

With the following scheme, we can simply determine how we can make a choice.


![](https://github.com/ayyucekizrak/TransferLearning_FineTuning/blob/master/TL_FN2.png)


 🕵 So let's look at a simple example of how we can use a test process that we can run edge!

### 🔥For this purpose, ResNet50 was trained with deep neural networks for the IMAGENET dataset and weight parameters were recorded at the end of the training.

---
⚡️[On **Algorithmia** you can make your own model available to everyone as an API.
With the **ResNet** deep learning model trained on the **ImageNe**t dataset, you can try the image classification algorithm free of charge from the link below. Thanks to **Yavuz Kömeçoğlu** for this work.](https://algorithmia.com/algorithms/yavuzkomecoglu/ImageClassification)
![](https://github.com/ayyucekizrak/Udemy_DerinOgrenmeyeGiris/blob/master/TransferOgrenme_FineTuning/Algortihma.jpg)

---
 ✏️ **Use the links below for more resources:**

[Comparison of Activation Functions for Deep Neural Networks](https://towardsdatascience.com/comparison-of-activation-functions-for-deep-neural-networks-706ac4284c8a)

[Step-by-Step Use of Google Colab’s Free TPU](https://medium.com/deep-learning-turkiye/ad%C4%B1m-ad%C4%B1m-google-colab-%C3%BCcretsiz-tpu-kullan%C4%B1m%C4%B1-621dc6e5487dhttps://heartbeat.fritz.ai/step-by-step-use-of-google-colab-free-tpu-75f8629492b3)

---

 ### ⭐️[Transfer learning with TensorFlow Hub](https://www.tensorflow.org/tutorials/images/hub_with_keras)⭐️
 ### ⭐️ [Transfer learning from pre-trained models](https://towardsdatascience.com/transfer-learning-from-pre-trained-models-f2393f124751)⭐️
