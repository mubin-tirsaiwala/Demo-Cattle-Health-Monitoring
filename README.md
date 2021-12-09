# Cattle Health Monitoring and Activity Classification
This repo is only for demonstrating this project. Development codes are kept confidential.

### Project Description :
---
Statlogic has earlier built a collar device for cattle which logs sensor data continuously. Utilising this data, we built models to identify the stance of the animal and its current activity. Apart from this, we also utilize microphone data to classify between the type of fodder the cattle is feeding on so that the nutritional intake can be monitored. Bundling all of this, we analyse if the animal is under any kind of stress since the first sign of illness is loss of appetite and fluctuations in daily activities.  

Models are trained using [Edge Impulse Studio](https://www.edgeimpulse.com/) which makes it easier to train and deploy models on edge, by utilizing harware accelerators and optimizing the models for lowest latency.  

Currently, the collars are deployed at multiple private farms and users are highly benefiting from this.

### Results :
---
All the models work continuously and keep logging the daily data along with the predictions.  
* Activity model can classify between 3 classes i.e. None, Feeding or Ruminating with 96% accuracy.
* Stance model can identify if the animal is standing or resting with 99% accuracy.
* Feed model can correctly classify between 3 type of fodder i.e. Concentrate, Green or dry with 97% accuracy. This model only runs when the activity model predicts that the animal is feeding.

### Demonstration of PowerBI Dashboard :
---
This dashboard continuously gets data from the source where the data from sensors are logged in real time. User can see the real time statistics of the animal for the past 24 hours.  

