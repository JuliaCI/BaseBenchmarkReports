# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0b39a43d29a1c282a6e96fbb04dfffc02d2ad59e](https://github.com/JuliaLang/julia/commit/0b39a43d29a1c282a6e96fbb04dfffc02d2ad59e) vs [JuliaLang/julia@f73e6e126b1d48a0968694ee2f972270dbf2292a](https://github.com/JuliaLang/julia/commit/f73e6e126b1d48a0968694ee2f972270dbf2292a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18040#issuecomment-239967601)

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
| `["array","cat",("hcat",500)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.63 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("prerend!",2048)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.38 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.56 (25%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 1.48 (25%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","random")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.76 (40%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.234
Commit 0b39a43 (2016-08-15 23:34 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20542.96484375 MB free)
Uptime: 6.956616e6 sec
Load Avg:  1.0029296875  1.001953125  0.955078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   11123676 s          0 s    2022890 s  680914627 s         22 s
#2  3501 MHz   25182276 s          0 s    1630886 s  668112910 s          5 s
#3  3501 MHz    8788133 s          0 s    1168418 s  685340616 s         12 s
#4  3501 MHz    6641911 s          0 s    1132497 s  687578057 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.231
Commit f73e6e1 (2016-08-15 23:34 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20387.38671875 MB free)
Uptime: 6.961507e6 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   11167841 s          0 s    2030072 s  681350957 s         22 s
#2  3501 MHz   25395760 s          0 s    1641588 s  668377110 s          5 s
#3  3501 MHz    8930732 s          0 s    1178921 s  685675913 s         12 s
#4  3501 MHz    6696386 s          0 s    1138752 s  688005844 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
