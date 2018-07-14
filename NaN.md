# `NaN` Not-a-Number

Basically identical in Julia, other than that Julia doesn't have the lowercase `nan` built-in, but of course you can just create it:

```
julia> nan
ERROR: UndefVarError: nan not defined

julia> nan = NaN
NaN

julia> nan
NaN
```

***

Back to [Numeric Types](https://github.com/pbouffard/matlabtojulia/wiki/Language-Fundamentals#numeric-types)