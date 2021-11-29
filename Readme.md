# Realistic Simulated (Bayesian) Marketing Mix Model 

In this notebook, I simulate a realistic marketing mix dataset that exhibits, for example, non-stationary and heterogeneous main effects, non-stationary confounding effects, group (market/geo) effects on intercept and slope, cold starts (geographic expansion), and correlated ad spend across advertising channels, with quite different scales (e.g. Google vs. Pinterest). (There's only so much time in the day, so I chose to not include advertising saturation and adstock decay.)  

I'll pretend we're a company making a new and great coffee pour-over device to make things a bit more concrete, though, of course, it won't affect the math much.  

I'll start by investigating with some frequentist models - both reasonably well- and quite mis-specified. Then I'll compare them with a few Bayesian models. Note that to keep this semi-realistic, none of the models will perfectly capture the data-generating process. E.g. we'll (at least to start with) assume stable coefficients over time and have an incomplete understanding of confounding (latent variables). We'll see how much bias we end up with - can with get our incremental return on ad spend _about_ right? Can we rank our channel effectiveness successfully?  

As a side comparison, I'll see whether we could've gotten away with using variational inference to fit our Bayesian models. (I tend to be a bit suspicious of these results after some bad experiences in the past.)  

(Please see detailed results in the notebook! If I wrote them here, I'd inevitably forget to update the readme when I revised the notebook.)  
