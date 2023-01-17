## Further sieving on "one equation to rule them all"
This code is an attempt to extend the computations presented in [48 MORE SOLUTIONS OF MARTIN DAVIS'S QUATERNARY QUARTIC EQUATION](https://www.jstor.org/stable/2153381). Using the [cado-nfs](https://gitlab.inria.fr/cado-nfs/cado-nfs) implementation of the [general number field sieve](https://en.wikipedia.org/wiki/General_number_field_sieve), I found that $A_{168}$ [factors](http://factordb.com/index.php?query=9528778331546509263788136187634193963092971274019101645251866033831985993967119289412141445999804608015425212446569171105752571905679068407670323075626717053055517302730715294912767547558222369434104641) as a product including two primes equivalent to $5 \pmod 7$. By computing the recurrence relation mod every prime less than $10^9$ and using [primefac](https://pypi.org/project/primefac/)'s interface for the probabilistic [elliptic-curve factorization method](https://en.wikipedia.org/wiki/Lenstra_elliptic-curve_factorization), all but $285$ of the remaining possibilities under $10000$ were eliminated, with only $\{320,495,530,543,761,831,938\}$ less than $1000$. Some interesting remaining numbers to look at are $1118$ and $3981$, since $A_{1118}$ and $B_{3981}$ are both prime. In addition, $(53^2-1)/2=1404$ is the smallest composite number which has not been eliminated ( $A_{26}|A_{1404}$ and $1214504828571031609765841B_{26}|B_{1404}$ is all that has been found ).
