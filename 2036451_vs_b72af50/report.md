# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@20364516cf1c2dd986c86a8f9cd13c082e90a075](https://github.com/JuliaLang/julia/commit/20364516cf1c2dd986c86a8f9cd13c082e90a075) vs [JuliaLang/julia@b72af507df65c73b16766b8799f7e7ce70cd39bf](https://github.com/JuliaLang/julia/commit/b72af507df65c73b16766b8799f7e7ce70cd39bf)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23914)

*Tag Predicate:* `ALL`

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
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","sparse",((10000000,),2)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",5)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["dates","string","DateTime"]` | 1.22 (15%) :x: | 1.11 (1%) :x: |
| `["io","read","readstring"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io","serialization",("serialize","Vector{String}")]` | 1.12 (15%)  | 1.10 (1%) :x: |
| `["problem","laplacian","laplace_iter_vec"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.00 (25%)  | 0.99 (1%) :white_check_mark: |
| `["shootout","k_nucleotide"]` | 1.06 (15%)  | 1.11 (1%) :x: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["shootout","regex_dna"]` | 1.05 (15%)  | 1.06 (1%) :x: |
| `["string","join"]` | 1.69 (40%) :x: | 1.00 (1%)  |
| `["string","replace"]` | 1.29 (15%) :x: | 1.24 (1%) :x: |

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
Julia Version 0.7.0-DEV.1983
Commit 2036451 (2017-09-28 02:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   87033668 s          0 s   13556214 s  4111968415 s        171 s
       #2  3501 MHz  348977459 s          0 s   14457634 s  3851183147 s         58 s
       #3  3501 MHz   72683810 s          0 s    8311303 s  4139205289 s         79 s
       #4  3501 MHz   68024529 s          0 s    8198150 s  4144374690 s         28 s
       
  Memory: 31.383651733398438 GB (3232.34375 MB free)
  Uptime: 4.2220108e7 sec
  Load Avg:  1.0830078125  1.03125  1.05078125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1981
Commit b72af50 (2017-09-27 21:29 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   87132095 s          0 s   13566313 s  4112589449 s        172 s
       #2  3501 MHz  349647186 s          0 s   14469264 s  3851233469 s         58 s
       #3  3501 MHz   72767618 s          0 s    8319244 s  4139844944 s         80 s
       #4  3501 MHz   68103562 s          0 s    8205810 s  4145019739 s         28 s
       
  Memory: 31.383651733398438 GB (3001.34765625 MB free)
  Uptime: 4.2227433e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
