# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c55feaa19498ee9fa524154989ee3ca547a6afe5](https://github.com/JuliaLang/julia/commit/c55feaa19498ee9fa524154989ee3ca547a6afe5) vs [JuliaLang/julia@80369bf7b49959d28837e764b41621456ae0e32e](https://github.com/JuliaLang/julia/commit/80369bf7b49959d28837e764b41621456ae0e32e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22208#issuecomment-306545782)

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
| `["array","comprehension",("collect","Array{Float64,1}")]` | 0.44 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.64 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","StepRangeLen{Float64,Base.TwicePrecision{Float64},Base.TwicePrecision{Float64}}")]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 1.15 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 1.83 (45%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 1.49 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",1024)]` | 1.61 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",256)]` | 1.97 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Matrix","Matrix",1024)]` | 1.58 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Matrix","Matrix",256)]` | 1.96 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 1.76 (45%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 1.48 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 1.64 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 1.27 (45%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",1024)]` | 1.60 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",256)]` | 1.96 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 1.92 (45%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 1.47 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 1.15 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 1.88 (45%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 1.51 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",1024)]` | 1.61 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",256)]` | 1.97 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Matrix","Matrix",1024)]` | 1.56 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Matrix","Matrix",256)]` | 2.00 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 1.76 (45%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 1.46 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 1.62 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 1.26 (45%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",1024)]` | 1.59 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",256)]` | 1.96 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 1.91 (45%) :x: | 1.01 (1%)  |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 1.46 (45%) :x: | 1.02 (1%) :x: |
| `["sparse","transpose",("transpose",(20000,20000))]` | 0.70 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 1.43 (40%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(2,))]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.486
Commit c55feaa (2017-06-06 14:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   68237853 s          0 s   12749706 s  3151435192 s         82 s
       #2  3501 MHz  284383586 s          0 s    8062366 s  2947519439 s         12 s
       #3  3501 MHz   61466882 s          0 s    7184762 s  3171649275 s         65 s
       #4  3501 MHz   58444031 s          0 s    7347478 s  3174504189 s         15 s
       
  Memory: 31.383651733398438 GB (2757.94921875 MB free)
  Uptime: 3.2418714e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.484
Commit 80369bf (2017-06-06 13:51 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   68334397 s          0 s   12759258 s  3151856120 s         82 s
       #2  3501 MHz  284856016 s          0 s    8071296 s  2947566424 s         12 s
       #3  3501 MHz   61548127 s          0 s    7193060 s  3172088063 s         65 s
       #4  3501 MHz   58529750 s          0 s    7355564 s  3174938874 s         15 s
       
  Memory: 31.383651733398438 GB (2717.12109375 MB free)
  Uptime: 3.2424003e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
