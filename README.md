# DL4SN-Detect-Soprano
MSc CE Deep Learning Networks Repository


https://studio.edgeimpulse.com/studio/203785

## Introduction

My project’s idea was to understand how auto ID on Echo Meter Touch 2 Pro works and if I am able to train a model to identify only one of 18 UK species. As an ecologist, I undertake bat surveys from May to September following Bat Conservation Trust’s Guidelines. I use Echo Meter Touch 2 Pro for IOS which is a dongle that attaches to iPhone or iPad and an app starts to display a spectrogram of the surrounding noise. 
Nocturnal bats employ echolocation, emitting high-frequency calls to navigate and visualize their environment. These ultrasonic calls, akin to sonar, are captured by ecologists to study bat behavior, revealing details about their surroundings in real time. This mechanism, functioning as an acoustic imaging system, aids in tasks such as locating food, maneuvering obstacles, and surviving perilous environments. Identifying bat species acoustically involves recognizing call patterns from sonograms, a process demanding substantial training and time. 

<img width="151" alt="image" src="https://github.com/Rita888/DL4SN-Detect-Soprano/assets/93122551/487a5a95-1be7-486b-bae1-3df82ef7fae9">



## Research Question

Is it possible to train a model to detect one bat species using Edge Impulse and Nano BLE? 

## Application Overview
Convolutional Neural Network
Passive acoustic sensing has recently emerged as a valuable method for monitoring and assessing the impact of human activities on wildlife and biodiversity. In particular, it has proven to be quite effective in quantifying the echolocation calls of bats. In a study conducted by Mac Aodha et al. in 2018, they introduced an open-source pipeline based on Convolutional Neural Networks (CNNs) to identify various types of bat calls, including those during the search phase, ultrasonic calls, and full spectrum calls.
To train their deep learning algorithms, the researchers collected ultrasonic audio data along road transects in Bulgaria and Romania as part of the iBats program. The CNN-based detector they designed was put to the test against different commercial systems and algorithms, using datasets recorded in various countries with different types of sensors.
The results of these tests demonstrated that the CNN-based detector outperforms commercial systems, particularly when it comes to accurately identifying search-phase bat calls, as evidenced by its higher recall and precision rates.

As I am working with audio files, I am aiming to use Mel-frequency cepstral coefficients (MFCCs), spectrograms and classifier. Different features within Edge Impulse were available and I would like to try different representations to identify which works best for the data.

## Data
Data used in this study were the bat calls that were recorded during the bat survey. These were auto classified by using ML embedded within Wildlife Acoustics Products such as Echo 
Meter Touch. 

<img width="208" alt="image" src="https://github.com/Rita888/DL4SN-Detect-Soprano/assets/93122551/f3e0cdaa-5610-4867-a3b2-3192bba83cfa">


## Model
The Impulse design allowed Spectrogram to be trained as a processing block and then classifier to analyse the spectrograms. 
<img width="306" alt="image" src="https://github.com/Rita888/DL4SN-Detect-Soprano/assets/93122551/9f6ae873-ba91-4469-b1ab-0a54477abbd3">
<img width="300" alt="image" src="https://github.com/Rita888/DL4SN-Detect-Soprano/assets/93122551/aa1603ec-7816-4f84-9734-41354f70fb10">

## Experiments
[
](https://drive.google.com/drive/folders/14VS9gDBJejs9kDNSuPBaC1lrOkg_sRhg?usp=share_link)

## Results and Observations
<img width="143" alt="image" src="https://github.com/Rita888/DL4SN-Detect-Soprano/assets/93122551/27f55eb1-f925-416f-998e-055a110bf27b">

## Bibliography
Mac Aodha, O., Gibb, R., Barlow, K.E., Browning, E., Firman, M., Freeman, R., Harder, B., Kinsey, L., Mead, G.R., Newson, S.E. and Pandourski, I., 2018. Bat detective—Deep learning tools for bat acoustic signal detection. PLoS computational biology, 14(3), p.e1005995.
Mac Aodha, O., Martinez Balvanera, S., Damstra, E., Cooke, M., Eichinski, P., Browning, E., Barataud, M., Boughey, K., Coles, R., Giacomini, G. and Mac Swiney G, M.C., 2022. Towards a General Approach for Bat Echolocation Detection and Classification. bioRxiv, pp.2022-12.


----

## Declaration of Authorship

I, Margarita Smoldareva, confirm that the work presented in this assessment is my own. Where information has been derived from other sources, I confirm that this has been indicated 
in the work.


*Margarita Smoldareva*

8th September 2023
