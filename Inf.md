# `Inf` Infinity

Basically identical in Julia, other than that Julia doesn't have the lowercase `inf` built-in, but of course you can just create it:

```
julia> inf
ERROR: UndefVarError: inf not defined

julia> inf = Inf
Inf

julia> inf
Inf
```

***

Back to [Numeric Types](https://github.com/pbouffard/matlabtojulia/wiki/Language-Fundamentals#numeric-types)