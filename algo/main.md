---
title: Algorithms
---

I'm going through an MIT OCW [6.006](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-006-introduction-to-algorithms-fall-2011/index.htm), which uses the CLRS book. Below are my notes:

(12/15) Bloomberg [opinion](https://www.bloomberg.com/opinion/articles/2018-03-15/computer-algorithms-need-to-know-what-fair-means) on the social impact of algorithms and how they should incorporate "fairness". In the context of credit ratings: assigning equal ratings to minorities or completely ignoring demographics are two end of the spectrum. They symbolize progressives and corporate interest, respectively. The right balance is to give loans to the disadvantaged group at rates higher than the max profit scenario. Quantitatively, this [work](https://arxiv.org/abs/1803.04383) is about adjusting the optimizer for maximizing some form of utility. 

(12/17) Recommendation engines: store info about users and content as a vector, with elements describing their taste/content. Each element refers to a specific/statistically independent characteristic, with the more powerful indicators first. For gender, one would get assigned 1 if they like things women like and -1 if they lean male. The corresponding element for a video ranges from 1 (content that females love) to -1 (males love it). Other elements could be tendency for violence, humor, lust, etc. To make a recommendation for someone, the algorithm takes a dot product between them and all videos. 

(12/18) Unit 1 , finished both lectures. 

Used a 1D peak finding example to introduce *recurrences* and *asymptotic complexity*, i.e. big-![equation](https://latex.codecogs.com/gif.latex?%5CTheta%2C%20O%2C%20%5COmega) notations). Here is a helpful [ipynb](asymptotic_complexity.html) illustrating these notations. Essentially, they describe an upper bound, lower bound, or both for a function. One benefit is to reduce complex functional forms (such as logarithms). 

Lecture 2 talks introduces two *models of computation* (1) random access machine, RAM (arrays, assembly programming) (2) pointer machines (pointers/references, think OOP).

In Python, lists (arrays) and objects with O(1) attributes (pointers) are basic operations related to the models of computation. L2 then uses the document distance example to discuss algorithm runtime. 
