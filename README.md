# Distracted Driver Detection 🚗🪪
![image](https://user-images.githubusercontent.com/73777608/221331219-aa6a3502-0aa0-4494-929e-6f09b4f543ef.png)

This project works on developing a model that can detect whether a driver is distracted while driving, and what distraction they have. The dataset used ofr this project can be found here : https://www.kaggle.com/competitions/state-farm-distracted-driver-detection/data

## Modelling Experiments 🧪

We now have to decide which models we'll create and fine tune. Here is the list of all the experiments I'm going to run :  
- `model0` :- A simple Convolutional Neural Network with 3 conv and pooling layers stacked on each other
- `model1` :- A ResNet152V2 with custom input and output layers and a global average pooling layer.
- `model2` :- A MobileNetNetV2 with custom input and output layers and a global average pooling layer.
- `model3` :- A EfficientNetV2B3 with custom input and output layers and a global average pooling layer.

All these experiments will be saved and viewed on tensorboard later on. 

## Results and Conclusion

Here is what each class means :- 
- c0: safe driving
- c1: texting - right
- c2: talking on the phone - right
- c3: texting - left
- c4: talking on the phone - left
- c5: operating the radio
- c6: drinking
- c7: reaching behind
- c8: hair and makeup
- c9: talking to passenger

At the end of each experimet, lets see what accuracy they achieved 
- `model0` : 98%
- `model1` : 53%
- `model2` : 81%
- `model3` : 92%

Turns out the first model, just a simple CNN works the best with a high accuracy of 98%!
