# econ3916-lab09-ab-testing

# A/B Testing — Designing the Data-Generating Process

## Objective
In this lab, I explored how randomized experiments, selection bias, and statistical testing help us estimate treatment effects and make decisions using data.

## Methodology
- Loaded the LaLonde NSW job training dataset with 445 participants, including 185 trainees and 260 controls.
- Calculated the experimental Average Treatment Effect (ATE) by comparing earnings between the treatment and control groups.
- Simulated an observational comparison group to examine selection bias and the relationship between observational ATE, true ATE, and selection bias.
- Conducted a permutation test with 9,999 shuffles and calculated a bootstrap BCa 95% confidence interval.
- Performed a power analysis to estimate the study's statistical power and the sample sizes needed to detect different treatment effects.
- Analyzed the Cookie Cats A/B test with 90,189 players to compare Day-1 retention between gates at levels 30 and 40.
- Created an `n_needed()` function to calculate the required sample size for future experiments.

## Key Findings

### LaLonde Job Training Experiment
- The experimental ATE measured the difference in average earnings between trainees and controls.
- The simulated observational comparison demonstrated how selection bias can affect estimated treatment effects.
- The permutation test and bootstrap confidence interval helped assess the statistical significance and uncertainty of the estimated ATE.

### Cookie Cats A/B Test
- The gate_30 group had a Day-1 retention rate of approximately 44.82%, compared with 44.23% for gate_40.
- The observed retention difference was **0.59 percentage points**, favoring gate_30.
- The permutation test gave a p-value of approximately **0.075**, indicating that the difference was not statistically significant at the 5% level.
- The bootstrap 95% confidence interval was approximately **[-0.06, 1.24] percentage points**, which includes zero.
- The power analysis showed how sample size affects our ability to detect small differences in retention.

## Conclusion
Through this lab, I learned how randomized experiments help estimate causal effects and how selection bias can influence observational results. I also learned to use permutation tests, bootstrap confidence intervals, and power analysis to evaluate A/B test results and plan future experiments.
