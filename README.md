# CONSTRUCT

_**Nikolai Andrianov**, nandria@dtu.dk_

_March 18, 2004_

## Overview

CONSTRUCT is a collection of MATLAB routines for constructing exact solutions to the Riemann problem for the following hyperbolic systems
* Baer-Nunziato model for the deflagration-to-detonation transition (DDT) in gas-permeable, reactive granular materials; 
* Euler equations in a duct of variable cross-section;
* Shallow water equations.

All these models are described by a set of non-conservative, non-strictly hyperbolic systems of partial differential equations.
By non-conservtive we mean that the system cannot be written in divergence form.
Due to non-strict hyperbolicity of the systems, the solution to the Riemann problem becomes much more complicated, compared to the case
of a strictly hyperbolic system. Indeed, the waves in the Riemann solution cannot be order *a priori* by their propagation speeds.
Therefore, in order to find a solution to the Riemann problem one has to consider a number of different cases. Although this can be done
for simple systems like the Euler equations in a duct and the shallow water equations, 
for bigger systems like the Baer-Nunziato model it becomes too complicated.
An alternative way to obtain exact solutions to a Riemann problem is to consider its *inverse* solution, that is to prescribe the solution
and to find the initial data, which correspond to this solution. This is the algorithm, implemented in CONSTRUCT.

With CONSTRUCT, one can easily obtain exact solutions which have potentially interesting properties, e.g. with coinciding wave speeds or
almost vacuum states. The exact solutions can be used e.g. to assess the performance of numerical methods developed for non-conservative
systems like listed above. This question becomes more important since the solution to the Riemann problem for these systems appears
to be in general non-unique.

For more information on the structure of the Riemann problem for the models listed above, see the references below.

## References

1. N. Andrianov, Testing numerical schemes for the shallow water equations,
preprint, 2004.  Available at https://github.com/nikolai-andrianov/CONSTRUCT/blob/master/testing_sw.pdf.
2. N. Andrianov and G. Warnecke, The Riemann problem for the Baer-Nunziato two-phase flow model,
 *J. Comput. Phys.* **195**, 434-464 (2004).
3. N. Andrianov and G. Warnecke, On the solution to the Riemann problem for the compressible duct flow,
*SIAM J. Appl. Math.* **64**(3), 878-901 (2004).
