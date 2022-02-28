# EEG_DSP
EEG signal processing using python during normal brain activity and seizure.
Libraries: Scipy, Matplotlib, Pandas, Numpy

Electroencephalography (EEG) biosignal has a widespread popularity to monitor and understand brain acitvity. EEG signals acquired from human scalp are contaminated with the distinct set of artifacts, most of the time. These artifacts affect the uniqueness of the signal due to which medical psychoanalysis and information retrieval may be difficult. Therefore, EEGs are first preprocessed to eradicate the present artifacts to make these signals ready for further signal processing. Noises in EEG signals could affect the accuracy of DoA monitor. The noises in EEG signal are from the muscle, eye movement and blinking, power line, and interference with other device. Those noises are overlapped each other. Hence, monitoring of DoA without removing the noise may result in an incorrect assessmen [[1]](https://core.ac.uk/download/pdf/11050484.pdf).

![alt text](https://github.com/MaryamHamzelu/EEG_DSP/blob/master/eeg.png?raw=true)
[Source](http://https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.gncdubai.com%2Ftreatments%2Fneurological-eeg%2F&psig=AOvVaw3f4VVgOGw3QU7Yj80K6UVc&ust=1646174038152000&source=images&cd=vfe&ved=0CAsQjRxqFwoTCPiTh6u6o_YCFQAAAAAdAAAAABAV)

A seizure is a sudden, uncontrolled electrical disturbance in the brain. It can cause changes in your behavior, movements or feelings, and in levels of consciousness. Having two or more seizures at least 24 hours apart that aren't brought on by an identifiable cause is generally considered to be epilepsy.
During a seizure, the electrical activity is abnormal. Once the seizure is over, the brain rapidly returns to normal in most individuals. When an EEG is done several hours or even days later, it misses the changes in electrical activity that occurred during the actual seizure [[2]](https://www.mayoclinic.org/diseases-conditions/seizure/symptoms-causes/syc-20365711).

In this project we study and visualize different type of noises for one sample (01_05_edfm) in [CHB-MIT dataset](https://www.mayoclinic.org/tests-procedures/eeg/about/pac-20393875), digital infinite impulse response (IIR) and finite impulse response (FIR) filter are implemented to remove or reduce artifacts effects for preprocessing of acquired EEG signals.

The results shows that: 

- Moving average filters (low degree) are cheap, efficient filters to remove high frequency noise.
- Finite impulse response (FIR) filters outperform infinite impulse response (IIR) filter while removing noise from the EEG signals.
- Higher frequencies are often more common in abnormal brain states such as epilepsy, there is a shift of EEG signal energy from lower to higher frequency bands before and during a seizure.
- It can be noticed that the EEG signal power of is shifting from lower to higher frequencies in the presence of epileptiform activity.
