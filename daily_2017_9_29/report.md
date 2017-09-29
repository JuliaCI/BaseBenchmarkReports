# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@378e07803bf60e592dfed1957c38104489e5cb59](https://github.com/JuliaLang/julia/commit/378e07803bf60e592dfed1957c38104489e5cb59)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/378e07803bf60e592dfed1957c38104489e5cb59#commitcomment-24643921)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-09-29 vs 2017-09-28

## Results

*Note: If Chrome is your browser, I strongly recommend installing the [Wide GitHub](https://chrome.google.com/webstore/detail/wide-github/kaalofacklcidaampbokdplbklpeldpj?hl=en)
extension, which makes the result table easier to read.*

Below is a table of this job's results, obtained by running the benchmarks found in
[JuliaCI/BaseBenchmarks.jl](https://github.com/JuliaCI/BaseBenchmarks.jl). The values
listed in the `ID` column have the structure `[parent_group, child_group, ..., key]`,
and can be used to index into the BaseBenchmarks suite to retrieve the corresponding
benchmarks.

The percentages accompanying time and memory values in the below table are noise tolerances. The "true"
time/memory value for a given benchmark is expected to fall within this percentage of the reported value.

A ratio greater than `1.0` denotes a possible regression (marked with :x:), while a ratio less
than `1.0` denotes a possible improvement (marked with :white_check_mark:). Only significant results - results
that indicate possible regressions or improvements - are shown below (thus, an empty table means that all
benchmark results remained invariant between builds).

| ID | time ratio | memory ratio |
|----|------------|--------------|
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),2)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["dates","string","DateTime"]` | 1.21 (15%) :x: | 1.11 (1%) :x: |
| `["io","serialization",("serialize","Vector{String}")]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","negative argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","positive argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 1.07 (15%)  | 1.11 (1%) :x: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["shootout","regex_dna"]` | 1.06 (15%)  | 1.06 (1%) :x: |
| `["sparse","constructors",("Diagonal",100)]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["string","readuntil","backtracking"]` | 0.00 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["string","readuntil","barbarian backtrack"]` | 0.01 (15%) :white_check_mark: | 0.04 (1%) :white_check_mark: |
| `["string","readuntil","no backtracking"]` | 0.01 (15%) :white_check_mark: | 0.05 (1%) :white_check_mark: |
| `["string","readuntil","target length 1"]` | 0.18 (15%) :white_check_mark: | 0.31 (1%) :white_check_mark: |
| `["string","readuntil","target length 1000"]` | 0.10 (15%) :white_check_mark: | 0.12 (1%) :white_check_mark: |
| `["string","readuntil","target length 2"]` | 0.26 (15%) :white_check_mark: | 0.38 (1%) :white_check_mark: |
| `["string","readuntil","target length 50000"]` | 0.12 (15%) :white_check_mark: | 0.03 (1%) :white_check_mark: |
| `["string","replace"]` | 1.25 (15%) :x: | 1.24 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","convert"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reductions"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["broadcast","dotop"]`
- `["broadcast","fusion"]`
- `["broadcast","mix_scalar_tuple"]`
- `["broadcast","sparse"]`
- `["broadcast","typeargs"]`
- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["misc","afoldl"]`
- `["misc","bitshift"]`
- `["misc","julia"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
- `["parallel","remotecall"]`
- `["problem","chaosgame"]`
- `["problem","fem"]`
- `["problem","go"]`
- `["problem","grigoriadis khachiyan"]`
- `["problem","imdb"]`
- `["problem","json"]`
- `["problem","laplacian"]`
- `["problem","monte carlo"]`
- `["problem","raytrace"]`
- `["problem","seismic"]`
- `["problem","simplex"]`
- `["problem","spellcheck"]`
- `["problem","stockcorr"]`
- `["problem","ziggurat"]`
- `["random","collections"]`
- `["random","randstring"]`
- `["random","ranges"]`
- `["random","sequences"]`
- `["random","types"]`
- `["scalar","acos"]`
- `["scalar","arithmetic"]`
- `["scalar","asin"]`
- `["scalar","atan"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
- `["scalar","tan"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","constructors"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["string","readuntil"]`
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1995
Commit 378e078 (2017-09-29 03:31 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   95447718 s          0 s   16937961 s  4106126139 s         93 s
       #2  3501 MHz  409590172 s          0 s   10926683 s  3807959502 s         20 s
       #3  3501 MHz   82661289 s          0 s    9388915 s  4136840569 s         77 s
       #4  3501 MHz   79007612 s          0 s    9578127 s  4140310365 s         18 s
       
  Memory: 31.383651733398438 GB (3091.98828125 MB free)
  Uptime: 4.2309205e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
