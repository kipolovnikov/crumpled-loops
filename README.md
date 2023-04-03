# crumpled-loops
A minimal polymer physics model for ensemble of random loops on a crumpled chain

It contains a Jupyter notebook for numerical calculation of P(s) for a fractal polymer chain folded into random loops.

Parameters of the system:
- Mean loop size $\lambda$;
- Mean spacer size $g$; density $d=\lambda/g$;
- Kuhn segment $l_k$;
- Fractal dimension $d_f$;
- Volume density $\phi$;
- Entanglement length $N_e$ of the chain without loops; 
$N_e$ is a function of volume density $\phi$, Kuhn segment $l_k$, loop size $\lambda$ and loop density $d$.

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

Authors: Bogdan Slavov, Kirill Polovnikov.

For any purpose contact: kipolovnikov@gmail.com (Kirill)
