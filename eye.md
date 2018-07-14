# `eye` Identity matrix

`eye` existed before Julia 0.7 but has been deprecated.

## In expressions
The identity operator `I` operator provides similar functionality for many use cases, e.g.:

```
julia> using LinearAlgebra

julia> x = ones(3,3)
3×3 Array{Float64,2}:
 1.0  1.0  1.0
 1.0  1.0  1.0
 1.0  1.0  1.0

julia> I*x
3×3 Array{Float64,2}:
 1.0  1.0  1.0
 1.0  1.0  1.0
 1.0  1.0  1.0
```

See [UniformScaling](https://docs.julialang.org/en/latest/stdlib/LinearAlgebra/#The-uniform-scaling-operator-1).

## Constructing identity matrices
For the purposes of constructing identity matrices, one can get something roughly equivalent to MATLAB `eye` by defining Julia macros:

```
julia> macro eye(); 1.0; end; macro eye(n); one(zeros(n,n)); end
@eye (macro with 2 methods)

julia> @eye
1.0

julia> @eye(5)
5×5 Array{Float64,2}:
 1.0  0.0  0.0  0.0  0.0
 0.0  1.0  0.0  0.0  0.0
 0.0  0.0  1.0  0.0  0.0
 0.0  0.0  0.0  1.0  0.0
 0.0  0.0  0.0  0.0  1.0
```
***

Back to [Matrices and Arrays](https://github.com/pbouffard/matlabtojulia/wiki/Language-Fundamentals#matrices-and-arrays)