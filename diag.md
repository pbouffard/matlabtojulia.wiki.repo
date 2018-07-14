# `diag` Create diagonal matrix or get diagonal elements of matrix

[`diag`](https://docs.julialang.org/en/latest/stdlib/LinearAlgebra/#LinearAlgebra.diag) in Julia is basically identical:

```
julia> using LinearAlgebra

julia> M = [11 12 13; 21 22 23; 31 32 33]
3×3 Array{Int64,2}:
 11  12  13
 21  22  23
 31  32  33

julia> diag(M)
3-element Array{Int64,1}:
 11
 22
 33

julia> diag(M, 1)
2-element Array{Int64,1}:
 12
 23
```

***

Back to [Matrices and Arrays](https://github.com/pbouffard/matlabtojulia/wiki/Language-Fundamentals#matrices-and-arrays)