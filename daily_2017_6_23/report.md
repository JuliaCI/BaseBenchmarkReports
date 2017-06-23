# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@02804aceefe1109a7392fcf2e1fe4a861f60edce](https://github.com/JuliaLang/julia/commit/02804aceefe1109a7392fcf2e1fe4a861f60edce)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/02804aceefe1109a7392fcf2e1fe4a861f60edce#commitcomment-22717289)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-06-23 vs 2017-06-22

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
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 2.42 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 2.40 (45%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4096)]` | 0.78 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.66 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","linear algebra",("matvec",(2,2),(2,))]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(2,))]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.679
Commit 02804ac (2017-06-23 01:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   70865538 s          0 s   13235397 s  3290154836 s         82 s
       #2  3501 MHz  296938098 s          0 s    8411342 s  3076734845 s         12 s
       #3  3501 MHz   64160236 s          0 s    7503489 s  3310777228 s         68 s
       #4  3501 MHz   61087245 s          0 s    7678941 s  3313659549 s         15 s
       
  Memory: 31.383651733398438 GB (2526.40625 MB free)
  Uptime: 3.3840841e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
