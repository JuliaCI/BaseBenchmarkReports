# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@4cf580dba7c1013e32f7d6904ae034207248138a](https://github.com/JuliaLang/julia/commit/4cf580dba7c1013e32f7d6904ae034207248138a) vs [JuliaLang/julia@13b22540b7b85cc29e62f15bbad7c2b29a82afeb](https://github.com/JuliaLang/julia/commit/13b22540b7b85cc29e62f15bbad7c2b29a82afeb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19259#issuecomment-270123448)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.73 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1.0:1.0:100000.0")]` | 0.79 (50%)  | 0.87 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","100000:-1:1")]` | 0.90 (50%)  | 0.89 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","1:100000")]` | 0.80 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Float32,2}")]` | 0.76 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Float64,3}")]` | 0.77 (50%)  | 0.82 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","Array{Int32,2}")]` | 0.89 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.77 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.76 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.79 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.88 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.88 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.77 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BitArray{2}")]` | 0.78 (50%)  | 0.77 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","linspace(1.0,2.0,10000)")]` | 0.81 (50%)  | 0.87 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","1.0:1.0:100000.0")]` | 0.30 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.91 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.93 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.77 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.75 (50%)  | 0.75 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BitArray{2}")]` | 0.79 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","linspace(1.0,2.0,10000)")]` | 2.71 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:1.0:100000.0")]` | 0.30 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 0.89 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","linspace(1.0,2.0,10000)")]` | 2.71 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","Array{Int32,2}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 1.52 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 1.52 (45%) :x: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 1.67 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",100)]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","range",10)]` | 0.64 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 1.95 (40%) :x: | 1.00 (1%)  |

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
- `["broadcast","sparse"]`
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
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
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
- `["scalar","floatexp"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1859
Commit 4cf580d (2017-01-03 12:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5272.83984375 MB free)
Uptime: 1.910637e7 sec
Load Avg:  1.0029296875  1.0146484375  0.970703125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   27202893 s          0 s    6263773 s  1871706606 s         60 s
#2  3501 MHz   88750438 s          0 s    3857786 s  1816890682 s          8 s
#3  3501 MHz   25731697 s          0 s    3316511 s  1880700238 s         40 s
#4  3501 MHz   23576467 s          0 s    3421742 s  1882735712 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1854
Commit 13b2254 (2017-01-03 12:45 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5635.1953125 MB free)
Uptime: 1.9114883e7 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   27265787 s          0 s    6273046 s  1872482961 s         60 s
#2  3501 MHz   89356162 s          0 s    3871871 s  1817121672 s          8 s
#3  3501 MHz   25838557 s          0 s    3325718 s  1881434704 s         40 s
#4  3501 MHz   23615395 s          0 s    3427914 s  1883541270 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
