# Benchmark Report

## Job Properties

*Commit(s):* [stevengj/julia@2dcbdf5272b469b7d36755e5c75abcc2ce8834d6](https://github.com/stevengj/julia/commit/2dcbdf5272b469b7d36755e5c75abcc2ce8834d6) vs [JuliaLang/julia@acafa9bc12746fb98e2764ce9618319e3db8799f](https://github.com/JuliaLang/julia/commit/acafa9bc12746fb98e2764ce9618319e3db8799f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/16305#issuecomment-218865319)

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
| `["array","comprehension",("comprehension_indexing","Array{Float64,1}")]` | 1.42 (30.00%) :x: | 1.00 (1.00%)  |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 1.46 (30.00%) :x: | 1.00 (1.00%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.37 (30.00%) :x: | 1.00 (1.00%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 1.86 (15.00%) :x: | 1.00 (1.00%)  |
| `["array","comprehension",("comprehension_iteration","FloatRange{Float64}")]` | 1.57 (15.00%) :x: | 1.00 (1.00%)  |
| `["array","comprehension",("comprehension_iteration","LinSpace{Float64}")]` | 1.45 (15.00%) :x: | 1.00 (1.00%)  |
| `["array","growth",("append!",2048)]` | 1.07 (15.00%)  | 0.99 (1.00%) :white_check_mark: |
| `["array","growth",("append!",256)]` | 1.60 (15.00%) :x: | 1.71 (1.00%) :x: |
| `["array","growth",("append!",8)]` | 1.45 (15.00%) :x: | 2.13 (1.00%) :x: |
| `["array","growth",("prerend!",2048)]` | 1.46 (15.00%) :x: | 0.98 (1.00%) :white_check_mark: |
| `["array","growth",("prerend!",256)]` | 1.45 (15.00%) :x: | 1.28 (1.00%) :x: |
| `["array","growth",("prerend!",8)]` | 1.58 (15.00%) :x: | 2.14 (1.00%) :x: |
| `["array","growth",("push_multiple!",2048)]` | 1.18 (15.00%) :x: | 1.88 (1.00%) :x: |
| `["array","growth",("push_multiple!",256)]` | 1.10 (15.00%)  | 1.04 (1.00%) :x: |
| `["array","growth",("push_multiple!",8)]` | 1.20 (15.00%) :x: | 2.13 (1.00%) :x: |
| `["array","growth",("push_single!",2048)]` | 1.03 (15.00%)  | 0.91 (1.00%) :white_check_mark: |
| `["array","growth",("push_single!",256)]` | 1.02 (15.00%)  | 0.98 (1.00%) :white_check_mark: |
| `["array","setindex!",("setindex!",1)]` | 1.02 (15.00%)  | 0.95 (1.00%) :white_check_mark: |
| `["array","setindex!",("setindex!",2)]` | 1.04 (15.00%)  | 0.95 (1.00%) :white_check_mark: |
| `["array","setindex!",("setindex!",3)]` | 1.00 (15.00%)  | 0.95 (1.00%) :white_check_mark: |
| `["array","setindex!",("setindex!",4)]` | 0.99 (15.00%)  | 0.95 (1.00%) :white_check_mark: |
| `["array","setindex!",("setindex!",5)]` | 1.00 (15.00%)  | 0.95 (1.00%) :white_check_mark: |
| `["parallel","remotecall",("identity",1024)]` | 1.01 (15.00%)  | 1.02 (1.00%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.02 (15.00%)  | 1.03 (1.00%) :x: |
| `["parallel","remotecall",("identity",4096)]` | 1.02 (15.00%)  | 1.02 (1.00%) :x: |
| `["parallel","remotecall",("identity",512)]` | 1.02 (15.00%)  | 1.03 (1.00%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.02 (15.00%)  | 1.03 (1.00%) :x: |
| `["problem","json","parse_json"]` | 0.99 (15.00%)  | 0.97 (1.00%) :white_check_mark: |
| `["problem","spellcheck"]` | 1.13 (15.00%)  | 1.02 (1.00%) :x: |
| `["sort","issorted",("forwards","ascending")]` | 0.83 (15.00%) :white_check_mark: | 1.00 (1.00%)  |
| `["sort","issorted",("forwards","random")]` | 0.85 (15.00%) :white_check_mark: | 1.00 (1.00%)  |
| `["sparse","index",("spmat","integer",100)]` | 0.73 (25.00%) :white_check_mark: | 1.00 (1.00%)  |
| `["sparse","index",("spmat","row","array",100)]` | 0.96 (15.00%)  | 1.09 (1.00%) :x: |
| `["sparse","index",("spmat","row","array",1000)]` | 1.05 (15.00%)  | 1.70 (1.00%) :x: |
| `["sparse","index",("spmat","row","logical",1000)]` | 1.03 (15.00%)  | 1.08 (1.00%) :x: |
| `["sparse","index",("spmat","row","range",100)]` | 1.02 (15.00%)  | 1.29 (1.00%) :x: |
| `["sparse","index",("spmat","row","range",1000)]` | 1.02 (15.00%)  | 1.14 (1.00%) :x: |
| `["string","join"]` | 1.08 (15.00%)  | 1.01 (1.00%) :x: |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 1.62 (40.00%) :x: | 1.00 (1.00%)  |

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
Julia Version 0.5.0-dev+4069
Commit 2dcbdf5 (2016-05-12 18:00 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (22106.08203125 MB free)
Uptime: 615640.0 sec
Load Avg:  0.9228515625  0.998046875  0.94921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1070356 s          0 s     177773 s   60179241 s          2 s
#2  3501 MHz    1950019 s          0 s     137114 s   59412364 s          0 s
#3  3501 MHz     911174 s          0 s     114740 s   60505783 s          0 s
#4  3501 MHz     703126 s          0 s     108556 s   60718679 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+4066
Commit acafa9b (2016-05-12 17:59 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (22076.07421875 MB free)
Uptime: 620268.0 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    1161370 s          0 s     186378 s   60541074 s          2 s
#2  3501 MHz    2188091 s          0 s     145339 s   59628323 s          0 s
#3  3501 MHz     968148 s          0 s     121404 s   60904104 s          0 s
#4  3501 MHz     750287 s          0 s     114554 s   61127733 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
