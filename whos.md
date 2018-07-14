In Julia [`varinfo()`](https://docs.julialang.org/en/latest/stdlib/InteractiveUtils/#InteractiveUtils.varinfo) is roughly comparable to `whos` in MATLAB:

**Julia**
```
julia> x = 2

julia> varinfo()
name                    size summary        
–––––––––––––––– ––––––––––– –––––––––––––––
Base                         Module         
Core                         Module         
InteractiveUtils 180.140 KiB Module         
Main                         Module         
ans                  0 bytes typeof(varinfo)
x                    8 bytes Int64    
```

**MATLAB**
```
>> whos
  Name      Size            Bytes  Class     Attributes

  x         1x1                 8  double         
```