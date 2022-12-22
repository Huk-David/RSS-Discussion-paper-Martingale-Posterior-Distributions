# RSS Discussion contribution paper on Martingale Posterior Distributions
Code for a discusssion paper on Fong et al. Martingale posterior distributions, 2021 (link: https://doi.org/10.48550/arxiv.2103.15671). I have a notebook for reproducing some of the figures in the original paper, as well as doing experiements for our discussion contribution. The main focus of those is robustness to miss-scpecification of the model.

INSTRUCTIONS:
The relevant experiment is in the section 'DPMM example, section 4.2 in the RSS paper'. Run the first block  'Generating observations function'. Then run a subsection below titled 'Energy Prequential Scoring Rule' to define the SR. Then finally the section below that titled 'SR estimate with fast function evaluation' is the main body of work. It defines the update function and does the updating for a given value of rho. There are two loops, the outer one for generating different observed data, the inner one to compute the SR for different values of rho for the given observed data.


TODO -
Implement a regression example with a Normal linear model with known variance and unknown mean. The first n obsevations come from the true distribution but 2 of them have another mean parameter value. We then perform parameter estimation for the mean under the copula based formulation with 2 methods: mle and energy scoring rule. Our aim is to show that using the energy scoring rule results in more robustness to model misspecification when compared to mle.
