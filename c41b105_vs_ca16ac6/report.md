# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@c41b10537fa100eb45638493006f1e898edca70e](https://github.com/pabloferz/julia/commit/c41b10537fa100eb45638493006f1e898edca70e) vs [JuliaLang/julia@ca16ac6550e5a6b6ba1a8fdeb9c813d360469638](https://github.com/JuliaLang/julia/commit/ca16ac6550e5a6b6ba1a8fdeb9c813d360469638)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18642#issuecomment-249359634)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.55 (15%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 2.29 (30%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 2.14 (30%) :x: | 1.04 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 1.48 (30%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 2.02 (30%) :x: | 1.04 (1%) :x: |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.94 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.43 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",10)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 0.70 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","range",1000)]` | 0.51 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.49 (40%) :x: | 1.00 (1%)  |

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
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
- `["parallel","remotecall"]`
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
Julia Version 0.6.0-dev.759
Commit c41b105 (2016-09-24 09:31 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16888.9375 MB free)
Uptime: 1.0366066e7 sec
Load Avg:  1.0029296875  1.0146484375  0.96533203125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16574793 s          0 s    2836186 s  1015000863 s         32 s
#2  3501 MHz   40709573 s          0 s    2972718 s  991497135 s          9 s
#3  3501 MHz   14254794 s          0 s    1843030 s  1020001263 s         16 s
#4  3501 MHz   11923774 s          0 s    1795628 s  1022471367 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.756
Commit ca16ac6 (2016-09-24 01:14 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (16537.15625 MB free)
Uptime: 1.0371086e7 sec
Load Avg:  1.0029296875  1.0146484375  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   16618844 s          0 s    2842946 s  1015450551 s         32 s
#2  3501 MHz   40950019 s          0 s    2985385 s  991745221 s          9 s
#3  3501 MHz   14309811 s          0 s    1849776 s  1020440704 s         16 s
#4  3501 MHz   12051066 s          0 s    1805477 s  1022835772 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
