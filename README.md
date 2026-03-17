# CONVOLUTION OF SEQUENCES

## Aim:

To perform linear convolution using MAT LAB.

## Software Required:

MAT LAB R2012

## Algorithm:

Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 

~~~
% D.MATHIYAZHAGAN 212223050028
clc; % clear screen
 clear all; % clear screen
 close all; % close all figure windows
% INPUT SEQUENCE
a=input('enter the starting x(n)');
x=input('enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');
% IMPULSE SEQUENCE
b=input('enter the starting h(n)');
y=input('enter the h(n) sequence');
m=b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impulse response')
% LINEAR CONVOLUTION
z=conv2(x,y);
n1=a+b:1:length (z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude');
title('linear convolution');
~~~

## OUTPUT:

## Input Sequence:

<img width="1681" height="881" alt="image" src="https://github.com/user-attachments/assets/5b4d1213-f008-4aee-8e9d-c32d1952b057" />


## Impulse Response:

<img width="1629" height="873" alt="image" src="https://github.com/user-attachments/assets/eecd94be-b2b8-430a-bb39-0bf6b5e862e3" />


## Linear Convolution:

<img width="1666" height="876" alt="image" src="https://github.com/user-attachments/assets/df581193-b815-497e-bfdf-1a0ace345ccb" />

## RESULT:

The linear Convolution of signal is {6,-11,17.5,4,-0.21,**22.9**,35.05,-18.5,60.5,36.9,13.5,7,6,-3}
