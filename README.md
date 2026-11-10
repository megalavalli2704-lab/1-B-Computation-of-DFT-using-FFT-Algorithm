# EXPT 1b: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
## PROGRAM 
### DFT FFT-ALGORITHM

    INDIRECT METHOD:

    clc;
    clear;
    clf;
    
    xn = [1,2,3,4,4,3,2,1];
    N = length(xn);
    n = 0:N-1;
    
    Xk = fft(xn);
    
    disp("FFT output:");
    disp(Xk);
    
    K = 0:N-1;
    magnitude = abs(Xk);
    phase = atan(imag(Xk), real(Xk));
    
    y = ifft(Xk);
    
    subplot(2,2,1);
    plot2d3(n, xn);
    xtitle("Input Sequence", "n", "x(n)");
    
    subplot(2,2,2);
    plot2d3(K, magnitude);
    xtitle("Magnitude Spectrum", "k", "|X(k)|");
    
    subplot(2,2,3);
    plot2d3(K, phase);
    xtitle("Phase Spectrum", "k", "Phase (radians)");
    
    subplot(2,2,4);
    plot2d3(n, real(y));
    xtitle("Inverse FFT Output", "n", "x(n)");


### CALCULATIONS:
<img width="979" height="1533" alt="WhatsApp Image 2026-11-10 at 2 02 38 PM" src="https://github.com/user-attachments/assets/08d9c015-8b51-4fe8-989c-b1ad6f339124" />

<img width="1019" height="1554" alt="WhatsApp Image 2026-11-10 at 2 02 50 PM" src="https://github.com/user-attachments/assets/c6198ddd-394e-436e-a317-de096adc30dd" />

<img width="855" height="1470" alt="WhatsApp Image 2026-11-10 at 2 03 08 PM" src="https://github.com/user-attachments/assets/91596756-348b-480c-b5ac-f033d385c288" />

<img width="987" height="1514" alt="WhatsApp Image 2026-11-10 at 2 03 23 PM" src="https://github.com/user-attachments/assets/f13f8216-fcd2-4e0a-89f3-868e258548f9" />

### SAMPLE OUTPUT:

<img width="1599" height="1307" alt="WhatsApp Image 2026-11-10 at 2 03 43 PM" src="https://github.com/user-attachments/assets/937e0fb0-0a8c-4e73-98b9-1a9b4f7025fa" />

## RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

