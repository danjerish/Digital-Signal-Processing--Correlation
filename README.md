# Digital-Signal-Processing--Correlation
## AIM:
To generate discrete auto correlation and cross correlation of signals using MATLAB.
## APPARATUS REQUIRED:
MATLAB R2012.
## ALGORITHM:
Step 1: Open matlab. Write the program.

Step 2: Read the input sequence 1 and input sequence 2 sequence.

Step 3: Perform auto correlation and cross correlation for both the sequences. 

Step 4: Plot the output sequence with x-label and y-label with suitable title.

Step 5: Terminate the program.


## PROGRAM: 
clc; % clear screen 
clear all; % clear screen 
close all; % close all figure windows 
% INPUT SIGNAL-1 
x=input(‘Enter the x(n) sequence’) 
n=0:1:length(x)-1 
figure(1) 
stem(x) 
xlabel(‘Time’) 
ylabel(‘Amplitude’) 
title(‘Input Signal-1’) 
% INPUT SIGNAL 2 
y=input(‘Enter the y(n) sequence’) 
n1=0: 1:length(y)-1 
figure(2) 
stem(y) 
xlabel(‘Time’) 
ylabel(‘Amplitude’) 
title(‘Input signal-2’) 
% DISCRETE AUTO CORRELATED SIGNAL 
out1=xcorr(x,x) 
figure(3) 
stem(out1) 
xlabel(‘Time’) 
ylabel(‘Amplitude’) 
title(‘ Discrete auto correlated waveform’) 
% DISCRETE CROSS CORRELATED SIGNAL 
Out2=xcorr(x,y) 
figure(4) 
stem(out2) 
xlabel(‘Time’) 
ylabel(‘Amplitude’) 
title(‘ Discrete cross correlated waveform’)

## OUTPUT:
<img width="1917" height="1069" alt="Screenshot 2025-09-26 184654" src="https://github.com/user-attachments/assets/e3ddd385-3788-4e58-a85e-760e478c5b61" />

## RESULT:
![EXP2](https://github.com/user-attachments/assets/f2e5db1d-b757-43c0-b8e6-d9022df91240)

