# ibot

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

ASSIGNMENT 4

PROBLEM 3
lambda=5;
count=1000;
x=poissrnd(lambda,1,count);
xMin=min(x);
xMax=max(x);
H=histogram(x,'BinEdges',[xMin:xMax],'Normalization','probability');
hold on;
index=linspace(xMin,xMax,count);
plot(index,poisspdf(lambda,index),'r');

ASSIGNMENT 4

PROBLEM 6
>> res=200;
>> x=linspace(0,2*pi,res);
>> y=sin(x);
>> figure;
>> plot(x,y,'r');
>> xlim([0,2*pi]);
>> set(gca,'xtick',[0,pi,2*pi],'xticklabel',{'0','1','2'});
>> set(gca,'ytick',-1:0.5:1);
>> grid on;
>> set(gca,'xcolor','cyan','ycolor','black','color','black');
>> set(gcf,'color',[.3 .3 .3]);
>> title('One sine wave from 0 to 2\pi', 'fontsize', 14,'fontweight', 'bold','color','white');
>> xlabel('multiples of \pi','fontsize',12,'color','cyan');
>> ylabel('sin(x\pi)','fontsize',12,'color','green');






