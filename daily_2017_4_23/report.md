# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@1b2afd9146c2fcfdd4de51258cf7d3d4a9be9d46](https://github.com/JuliaLang/julia/commit/1b2afd9146c2fcfdd4de51258cf7d3d4a9be9d46)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/1b2afd9146c2fcfdd4de51258cf7d3d4a9be9d46#commitcomment-21869412)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-04-23 vs 2017-04-22

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
| `["array","cat",("hcat",5)]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 2.40 (45%) :x: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 2.38 (45%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 1.24 (20%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 0.75 (20%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("minimum",(4,4))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,))]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 1.20 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-pre.beta.272
Commit 1b2afd9 (2017-04-23 02:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2662.23046875 MB free)
Uptime: 2.85707e7 sec
Load Avg:  0.95556640625  1.009765625  1.04052734375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   56792801 s          0 s   10967541 s  2780991791 s         77 s
#2  3501 MHz  230768020 s          0 s    6807077 s  2617827458 s         11 s
#3  3501 MHz   50917310 s          0 s    6048096 s  2798731218 s         59 s
#4  3501 MHz   48192767 s          0 s    6187703 s  2801323722 s         12 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
