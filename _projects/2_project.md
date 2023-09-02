---
layout: page
title: Convex Optimization in Trust Region Policy Optimization
description: 

img: assets/img/16.png
importance: 2
category: Work
giscus_comments: true
---
This research investigates the application of Trust Region Policy Optimization (TRPO) in reinforcement learning using convex optimization techniques. Utilizing the CVX software suite, we construct and resolve the restricted optimization problem that develops during the policy optimization phase. Our findings point to fresh directions for future study in this field and show how convex optimization might be used to solve the challenge of policy optimization. Our work has sig- nificant applications in fields including robotics, autonomous systems, and making decisions in the face of uncertainty.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/15.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/18.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/17.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    optimization analysis vs parameters and code snippet 
</div>

To assess the performance of the TRPO algorithm under different discount factors, we evaluate its performance across a range of 𝛾 values. Figure 2 illustrates the performance of the algorithm as the discount factor varies. The plot shows that as 𝛾 increases, the average performance also increases, indi- cating a stronger consideration for future rewards. However, beyond a certain point, the performance saturates, suggest- ing diminishing returns for higher 𝛾 values. This trade-off between immediate and future rewards can be crucial in designing policies for reinforcement learning tasks.



We plot the surrogate objective function versus x to visu- alize the behavior of the optimization process. The surro- gate objective function captures the expected return of each state-action pair and serves as a proxy for the true objective function.
Figure 3 shows the plot of the surrogate objective func- tion as a function of x. The graph provides insights into the optimization landscape and helps in understanding how the algorithm explores different states to find the optimal
solution.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/19.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    code snippet
</div>

The Trust Region Policy Optimization (TRPO) algorithm was applied in this research, and its effectiveness with regard to a reinforcement learning problem was assessed. Our research revealed that the TRPO algorithm successfully increased expected returns by optimizing policy parameters.


The algorithm’s capacity to recognize state-action com- binations with high expected returns was highlighted by the comparison of the optimal solution to the state variable and optimization was shown by the graph of the surrogate objective function.


We also looked into how the discount factor 𝑔𝑎𝑚𝑚𝑎 af- fected performance. The trade-off between now and future benefits was exposed by the many optimal solutions for var- ious 𝑔𝑎𝑚𝑚𝑎 values. Future research could compare TRPO to other reinforcement learning algorithms and apply it to more complicated situations.
Overall, the TRPO algorithm demonstrated its efficiency in maximizing expected returns and optimizing policy pa- rameters. This project improved our comprehension of op- timization and reinforcement learning approaches, which helped to advance their usefulness.