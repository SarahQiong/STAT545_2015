This is the repository of Qiong Zhang(for STAT 545)
=====================================

This is a Markdown document.

## Self Introduction

> For Today’s Graduate, Just One Word: Statistics.

Hi, my name is __Qiong__, a first year *Ms.c.* student in department of Statistics. So happy to meet you and thanks for the help of Jenny, the TAs and other classmates. I'm interested in data analysis and plan to study Python by myself.



## My Experience of Assignment 1

- I googled when I learned how to use Markdown syntax, there's a help page on Github is very useful, here it is:[Visit Github page!](https://help.github.com/articles/markdown-basics/)

- I commit first and then push the readme file, I felt so strange that the readme file disappered. Then Mary told me it is the right thing to do, thanks Mary for her help. 

- I think push from shell or the git command line is not very hard, you can follow the steps on github after you create your new repository.

- I don't know how to show the hist plot of my new random variable...Need help with that, I save the photo in my public repository name repo-for-STAT545, and I copied the link, it doesn't work. Stiil have no idea about insert a picture in this way, but I find another way, here is the useful guide: [useful guide!](http://solutionoptimist.com/2013/12/28/awesome-github-tricks/)
## For Fun!
Just put a simulation code here for fun.

We want to simulation an exponential distribution from a uniform distribution on [0,1], which means ![equation](http://www.sciweavers.org/upload/Tex2Img_1442978223/render.png). We hope to build X using Y.


If Y have the following form, then ![equation](http://www.sciweavers.org/upload/Tex2Img_1442978520/render.png):
![equation](http://www.sciweavers.org/upload/Tex2Img_1442978551/render.png)

where ![equation](http://www.sciweavers.org/upload/Tex2Img_1442978606/render.png)

Here is the explanation:

F is continuous and has inverse,thus
![equation](http://www.sciweavers.org/upload/Tex2Img_1442978649/render.png)



Simulation with R, here is the R code:
```
n = 1000000;
lambda = 1/2;
x = runif(n,0,1);
y = (1/lambda) * log(1/(1-x))
hist(y)
```
This is the hist plot of Y:

![Hist plot of Y](https://cloud.githubusercontent.com/assets/14189534/10037441/e084eed0-616a-11e5-9a1f-4f8e9432df40.png)

This is a exponential distribution get from a uniform distribution on [0,1]. Amazing! 

It seems like for continuous distribution, uniform distribution is enough to build others.
