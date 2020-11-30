Lab 2: Drawing an SCM, simulating a DGP, and estimating the ATE

Tianran Zhang

1. Draw DAG for this SCM

2. Exclusion restrictions: exclusion restrictions on the parents of X; exclusion restriction of the impact of W2 on the outcome.

   Independence assumptions: None.

3. Counterfactual outcomes of interest

   In words:

   * $Y_1$ : counterfactual score for a medical student if possibly ate dark chocolate right before the exam started.

   * $Y_0$ : counterfactual score for a medical student if possibly did not have dark chocolate right before the exam started.

   Notation: 

   * $Y_1 <- f_Y(W_1, 1, U_Y)$ 
   * $Y_0 <- f_Y(W_1, 0, U_Y)$ 

4. The counterfactuals are uniquely determined by U and F.

5. The distribution of U implies the distribution of the counterfactuals. 

   $U = (U_{W_1}, U_A, U_Y) \sim P^*$ 

6. Other possible target causal parameters: 

   ?

7.   

   $\begin{align} \theta^*(P^*) & = E^*(Y_1) - E^*(Y_0) = E^*[f_Y(W_1, 1, U_Y)] - E^*[f_Y(W_1, 1, U_Y)] \\ &= E^*[1 + 2.5 * 1 + 3 * W_1 - 0.25 * 1 * W1 + U_Y] - E^*[1 + 2.5 * 0 + 3 * W_1 - 0.25 * 0 * W1 + U_Y] \\ &= E[3.5 + 2.75W_1 + U_Y] - E[1 + 3W_1 + U_Y] \\ &= -0.25E[W_1] \\ &= 2.5 -0.25 * 0.35 \\ &= 2.4125 \end{align}$

8.  $\theta^*(P^*) = 2.4125$ means that the expected scores for medical students who ate dark chocolate before an exam would be 2.4125 higher than those who did not have dark chocolate.
