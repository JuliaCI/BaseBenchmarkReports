# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@309bd549d54fabcf572dc771df6a86c901888a03](https://github.com/pkofod/julia/commit/309bd549d54fabcf572dc771df6a86c901888a03) vs [JuliaLang/julia@dda08d612448dcf8a8aeae02f42ab3936441bff3](https://github.com/JuliaLang/julia/commit/dda08d612448dcf8a8aeae02f42ab3936441bff3)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23283#issuecomment-332134223)

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
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 1.65 (50%) :x: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","Complex{Int16}")]` | 1.25 (25%) :x: | 1.00 (1%)  |
| `["random","types",("randn!","MersenneTwister","Float32")]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("0.5 <= abs(x) < 1","positive argument","Float32")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("abs(x) < 0.5","negative argument","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("abs(x) < 0.5","positive argument","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("one","negative argument","Float32")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("one","negative argument","Float64")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("one","positive argument","Float32")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("one","positive argument","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("small","negative argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("small","positive argument","Float64")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","acos",("zero","Float64")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64","sin_kernel")]` | 3.60 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 0.79 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("adjoint!",(20000,20000))]` | 0.63 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string","join"]` | 1.57 (40%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
- `["misc","julia"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
- `["parallel","remotecall"]`
- `["problem","chaosgame"]`
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
- `["random","collections"]`
- `["random","randstring"]`
- `["random","ranges"]`
- `["random","sequences"]`
- `["random","types"]`
- `["scalar","acos"]`
- `["scalar","arithmetic"]`
- `["scalar","asin"]`
- `["scalar","atan"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
- `["scalar","tan"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","constructors"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["string","readuntil"]`
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1965
Commit 309bd54 (2017-09-26 08:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   94745394 s          0 s   16828337 s  4083090784 s         92 s
       #2  3501 MHz  404536208 s          0 s   10825294 s  3789206077 s         20 s
       #3  3501 MHz   81977548 s          0 s    9321602 s  4113680446 s         76 s
       #4  3501 MHz   78374512 s          0 s    9508671 s  4117101656 s         18 s
       
  Memory: 31.383651733398438 GB (3089.453125 MB free)
  Uptime: 4.206998e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1961
Commit dda08d6 (2017-09-26 07:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   94823588 s          0 s   16837684 s  4083718395 s         92 s
       #2  3501 MHz  405189116 s          0 s   10836943 s  3789258789 s         20 s
       #3  3501 MHz   82075338 s          0 s    9329327 s  4114291965 s         76 s
       #4  3501 MHz   78456666 s          0 s    9516170 s  4117729294 s         18 s
       
  Memory: 31.383651733398438 GB (3023.203125 MB free)
  Uptime: 4.2077159e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
