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
In general the intent is to capture the information itself in this wiki, for the same reasons as this is [encouraged on StackOverflow](https://stackoverflow.com/help/how-to-answer):

> **Provide context for links**
>
> Links to external resources are encouraged, but please add context around the link so your fellow users will have some idea what it is and why it’s there. Always quote the most relevant part of an important link, in case the target site is unreachable or goes permanently offline.

As such, it is assumed that the main [Julia documentation](https://docs.julialang.org) isn't at risk of going offline, but the salient points from other sources should in general be included in this wiki so it is largely self-contained (and thus is itself suitable for offline use). Of course, attribution by means of links to sources of information is highly encouraged.

That said, much of what's in this wiki is taken from the following resources:

* Julia documentation [noteworthy differences from MATLAB](https://docs.julialang.org/en/latest/manual/noteworthy-differences/#Noteworthy-differences-from-MATLAB-1)
* Julia [package index](https://pkg.julialang.org/)
* QuantEcon [MATLAB - Python - Julia Cheatsheet](https://cheatsheets.quantecon.org/)

## Searching
You can [search GitHub wikis](https://blog.github.com/2016-08-08-search-wiki-pages/) by using the main GitHub search bar and specifying the repo, e.g.:

`repo:pbouffard/matlabtojulia clc`

In the search results page, click the Wikis link to display search hits from the wiki.

## Contributing
Contributions are encouraged! The repo settings have the "Restrict editing to collaborators only" option turned off so that it should be possible to simply edit the wiki, though GitHub requires you to be [signed in](https://github.com/login?return_to=%2Fpbouffard%2Fmatlabtojulia%2Fwiki) so that anonymous edits are not possible. 

Please include an edit message in cases where the explanation of the change isn't obvious.

Unfortunately GitHub [doesn't support](https://github.com/gollum/gollum/issues/265) pull requests into wikis so PRs for bulk (or any) edits are not possible, however a suggested workflow if you have a bulk edit to contribute is to submit an [issue](https://github.com/pbouffard/matlabtojulia/issues) where the best way to bring in such an edit can be discussed.

## License
Creative Commons Attribution-ShareAlike 4.0 International Public License.

See [LICENSE.md](https://github.com/pbouffard/matlabtojulia/blob/master/LICENSE.md).