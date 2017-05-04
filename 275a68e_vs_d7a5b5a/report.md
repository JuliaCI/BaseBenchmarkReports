# Benchmark Report

## Job Properties

*Commit(s):* [fredrikekre/julia@275a68e00c3d74019ef31d38a88f918ff9c88f08](https://github.com/fredrikekre/julia/commit/275a68e00c3d74019ef31d38a88f918ff9c88f08) vs [JuliaLang/julia@d7a5b5acffbe52f8221fd06b94908074abac5586](https://github.com/JuliaLang/julia/commit/d7a5b5acffbe52f8221fd06b94908074abac5586)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21688#issuecomment-299154523)

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
| `["array","bool","boolarray_true_load!"]` | 1.44 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.66 (50%) :x: | 1.00 (1%)  |
| `["io","read","read"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Matrix",1024)]` | 0.51 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Matrix",256)]` | 0.44 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",1024)]` | 0.51 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 0.44 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("schur","Matrix",1024)]` | 0.47 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("schur","Matrix",256)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",1024)]` | 0.48 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",256)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["problem","spellcheck","spellcheck"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["scalar","intfuncs"]`
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
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.23
Commit 275a68e (2017-05-04 11:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9096.15234375 MB free)
Uptime: 2.9546894e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   60900090 s          0 s    9400813 s  2878072409 s         85 s
#2  3501 MHz  231040783 s          0 s   10383431 s  2707785190 s         35 s
#3  3501 MHz   51788819 s          0 s    6031386 s  2895544722 s         45 s
#4  3501 MHz   47315382 s          0 s    5972455 s  2900354743 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.21
Commit d7a5b5a (2017-05-04 04:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8759.80859375 MB free)
Uptime: 2.9552511e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   60984717 s          0 s    9411076 s  2878536948 s         85 s
#2  3501 MHz  231549006 s          0 s   10392750 s  2707828791 s         35 s
#3  3501 MHz   51879061 s          0 s    6040386 s  2896006512 s         45 s
#4  3501 MHz   47401386 s          0 s    5981102 s  2900821219 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
