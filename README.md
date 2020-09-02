# Machine Learning for Conditioning Monitoring
## Faulty Machine Prediction

### Table of Content
  1. Libraries
  2. Introduction
  3. Project Motivation
  4. Files
  5. Result
  6. Acknowledgment
  
### Libraries
Libraries needed to install so as to run the file are:
  1. `Anaconda`: It is a free and open-source distribution of the Python and R programming languages for scientific computing that aims to simplify package
  2. `Tensorflow`: TensorFlow is an open source library for numerical computation and large-scale machine learning.
  
### Introduction
ExampleCo, Inc is gathering several types of data for its fleet of very expensive machines. These very expensive machines have three operating modes: normal, faulty and failed. The machines run all the time, and usually they are in normal mode. However, in the event that the machine enters faulty mode, the company would like to be aware of this as soon as possible. This way they can take preventative action to avoid entering failed mode and hopefully save themselves lots of money.

They collect four kinds of timeseries data for each machine in their fleet of very expensive machines. When a machine is operating in normal mode the data behaves in a fairly predictable way, but with a moderate amount of noise. Before a machine fails it will ramp into faulty mode, during which the data appears visibly quite different. Finally, when a machine fails it enters a third, and distinctly different, failed mode where all signals are very close to 0.

You can download the data here: [exampleco_data](https://drive.google.com/drive/folders/1b12u6rzkG1AxB6wLGl7IBVoaoSoZLHNR)

The objectives:

  1. There are some clear outliers in the data due to communication errors from the sensor equipment. These bad measurements have no bearing on the problem you’re trying to solve, and a good place to start is to find a way to filter them out.
  2. Develop an approach to detect the beginning of the “faulty” period, ideally giving the ExampleCo engineers as much time as possible to shut down their machines before failure occurs (at which time all measurements drop close to 0). The best solutions are automated in the sense that they would generalize to similar but slightly different data; simpler methods are acceptable but are less likely to receive full credit.

### Project motivation
There is a great deal of literature on anomaly detection out in the world, from open-source packages like Twitter’s AnomalyDetection to Linkedin’s Luminol. I chose this project because I wanted to explore more about Anamoly Detection using Time Series data. It is a real-world scenario; making it a chance for an intensive experience with data processing.

### Files
  1. `Data_science_exercise.ipynb`: Jupyter Notebook with Visualizations and Code
  2. `exampleco_data`: Folder with data of 20 machines
  
### Result
Predicted Anamolies using Auto-Regressive model, OneSVM model and AutoEncoders.

### Acknowledgement
  * ExampleCo for providing the data
