# DifferentialEquations.jl

[![Join the chat at https://gitter.im/JuliaDiffEq/Lobby](https://badges.gitter.im/JuliaDiffEq/Lobby.svg)](https://gitter.im/JuliaDiffEq/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge) [![Build Status](https://travis-ci.org/JuliaDiffEq/DifferentialEquations.jl.svg?branch=master)](https://travis-ci.org/JuliaDiffEq/DifferentialEquations.jl) [![Build status](https://ci.appveyor.com/api/projects/status/032otj4kh462tq2l/branch/master?svg=true)](https://ci.appveyor.com/project/JuliaDiffEq/differentialequations-jl/branch/master)
[![Coverage Status](https://coveralls.io/repos/github/JuliaDiffEq/DifferentialEquations.jl/badge.svg?branch=master)](https://coveralls.io/github/JuliaDiffEq/DifferentialEquations.jl?branch=master)
[![codecov](https://codecov.io/gh/JuliaDiffEq/DifferentialEquations.jl/coverage.svg?branch=master)](https://codecov.io/gh/ChrisRackauckas/DifferentialEquations.jl)
[![](https://img.shields.io/badge/docs-stable-blue.svg)](https://JuliaDiffEq.github.io/DifferentialEquations.jl/stable)
[![](https://img.shields.io/badge/docs-latest-blue.svg)](https://JuliaDiffEq.github.io/DifferentialEquations.jl/latest)

This is a package for numerically solving differential equations in Julia by Chris Rackauckas. The purpose of this package is to supply efficient Julia implementations of solvers for various differential equations. Equations within the realm of this package include (but are not limited to):

- Ordinary differential equations (ODEs)
- Stochastic ordinary differential equations (SODEs or SDEs)
- (Stochastic) partial differential equations ((S)PDEs) (with both finite difference and finite element methods)
- Algebraic differential equations
- Differential delay equations.

It includes well-optimized implementations classic algorithms and ones from recent research, including algorithms optimized for high-precision and HPC applications. It integrates with the Julia package sphere, for example using Juno's progress meter, and wraps other differential equation solvers (ODE.jl, ODEInterface.jl, and Sundials.jl) so that many different methods for solving the equations can be accessed by simply switching a keyword argument.

For information on using the package, [see the documentation](http://chrisrackauckas.github.io/DifferentialEquations.jl/latest/).

All of the algorithms are thoroughly tested to ensure accuracy. Convergence tests are included in the [test](https://github.com/ChrisRackauckas/DifferentialEquations.jl/tree/master/test) folder. The algorithms were also tested to show correctness with nontrivial behavior such as Turing morphogenesis. Example IJulia notebooks
[can be found in the examples folder](https://github.com/ChrisRackauckas/DifferentialEquations.jl/tree/master/examples). If you find any equation where there seems
to be an error, please open an issue.

If you have any questions, or just want to chat about solvers/using the package, please feel free to message me in the [Gitter channel](https://gitter.im/ChrisRackauckas/DifferentialEquations.jl?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge). For bug reports, feature requests, etc., please submit an issue. For help installing conditional dependencies such as the ODE.jl wrappers, see the [Conditional Dependences manual page](http://chrisrackauckas.github.io/DifferentialEquations.jl/latest/man/conditional_dependencies/). If you're interested in contributing, please see the [Contributor's Guide](http://chrisrackauckas.github.io/DifferentialEquations.jl/latest/internals/contributors_guide/).

--------------------------------


<img src="https://raw.githubusercontent.com/ChrisRackauckas/DifferentialEquations.jl/master/examples/plots/DifferentialEquations_Example.png" align="middle"  />
