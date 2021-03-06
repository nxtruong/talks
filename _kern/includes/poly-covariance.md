\helpercode{%load -s polynomial_cov mlai.py}
\setupcode{import teaching_plots as plot}
\setupcode{import numpy as np}

\code{x=np.linspace(-1, 1, 30)[:, np.newaxis]
\code{plot.covariance_func(x, mlai.compute_kernel, 
                     formula = r'$$k(\inputVector, \inputVector^\prime) = \alpha(w \inputVector^\top \inputVector^\prime + b)^d$$', 
                     shortname='poly', 
                     longname='Polynomial', 
					 kernel=polynomial_cov,
                     degree=4., 
					 diagrams='../slides/diagrams/kern')}


### Polynomial Covariance

$$k(\inputVector, \inputVector^\prime) = \alpha(w \inputVector^\top
\inputVector^\prime + b)^d$$

\columns{
\includesvg{../slides/diagrams/kern/poly_covariance.svg}
}{
\includegif{../slides/diagrams/kern/poly_covariance.gif}{80%}
}{50%}{50%}

