# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e8efdfd03fbab70387ff51c1cfedb19f4d217ff8](https://github.com/JuliaLang/julia/commit/e8efdfd03fbab70387ff51c1cfedb19f4d217ff8) vs [JuliaLang/julia@3704eac25df42f2bb0433669fc0aaeb2f57cb73e](https://github.com/JuliaLang/julia/commit/3704eac25df42f2bb0433669fc0aaeb2f57cb73e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/17137#issuecomment-231158603)

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
| `["array","bool","bitarray_bool_load!"]` | 1.66 (15%) :x: | 1.00 (1%)  |
| `["array","bool","bitarray_true_load!"]` | 1.51 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["array","growth",("prerend!",8)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt","100000000:-1:1")]` | 1.41 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:1.0e8")]` | 0.54 (40%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 0.47 (40%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 0.25 (30%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 0.19 (30%) :white_check_mark: | 0.83 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 0.26 (30%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.19 (30%) :white_check_mark: | 0.83 (1%) :white_check_mark: |
| `["scalar","predicate",("iseven","BigInt")]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","BigFloat")]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isodd","BigInt")]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 1.22 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 1.01 (15%)  | 1.01 (1%) :x: |

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
Julia Version 0.5.0-dev+5217
Commit e8efdfd (2016-07-07 17:58 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (21041.57421875 MB free)
Uptime: 3.564328e6 sec
Load Avg:  1.01123046875  1.0146484375  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    4381217 s          0 s    1039811 s  350066915 s         13 s
#2  3501 MHz   12113718 s          0 s     648148 s  343458116 s          2 s
#3  3501 MHz    4374459 s          0 s     577842 s  351309883 s          4 s
#4  3501 MHz    3848726 s          0 s     591160 s  351803168 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.5.0-dev+5202
Commit 3704eac (2016-07-07 16:50 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20926.78515625 MB free)
Uptime: 3.568878e6 sec
Load Avg:  0.9970703125  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    4441533 s          0 s    1045492 s  350454522 s         13 s
#2  3501 MHz   12310663 s          0 s     655304 s  343708520 s          2 s
#3  3501 MHz    4422330 s          0 s     584544 s  351709535 s          4 s
#4  3501 MHz    3969544 s          0 s     600686 s  352127328 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
