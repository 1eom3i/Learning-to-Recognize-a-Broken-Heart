# Learning-to-Recognize-a-Broken-Heart

## Problem Description
An arrhythmia is a problem with the rate or rhythm of the heartbeat. Arrhythmia has two 
types which are ventricular fibrillation(VF) and atrial fibrillation(AF). The project mainly 
focuses on the diagnosis of atrial fibrillation(AF).

This project aims to leverage an ECG dataset for phase-space reconstruction, exploring optimal methodologies in the process. Furthermore, it will investigate the potential role of cutting-edge, fully-automated software—developed with the help of convolutional neural networks, a subset of machine learning—in assisting arrhythmia diagnosis. The focus will be on the diagnostic potential drawn from the Reconstructed Phase Space (RPS) of ECG readings.

![1687221864765](https://github.com/1eom3i/Learning-to-Recognize-a-Broken-Heart/assets/124229472/eeb39de4-310e-4a78-a5bd-cada496b9fa9)

## Dataset
ECG recordings, collected using the AliveCor device, were generously donated for this Challenge by AliveCor. The training set contains 8,528 single lead ECG recordings lasting from 9s to just over 60s and the test set contains 3,658 ECG recordings of similar lengths. The test set is unavailable to the public and will remain private for the purpose of scoring for the duration of the Challenge and for some period afterwards.

ECG recordings were sampled as 300Hz and they have been band pass filtered by the AliveCor device. All data are provided in MATLAB V4 WFDB-compliant format (each including a .mat file containing the ECG and a .hea file containing the waveform information). More details of the training set can be seen in Table 2. Figure 1 shows the examples of the ECG waveforms (lasting for 20s) for the four classes in this Challenge. From top to bottom, they are ECG waveforms of normal rhythm, AF rhythm, other rhythm and noisy recordings.

![1687222411845](https://github.com/1eom3i/Learning-to-Recognize-a-Broken-Heart/assets/124229472/9244d144-50bf-4e84-9cc0-7f0cfcc8b157)

## Feature Engineering

### Phase Space Reconstruction
Phase Space Reconstruction (PSR) is a technique often used in time series analysis and can provide significant utility in the diagnosis of Atrial Fibrillation (AF). 

1. **Nonlinear Analysis**: Atrial Fibrillation is a complex condition that cannot always be fully understood using linear methods. PSR is a tool used in nonlinear dynamics that can provide unique insights into the patterns of AF.

2. **Revealing Hidden Dynamics**: The principle of PSR is that it can reveal dynamics in the system (in this case, the heart's electrical activity) that may not be readily apparent in the raw time series data. These hidden dynamics could potentially indicate the presence of AF.

3. **Feature Extraction**: PSR can be used to extract features from ECG data that are useful for machine learning algorithms. These features can potentially improve the performance of these algorithms in diagnosing AF.

4. **Chaotic Behavior**: PSR is particularly suited to examining chaotic behavior, which is often present in AF. This method can help to distinguish AF from normal rhythms by identifying the underlying chaotic dynamics.

## Model
![1687222514129](https://github.com/1eom3i/Learning-to-Recognize-a-Broken-Heart/assets/124229472/d576dc4a-5b4b-45be-afd8-d5ec259472bb)

## Results
