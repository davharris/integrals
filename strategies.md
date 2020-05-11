# Fundamental integration strategies

Most methods for integration involve one of three fundamental approaches.

* Solve the integral. In rare cases (e.g. polynomials), the function is simple enough that a Calculus student or *Mathematica* can solve the integral. 
    * As far as I can remember, this has literally never happened for any of the functions I've needed to integrate in my career. 
    * In some other cases (e.g. [conjugate priors](conjugate_priors.md)), a real mathematician has already done the integral. This is extremely handy, when it works.
    * In the vast majority of cases, there is no closed-form solution, and you have to choose one of the other approaches described below.

* If you can't solve the function of interest, replace it with one whose solution is known. 
    * In my career, the replacement function has always been a Gaussian distribution. Depending on how you choose the parameters for the replacement function, this approach can give you [Laplace approximation](laplace.md), [variational approximation](variational.md), or [expectation propagation](expectation_propagation.md).

* Calculate the value of the function at a finite number of points, assign a weight to each one, and add them up. 
    * This covers an enormous array of methods, including some that are taught in basic calculus classes (like the [trapezoid rule](trapezoid.md)), as well as most methods used in practical applications. These include [Monte Carlo](monte_carlo.md) methods, [Gaussian quadrature](gaussian_quadrature.md), etc. Basically, this is the whole field of numerical integration.

There are definitely [other](https://en.wikipedia.org/wiki/Planimeter) [ways](https://en.wikipedia.org/wiki/Integraph) of estimating integrals, such as [literally cutting the function out of paper and weighing the pieces on a scale](https://books.google.com/books?id=juoR2_rnIuAC&pg=PA477&lpg=PA477&dq=cut+%22graph+paper%22+integral+weigh+scale&source=bl&ots=ZZCtUpt5dk&sig=ACfU3U3bLVbY7mhMNEnMuFwceo0lcWGcRg&hl=en&sa=X&ved=2ahUKEwi90q6cx6rpAhUQmHIEHbcUDE4Q6AEwDXoECAoQAQ#v=onepage&q=cut%20%22graph%20paper%22%20integral%20weigh%20scale&f=false), and there are special approaches for certain kinds of problems like differential equations, but we won't focus on them here.
