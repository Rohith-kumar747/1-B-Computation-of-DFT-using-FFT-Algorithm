# EXPT 2: Computation-of-DFT-using-FFT-ALGORITHM

## AIM
To perform and verify DFT using FFT-ALGORITHM by SCILAB.
## APPARATUS REQUIRED
PC installed with SCILAB
## PROGRAM 
### DFT FFT-ALGORITHM
```

clc;

clear;

xn = [2 1 2 1 1 2 1 2];

n1 = 0:1:length(xn)-1;

subplot(3,1,1);

plot2d3(n1,xn);

xlabel('Time n');

ylabel('Amplitude xn');

title('Input Sequence');

j = sqrt(-1);

N = length(xn);

Xk = zeros(1,N);

for k = 0:N-1

    for n = 0:N-1

        Xk(k+1) = Xk(k+1) + xn(n+1) * exp((-j*2*%pi*k*n)/N);

    end

end

Xk = round(real(Xk));

disp("DFT Output:");
disp(Xk);
```
### CALCULATIONS:
<img width="904" height="1548" alt="image" src="https://github.com/user-attachments/assets/1f73c502-c9c4-4627-831d-6d9a2d562874" />
<img width="949" height="1546" alt="image" src="https://github.com/user-attachments/assets/8c1ea6f8-2d70-4cd0-a98b-caebf3d6b977" />
<img width="960" height="1569" alt="image" src="https://github.com/user-attachments/assets/dcc2c272-b2e9-4409-b11d-7c33a53a31e3" />
<img width="1600" height="1363" alt="image" src="https://github.com/user-attachments/assets/7cdc8e6f-c63a-4a25-ad0c-583c13ca361a" />

### FFT ALGORITHM:
<img width="910" height="1562" alt="image" src="https://github.com/user-attachments/assets/b23c3dde-39af-4016-a6a2-99649b904b32" />
<img width="939" height="1575" alt="image" src="https://github.com/user-attachments/assets/8eb48ff1-54a2-4af8-bd22-6c14223b6242" />
<img width="957" height="1544" alt="image" src="https://github.com/user-attachments/assets/ef6507cc-d052-4b45-a722-7b12aad2e84b" />
<img width="979" height="1451" alt="image" src="https://github.com/user-attachments/assets/7d7ef5a3-0ec8-4459-a919-ab185309927b" />

### SAMPLE OUTPUT:
<img width="1440" height="612" alt="image" src="https://github.com/user-attachments/assets/acb11e54-096d-4807-9047-2124c8491dbc" />

## RESULT:
Thus,  DFT using FFT-ALGORITHM for two given sequences were performed and its result was verified.

