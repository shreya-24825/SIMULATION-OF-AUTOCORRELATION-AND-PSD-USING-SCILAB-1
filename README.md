# SIMULATION-OF-AUTOCORRELATION-AND-PSD-USING-SCILAB-1

__AIM:__

Write a program for Autocorrelation and PSD of signals in SCILAB and verify Wiener-Khinchin relation. 


__EQUIPMENTS Needed:__

.Computer with i3 Processor 

.SCI LAB


__THEORY:__

The Wiener-Khinchin theorem states that the power spectral density of a wide sense stationary random process is the 
Fourier transform of the corresponding autocorrelation function.

__Algorithm:__

 1.Load or Define the Signal: Input your time-domain signal. 

 2.Compute Autocorrelation: Calculate the autocorrelation function of the signal.

3.Compute Power Spectral Density (PSD): Estimate the PSD of the signal, either directly using a method like
Welch’s periodogram or by using the Fourier transform of the autocorrelation.

4.Plot Results: Visualize the autocorrelation function and PSD. 

__PROCEDURE:__


Refer Algorithms and write code for the experiment. 

Open SCILAB in System 

Type your code in New Editor 

Save the file 

Execute the code 

If any Error, correct it in code and execute again 

Verify the generated waveform using Tabulation and Model Waveform 

__PROGRAM:__
```
clc;
clear all;
t=0:0.01:2*%pi;
x=sin(2*t);
subplot(3,2,1);
plot(x);
au=xcorr(x,x);
subplot(3,2,2);
plot(au);
v=fft(au);
subplot(3,2,3);
plot(abs(v));
fw=fft(x);
subplot(3,2,4);
plot(fw);
fw2=(abs(fw)).^2;
subplot(3,2,5);
plot(fw2);
```

__OUTPUT:__
<img width="1600" height="1200" alt="image" src="https://github.com/user-attachments/assets/3dd49d48-ac45-4c9c-b705-a7b578a95bc8" />


__RESULT:__
Thus authocorrelation and PSD are executed and simulation is obtained.
