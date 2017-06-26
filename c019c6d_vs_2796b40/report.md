# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c019c6dd30bd96377daefc0e9c86ba323649600d](https://github.com/JuliaLang/julia/commit/c019c6dd30bd96377daefc0e9c86ba323649600d) vs [JuliaLang/julia@2796b40176dbe489602c5eef9951dfb005316779](https://github.com/JuliaLang/julia/commit/2796b40176dbe489602c5eef9951dfb005316779)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22481#issuecomment-311159872)

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
| `["array","index",("sumcartesian","BitArray{2}")]` | 0.16 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcartesian_view","BitArray{2}")]` | 0.34 (50%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","BitArray{2}")]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BitArray{2}")]` | 0.11 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumeach_view","BitArray{2}")]` | 0.81 (50%)  | 0.85 (1%) :white_check_mark: |
| `["array","index",("sumelt","BitArray{2}")]` | 0.09 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 0.15 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear","BitArray{2}")]` | 0.10 (50%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 0.81 (50%)  | 0.85 (1%) :white_check_mark: |
| `["array","index",("sumrange_view","BitArray{2}")]` | 0.46 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector_view","BitArray{2}")]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.29 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}()")]` | 0.36 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(0.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 2.73 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)")]` | 2.79 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}(1.000000000000000000000000000000000000000000000000000000000000000000000000000000)","Nullable{BigFloat}()")]` | 2.79 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}()")]` | 0.36 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(0)")]` | 2.73 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}(1)")]` | 2.79 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}()")]` | 2.79 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}(0)")]` | 2.22 (60%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}(1)","Nullable{BigInt}(1)")]` | 2.01 (60%) :x: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 0.91 (15%)  | 0.74 (1%) :white_check_mark: |
| `["shootout","spectralnorm"]` | 1.00 (15%)  | 0.22 (1%) :white_check_mark: |
| `["simd",("two_reductions","Int32",4095)]` | 0.13 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int32",4096)]` | 0.14 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",1000)]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 1.42 (30%) :x: | 1.00 (1%)  |
| `["tuple","linear algebra",("matvec",(4,4),(4,))]` | 1.42 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.744
Commit c019c6d (2017-06-26 19:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   70983973 s          0 s   10920334 s  3326470742 s         94 s
       #2  3501 MHz  279417573 s          0 s   11998478 s  3118098723 s         39 s
       #3  3501 MHz   60926986 s          0 s    7078935 s  3346151118 s         52 s
       #4  3501 MHz   56335758 s          0 s    7002064 s  3351146764 s         18 s
       
  Memory: 31.383651733398438 GB (2446.15234375 MB free)
  Uptime: 3.4157029e7 sec
  Load Avg:  1.14990234375  1.046875  1.0556640625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.741
Commit 2796b40 (2017-06-26 19:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   71063125 s          0 s   10928967 s  3326906718 s         94 s
       #2  3501 MHz  279900778 s          0 s   12006439 s  3118133129 s         39 s
       #3  3501 MHz   61006551 s          0 s    7086431 s  3346589212 s         52 s
       #4  3501 MHz   56414446 s          0 s    7009369 s  3351586339 s         18 s
       
  Memory: 31.383651733398438 GB (2493.828125 MB free)
  Uptime: 3.4162294e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
