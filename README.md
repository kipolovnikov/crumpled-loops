# crumpled-loops
A minimal polymer physics model for ensemble of random loops on a crumpled chain

It contains a Jupyter notebook for numerical calculation of $P(s)$ for a fractal polymer chain folded into random loops. In addition, we provide precalculated contact probabilities by diagrams for various parameters.   

Parameters of the system:
- Mean loop size $\lambda$;
- Mean spacer size $g$; density $d=\lambda/g$;
- Kuhn segment $l_k$;
- Fractal dimension $d_f$;
- Volume density $\varphi$;
- Entanglement length $N_e$ of the chain without loops; 
$N_e$ is a function of volume density $\varphi$, Kuhn segment $l_k$, loop size $\lambda$ and loop density $d$. 

The effect of the loops on is computed in the approximation of quenched loops disorder: the loops are randomly positioned and fixed on each conformation;
the chain is further equilibrated together with its loops.

The full list of assumptions of the model:
- quenched disorder of loops (equilibration is faster than extrusion at the scales of interest);
- Gaussian measure of chain conformations;
- absense of nested or overlapping loops;
- exponentially distributed sizes of loops and spacers;

As proposed in the paper, the short-scale loops on the chain are approximately ideal, since their size is less or of order of the real entanglement length.
Thus, the entanglement length of the chain with loops (of the backbone chain) importantly depends on the loop density: shorter the backbone, larger is $N_e$.
The expression for $N_e$ as a function of loop size $\lambda$ and loop density $d$ is derived in the paper. Here one can compute the contact probability $P(s)$
with the theoretical entanglement length corresponding to other parameters of the system, or with a phenomenological $N_e$ provided by the user.

The folder "data" contains files with $P(s)$ for the following parameters: $\lambda=100, 200$; $\varphi=0.1, 0.2, 0.3$; $d_f=2.7$, $l_k=3.5$ and different density values. The file names structured as `ideal_br_exp_N_e__l_*__g_*__N_e_*__phi_*__l_k_*__d_f_*.txt` where each * is the value of the according parameter (l is for $\lambda$). The value of the entanglement length $N_e$ is calculated for the given volume density, Kuhn segment, loop size and loop density. Each file contains 6 columns: $s$, $P_a(s)$, $P_b(s)$, $P_c(s)$, $P_d(s)$ and $P(s)$. 

Authors: Bogdan Slavov, Kirill Polovnikov.

For any purpose contact: kipolovnikov@gmail.com (Kirill)
