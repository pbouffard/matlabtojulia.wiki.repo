# `eye` Identity matrix

`eye` existed before Julia 0.7 but has been deprecated. You can get something roughly equivalent by defining Julia macros, however:

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