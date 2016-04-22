# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1f76eda7deee46933911e3bef165639e8fb8a695](https://github.com/JuliaLang/julia/commit/1f76eda7deee46933911e3bef165639e8fb8a695) vs [JuliaLang/julia@5c9b7a62fe10eabe193ab1d5bd4addbadf838cef](https://github.com/JuliaLang/julia/commit/5c9b7a62fe10eabe193ab1d5bd4addbadf838cef)

*Tag Predicate:* `ALL`

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/15997)

## Results

Below is a table of this job's results. If available, the data used to generate this
table can be found in the JLD file in this directory.

Benchmark definitions can be found in [JuliaCI/BaseBenchmarks.jl](https://github.com/JuliaCI/BaseBenchmarks.jl).

The ratio values in the below table equal `primary_result / comparison_result` for each corresponding
metric. Thus, `x < 1.0` would denote an improvement, while `x > 1.0` would denote a regression.
Note that a default tolerance of `0.20` is applied to account for the variance of our test
hardware.

Regressions are marked with :x:, while improvements are marked with :white_check_mark:. GC
measurements are not considered when determining regression status.

Only benchmarks with significant results - results that indicate regressions or improvements - are
shown below (an empty table means that all benchmark results remained invariant between builds).

| Group ID | Benchmark ID | time | GC time | memory allocated | number of allocations |
|----------|--------------|------|---------|------------------|-----------------------|
| `"blas"` | `("gbmv",1024)` | **0.73** :white_check_mark: | 1.46 | 1.00 | 1.00 |
| `"blas"` | `("gbmv!",1024)` | **0.71** :white_check_mark: | 1.00 | 1.00 | 1.00 |
| `"shootout mandelbrot"` | `"mandelbrot"` | 0.99 | 1.00 | 0.91 | **0.78** :white_check_mark: |
| `"simd"` | `("sum_reduce","Int64",999)` | **0.77** :white_check_mark: | 1.00 | 1.00 | 1.00 |
| `"sort insertionsort"` | `("sort reverse","insertionsort","random")` | 1.00 | 1.00 | 1.01 | **4.27** :x: |
| `"sort insertionsort"` | `("sort!","insertionsort","random")` | 1.00 | 1.00 | 1.08 | **135.00** :x: |
| `"sort mergesort"` | `("sort reverse","mergesort","random")` | 1.00 | 0.54 | 1.00 | **1.56** :x: |
| `"sort sortperm insertionsort"` | `("sortperm!","insertionsort","descending")` | 1.00 | 1.00 | 1.09 | **135.00** :x: |
| `"tuple indexing"` | `("sumelt","NTuple",30,Float64)` | **0.57** :white_check_mark: | 1.00 | 1.00 | 1.00 |

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+3693
Commit 1f76eda (2016-04-22 06:41 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-65-generic #105-Ubuntu SMP Mon Sep 21 18:50:58 UTC 2015 x86_64 x86_64
Memory: 31.383678436279297 GB (22495.08203125 MB free)
Uptime: 1.7704074e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    9902044 s       3496 s    7541754 s  1746395591 s         20 s
#2  3501 MHz   15232356 s        245 s    3765553 s  1749549229 s          4 s
#3  3501 MHz   12083823 s       1347 s    3881758 s  1753021725 s          2 s
#4  3501 MHz   10607697 s        303 s    3647624 s  1754990640 s          2 s
#5  3501 MHz   13347301 s       4215 s    3456030 s  1753129336 s          0 s
#6  3501 MHz    7134191 s       1198 s    3143346 s  1759728809 s          0 s
#7  3501 MHz    9287425 s       2155 s    3384174 s  1757289249 s          0 s
#8  3501 MHz    6808856 s       1400 s    3327234 s  1759909413 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+3691
Commit 5c9b7a6 (2016-04-22 04:35 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-65-generic #105-Ubuntu SMP Mon Sep 21 18:50:58 UTC 2015 x86_64 x86_64
Memory: 31.383678436279297 GB (22488.95703125 MB free)
Uptime: 1.7729628e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    9903689 s       3496 s    7550888 s  1748927173 s         21 s
#2  3501 MHz   15957410 s        245 s    3775988 s  1751343300 s          4 s
#3  3501 MHz   12971057 s       1347 s    3892836 s  1754658361 s          2 s
#4  3501 MHz   10689880 s        303 s    3655441 s  1757437311 s          2 s
#5  3501 MHz   14247492 s       4215 s    3474180 s  1754751060 s          0 s
#6  3501 MHz    7185289 s       1198 s    3150807 s  1762212968 s          0 s
#7  3501 MHz    9338672 s       2155 s    3391318 s  1759777132 s          0 s
#8  3501 MHz    6860522 s       1400 s    3334912 s  1762396133 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `"array bool"`
- `"array cat"`
- `"array comprehension"`
- `"array growth"`
- `"array index load reverse"`
- `"array index setindex!"`
- `"array index sum"`
- `"array subarray"`
- `"blas"`
- `"factorization"`
- `"iobuffer read"`
- `"linalg arithmetic"`
- `"micro"`
- `"problem go game"`
- `"problem grigoriadis khachiyan"`
- `"problem imdb graphs"`
- `"problem json parse"`
- `"problem laplacian"`
- `"problem monte carlo"`
- `"problem raytrace"`
- `"problem seismic simulation"`
- `"problem simplex"`
- `"problem sparse fem"`
- `"problem spellcheck"`
- `"problem stockcorr"`
- `"problem ziggurat"`
- `"scalar arithmetic"`
- `"scalar predicate"`
- `"shootout binary_trees"`
- `"shootout fannkuch"`
- `"shootout fasta"`
- `"shootout k_nucleotide"`
- `"shootout mandelbrot"`
- `"shootout meteor_contest"`
- `"shootout nbody_vec"`
- `"shootout pidigits"`
- `"shootout regex_dna"`
- `"shootout revcomp"`
- `"shootout spectralnorm"`
- `"simd"`
- `"sort insertionsort"`
- `"sort issorted"`
- `"sort mergesort"`
- `"sort quicksort"`
- `"sort sortperm insertionsort"`
- `"sort sortperm mergesort"`
- `"sort sortperm quicksort"`
- `"sparse matrix column indexing"`
- `"sparse matrix row + column indexing"`
- `"sparse matrix row indexing"`
- `"sparse matrix transpose"`
- `"sparse vector indexing"`
- `"string replace"`
- `"tuple indexing"`
