# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@820e7824a7de518535395318bb0e8da609f2c93a](https://github.com/JuliaLang/julia/commit/820e7824a7de518535395318bb0e8da609f2c93a) vs [JuliaLang/julia@cb50e0bf1468ff56d85a7b95c7d2cd693309bed7](https://github.com/JuliaLang/julia/commit/cb50e0bf1468ff56d85a7b95c7d2cd693309bed7)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22420#issuecomment-310904962)

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
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup_x3")]` | 1.89 (15%) :x: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}()")]` | 0.18 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigInt}()","Nullable{BigInt}()")]` | 0.21 (60%) :white_check_mark: | 1.00 (1%)  |
| `["problem","spellcheck","spellcheck"]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.40 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.718
Commit 820e782 (2017-06-25 13:22 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   71262896 s          0 s   13320136 s  3310652886 s         83 s
       #2  3501 MHz  299340731 s          0 s    8455866 s  3095329789 s         12 s
       #3  3501 MHz   64569297 s          0 s    7549155 s  3331363642 s         68 s
       #4  3501 MHz   61479061 s          0 s    7720063 s  3334270952 s         15 s
       
  Memory: 31.383651733398438 GB (2507.44921875 MB free)
  Uptime: 3.4051342e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.716
Commit cb50e0b (2017-06-25 12:53 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   71340716 s          0 s   13328927 s  3311091641 s         83 s
       #2  3501 MHz  299809361 s          0 s    8463705 s  3095380104 s         12 s
       #3  3501 MHz   64660512 s          0 s    7556546 s  3331791815 s         68 s
       #4  3501 MHz   61560105 s          0 s    7727272 s  3334709583 s         15 s
       
  Memory: 31.383651733398438 GB (2571.98046875 MB free)
  Uptime: 3.4056615e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
