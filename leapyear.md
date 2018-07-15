# [`leapyear`](https://www.mathworks.com/help/aerotbx/ug/leapyear.html) Determine leap year

In Julia [`Dates.isleapyear`](https://docs.julialang.org/en/latest/stdlib/Dates/#Query-Functions-1) is basically identical:

```
julia> using Dates

julia> isleapyear(2018)
false

julia> isleapyear.([2005 2012])
1×2 BitArray{2}:
 false  true
```