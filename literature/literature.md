# Bayesian Optimisation vs Response Surface Methodology (RSM)

Response Surface Methodology (RSM) and Bayesian Optimisation (BO) are two commonly used approaches for process optimisation. Both methods are widely used, especially in experimental and manufacturing processes (Durante et al., 2020; Shahriari et al., 2016). RSM is a traditional statistical technique that focuses on designing experiments, building empirical models, and identifying optimal input conditions that produce the desired output. It typically uses structured experimental designs (such as Central Composite Designs) and polynomial equations to model the relationship between input variables and responses (Srinivasan et al., n.d.). This makes RSM straightforward to apply and interpret, which is why it has been widely used in industrial experimentation and quality improvement processes (Tang et al., 2010).

However, RSM has some limitations. It usually assumes a fixed model form (often quadratic), meaning it may struggle to accurately represent complex, highly non-linear relationships between variables such as those of Albotherm’s experiments. Additionally, RSM relies on pre-planned experiments. Thus, it does not adapt dynamically as new data becomes available. This can lead to inefficiencies, especially when experiments are expensive or when the design space is large and complex (Njouond Kamdem et al., 2026).

Bayesian Optimisation, on the other hand, is a more modern, machine learning-based approach designed specifically for optimising expensive or unknown “black-box” functions. Instead of assuming a fixed model, BO builds a probabilistic surrogate model (commonly a Gaussian process) that estimates both the expected output and the uncertainty of that prediction (Frazier, 2018). This uncertainty is a key advantage, as it allows the method to intelligently decide where to run the next experiment.

The optimisation process in BO is iterative. After each experiment, the model is updated, and an acquisition function is used to determine the next best point to evaluate. This function balances two important goals: exploring new areas of the design space and exploiting areas that already show promising results (Frazier, 2018). As a result, BO is highly data-efficient and can find optimal solutions with fewer experiments compared to traditional methods.

Another major strength of Bayesian Optimisation is its flexibility. It does not require assumptions such as linearity or simple polynomial relationships in the same way RSM does, and it can handle noisy data, and complex interactions between variables more effectively (Tang et al., 2010). It also allows for adaptive experimental design, meaning each new experiment is chosen based on all previous results rather than being fixed in advance.

Despite its strengths, Bayesian Optimisation has issues with high dimensionality. This is due to its nature that as the number of input variables increases, the number of evaluations required to cover the search space grows exponentially (Shahriari et al., 2016). Therefore, its efficiency and practical applicability can diminish significantly in high-dimensional systems, such as that of Albotherm’s, which are common in complex chemical process optimisation problems.

In direct comparisons, Bayesian Optimisation often performs better than RSM in complex optimisation tasks. For example, studies have shown that BO can achieve significantly higher predictive accuracy (higher R² values) and lower error metrics than RSM when applied to real-world process optimisation problems (Njouond Kamdem et al., 2026). This suggests that BO is better at capturing the true underlying relationships in complex systems. Additionally, in chemical process optimisation, experiments are typically expensive and time-intensive. This is especially applicable for Albotherm as it is a start-up organisation and cost-effectiveness is vital. Due to its ability to find optimal conditions using relatively few experimental evaluations, Bayesian optimisation can provide a practical advantage (Desimpel et al., 2026).

In summary, RSM is a reliable and simple method that works well for smaller, well-understood problems with relatively simple relationships between variables. However, Bayesian Optimisation is generally more powerful and efficient for modern applications, particularly when dealing with complex systems, limited experimental budgets, or unknown functional relationships. Because of its ability to learn from data, adapt experiments, and incorporate uncertainty, BO is increasingly preferred for advanced optimisation tasks.

## References

Desimpel, S., Dorbec, M., Van Geem, K.M. and Stevens, C.V. (2026) Bayesian Optimization For Chemical Reactions. Chemical Society Reviews [online]. 55, pp. 2731-2775. [Accessed 17 April 2026].

Durante, M., Ferramosca, A., Treppiccione, L., Giacomo, M.D., Zara, V., Montefusco, A., Piro, G., Mita, G., Bergamo, P. and Lenucci, M.S. (2020) Application of Response Surface Methodology (Rsm) For the Optimization of Supercritical Co2 Extraction of Oil From Patè Olive Cake: Yield, Content of Bioactive Molecules and Biological Effects in Vivo. Food Chemistry [online]. 332 [Accessed 23 April 2026].

Frazier, P.I. (2018) A tutorial on Bayesian optimization. Available at: https://arxiv.org/abs/1807.02811 
(Accessed: 21 April 2026).

Njouond Kamdem, D., Kenmogne, S.B. and Wansi, J.D. (2026) Methodological approach to response surfaces and Bayesian optimization using the Gaussian process as predictive tools for lignin extraction. Available at: https://doi.org/10.21203/rs.3.rs-8781383/v1 
(Accessed: 21 April 2026).

Shahriari, B., Swersky, K., Wang, Z., Adams, R.P. and Freitas, N. (2016) Taking the Human Out of the Loop: A Review of Bayesian Optimization. [online]. [Accessed 17 April 2026].

Srinivasan, K., Kumar, A., Iyer, P. and Joshi, A. (n.d.) Manufacturing process optimization using statistical methodologies.

Tang, Q., Lau, Y.B., Hu, S., Yan, W., Yang, Y. and Chen, T. (2010) ‘Response surface methodology using Gaussian processes: Towards optimizing the trans-stilbene epoxidation’, Chemical Engineering Journal, 156(2), pp. 423–431. Available at: https://doi.org/10.1016/j.cej.2009.11.002 
(Accessed: 21 April 2026).
