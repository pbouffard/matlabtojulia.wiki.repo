# MATLAB to Julia

You may want to just **Jump to the [[Index]]**.

***

The purpose of this wiki is to have a place to capture information that could be helpful for people interested in migrating code from MATLAB™ to Julia, and also those who are familiar with MATLAB and would like to learn Julia. It is meant to supplement existing resources, for instance the [differences](https://docs.julialang.org/en/latest/manual/noteworthy-differences/#Noteworthy-differences-from-MATLAB-1) page from the Julia documentation. However this wiki intends to be more comprehensive, and to be structured in such a way as to make it easy for one to find answers to questions like:

* For a given MATLAB or MATLAB toolbox command/function/construct what are the closest Julia equivalents?
* For a given MATLAB toolbox, what Julia packages provide similar functionality?

The organization mirrors that of the MATLAB product line; that is, the core MATLAB language features are together in the [[MATLAB]] section which if complete would map everything found in the core MATLAB [documentation](https://www.mathworks.com/help/matlab/index.html) to Julia equivalents, while another section on the [[Control System Toolbox]], for instance, would map functionality documented in its [toolbox documentation page](https://www.mathworks.com/help/control/index.html) to Julia equivalents.

Of course, implicitly one can use the content of the wiki to map concepts in the other direction but the focus is on migration from MATLAB to Julia.

## Versions
The most recent MATLAB documentation (currently R2018a) is implied as the 'source' of the mapping in functionality unless otherwise specified. Note that only the most recent MATLAB documentation is available on the MathWorks' website without a login; [previous releases' documentation](https://www.mathworks.com/help/doc-archives.html) requires a login.

In general when equivalent Julia 1.0 (i.e. [0.7 without deprecation warnings](https://discourse.julialang.org/t/what-is-julia-0-7-how-does-it-relate-to-1-0/9994)) functionality exists this is what will be linked to, but in cases where this does not exist but an earlier version, e.g. 0.6, has the functionality the latter will be linked to.

## Related Resources
* Julia documentation [noteworthy differences from MATLAB](https://docs.julialang.org/en/latest/manual/noteworthy-differences/#Noteworthy-differences-from-MATLAB-1)
* [MATLAB - Python - Julia Cheatsheet](https://cheatsheets.quantecon.org/)