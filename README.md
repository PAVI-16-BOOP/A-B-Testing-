**Introduction**

This case study describes an A/B experiment on a website’s landing page aimed at boosting user engagement. We measured the click-through rate (CTR) – the percentage of visitors who click the main 
call-to-action after viewing the page. The control (original page) had a CTR of 19.89%, while a redesigned “experimental” page was tested against it. Our core question was: Does the new design significantly 
increase CTR above our business target (minimum detectable effect)?

*Goal*

The goal was to achieve a meaningful lift in CTR over the baseline. In business terms, we set a Minimum Detectable Effect (MDE) of 10 percentage points . In other words, we needed at least a 10‑point increase in 
CTR (from ~19.9% to ~29.9%) to consider the change worthwhile.This MDE represented the smallest improvement our stakeholders cared about, ensuring that any detected effect would have practical value.



![Initial CTR condition](Screenshot%202026-01-08%20225516.png)


*Methods*

We used a classic randomized controlled design to compare the original and new landing pages. Key steps included:

- Split Traffic: Visitors were randomly assigned to the control (current design) or variant (new design) page.
- Metric: For each group, we measured CTR as (number of clicks) / (number of page views) – the fraction of users who clicked the call-to-action
- Statistical Test: We applied a two-sample z-test for proportions (95% confidence, two-tailed) to compare the CTRs of the two groups . We computed the corresponding p-value and a 95% confidence interval (CI)
 for the difference in CTR.

This methodology ensured a rigorous comparison. By using a large sample, we achieved high statistical power to detect even modest effects, while checking that any detected effect met our practical threshold.

*Results*

The experimental page dramatically outperformed the control. Key findings:
Control CTR: 19.89% Variant CTR: 61.16% Absolute Uplift: 41.27 percentage points (61.16% − 19.89%) Z-Statistic: 59.44 (two-tailed) P-value: < 0.001 (essentially 0.000)
95% Confidence Interval for Uplift: [0.40, 0.425] (i.e. 40.0% to 42.5%)

*Business MDE: 10%*

These results speak for themselves. The new design’s CTR (61.16%) is enormously higher than the control’s (19.89%), yielding a 41.27-point lift. The z-test gives z ≈ 59.44 with p < 0.001, which is 
vanishingly small – far below the usual 0.05 threshold for significance. In practical terms, this means we confidently reject the null hypothesis of “no difference” and conclude the lift is real.
Moreover, the 95% confidence interval for the CTR increase is [40.0%, 42.5%]. Importantly, this entire interval lies well above zero. As noted by Statsig, when a CI stays above zero, it signals a positive 
effect – essentially a green light that the change is effective. In other words, we are 95% confident that the true CTR lift is between 40% and 42.5%, which is enormous.
Finally, the lift vastly exceeds our business requirement. The lower bound of the CI (40%) is four times higher than our MDE of 10%. In line with best practices, this confirms the effect is not only statistically
significant but practically significant too. (As one data scientist points out, with large samples even tiny differences can be statistically significant – so it’s crucial to check that the effect size is big enough to matter.)
Here, the effect size dwarfs the 10% threshold, meaning the gain is unquestionably meaningful for the business.

*Conclusion*

The experiment yielded a clear, decisive result: the new landing page dramatically improves CTR by over 40 points. Both the statistical test and the practical significance criterion are satisfied. 
The evidence strongly supports deploying the experimental design to all users. Rolling out the new page should substantially boost user engagement, as the CTR increase is both highly reliable and far beyond our minimum goal. 
This case is a textbook example of data-driven decision-making: the numbers speak with overwhelming confidence, and we proceed to launch the winning variant.
