# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@91bb175567f1c805b8decb966ed20e779ac80ce1](https://github.com/JuliaLang/julia/commit/91bb175567f1c805b8decb966ed20e779ac80ce1) vs [JuliaLang/julia@f46ed5f4967853bf90b177cbf896ec69af6b8265](https://github.com/JuliaLang/julia/commit/f46ed5f4967853bf90b177cbf896ec69af6b8265)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17228#issuecomment-231128174)

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
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 1.40 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 0.46 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",4)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",5)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_sub"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["shootout","revcomp"]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","ascending")]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["sort","issorted",("forwards","descending")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","range",10000)]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["io","read"]`
- `["io"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["parallel","remotecall"]`
- `["problem","fem"]`
- `["problem","go"]`
- `["problem","grigoriadis khachiyan"]`
- `["problem","imdb"]`
- `["problem","json"]`
- `["problem","laplacian"]`
- `["problem","monte carlo"]`
- `["problem"]`
- `["problem","seismic"]`
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+5196
Commit 91bb175 (2016-07-07 16:11 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (21193.62109375 MB free)
Uptime: 3.557757e6 sec
Load Avg:  1.0029296875  1.0146484375  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    3766711 s          0 s     829752 s  350383794 s         12 s
#2  3501 MHz   10206275 s          0 s     718584 s  344527295 s          4 s
#3  3501 MHz    3864468 s          0 s     564933 s  351140773 s          3 s
#4  3501 MHz    2652540 s          0 s     533955 s  352413489 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+5192
Commit f46ed5f (2016-07-07 15:36 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (21027.41015625 MB free)
Uptime: 3.56229e6 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    3885224 s          0 s     839458 s  350707710 s         12 s
#2  3501 MHz   10424438 s          0 s     725568 s  344754939 s          4 s
#3  3501 MHz    3907771 s          0 s     571078 s  351543851 s          3 s
#4  3501 MHz    2696959 s          0 s     540149 s  352815692 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
