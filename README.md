# EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
## PROGRAM 
### DFT FFT-ALGORITHM
```
clear;
clc;
close;
xn = [1 2 3 4 4 3 2 1]
n1=0:1:length(xn)-1;
subplot(2,2,1);
plot2d3(n1,xn);
xlabel('Time n');
ylabel('Amplitude');
title('Input Sequence');
Xk = fft(xn);
K1=0:1:length(Xk)-1;
magnitude=abs(Xk)
subplot(2,2,2);
plot2d3(K1,magnitude);
xlabel('frequency(Hz)');
ylabel('magnitude(gain)');
title('magnitude spectrum');
angle = atan(imag(Xk),real(Xk))
subplot(2,2,3);
plot2d3(K1,angle);
xlabel('frequency(Hz)');
ylabel('Phase');
title('Phase spectrum')
y= ifft(Xk)
n2=0:1:length(y)-1;
subplot(2,2,4)
plot2d3(n2,y)
xlabel('Time n');
ylabel('Amplitude');
title('Inverse FFT OF X(K)');

```

### CALCULATIONS:
<img width="500" height="800" alt="image" src="https://github.com/user-attachments/assets/30060166-786b-4c59-ab19-a9e0461ad89a" />
<img width="500" height="800" alt="image" src="https://github.com/user-attachments/assets/df5260aa-fda7-4a6d-a1b4-5b0e27b2b4ff" />
<img width="500" height="400" alt="image" src="https://github.com/user-attachments/assets/2026b9dd-b607-4491-bcc6-7301e0982a49" />

### SAMPLE OUTPUT:
<img width="500" height="500" alt="image" src="https://github.com/user-attachments/assets/038db21c-dfd2-4213-a7e1-e59135e9b89b" />



## RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

