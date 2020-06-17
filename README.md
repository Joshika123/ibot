# ibot
Matlab assignment2 

problem 3:
x = [1:10];
y = [21, 43, 34, 56, 67, 89, 90, 25, 65, 80];
bar(x,y,"r"),xlabel('minus'),ylabel('plus'),title('plusminus');

ASSIGNMENT3

PROBLEM 1:
 A = [ 3, 6, 4; 1, 5, 0; 0, 7, 7 ]
A =

   3   6   4
   1   5   0
   0   7   7

>> B = [ 1; 2; 3 ]
B =

   1
   2
   3

>> x = A\B
x =

  -0.582418
   0.516484
  -0.087912
  
  ASSIGNMENT 3
  
  PROBLEM 2:
   quad('x.*exp(-x.^(x/3))',0,5)
ans =  0.96746

ASSIGNMENT 4

PROBLEM1
>> a = 5;
>> b = 2;
>> y = a.*randn(500,1) + b;
>> stats = [ mean(y) std(y) ]
stats =

   1.6948   4.8709
   
ASSIGNMENT4

PROBLEM 2
rep = 5000;
>> flips = round(rand(1,rep));
>> headEvent = cumsum(flips);
>> totalEvent = 1:rep;
>> headProbability = headEvent./totalEvent;
>> Plot(totalEvent,headProbability,totalEvent,0.5*ones(1,rep));
error: 'Plot' undefined near line 1 column 1
>> plot(totalEvent,headProbability,totalEvent,0.5*ones(1,rep));




