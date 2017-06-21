# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@236e48634d94c0e96671bb9948d24a26b20ec66d](https://github.com/JuliaLang/julia/commit/236e48634d94c0e96671bb9948d24a26b20ec66d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/236e48634d94c0e96671bb9948d24a26b20ec66d#commitcomment-22669577)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-06-21 vs 2017-06-20

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
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 1.36 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup")]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("array",3)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["dates","construction","DateTime"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.43 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}()")]` | 2.83 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}()")]` | 2.83 (60%) :x: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{BigFloat}")]` | 1.42 (40%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","integer",100)]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.666
Commit 236e486 (2017-06-20 22:46 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   70712191 s          0 s   13196824 s  3273109483 s         82 s
       #2  3501 MHz  295982716 s          0 s    8385335 s  3060448478 s         12 s
       #3  3501 MHz   64004775 s          0 s    7476515 s  3293691175 s         67 s
       #4  3501 MHz   60911875 s          0 s    7655828 s  3296587959 s         15 s
       
  Memory: 31.383651733398438 GB (2552.72265625 MB free)
  Uptime: 3.3668049e7 sec
  Load Avg:  1.09033203125  1.041015625  1.05078125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
