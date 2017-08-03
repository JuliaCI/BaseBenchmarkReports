# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a342e0ffe32f3297f8d88bb08c9fec473ee938cb](https://github.com/JuliaLang/julia/commit/a342e0ffe32f3297f8d88bb08c9fec473ee938cb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/a342e0ffe32f3297f8d88bb08c9fec473ee938cb#commitcomment-23450287)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-08-03 vs 2017-08-02

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
| `["array","index",("sumcolon_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","julia",("macroexpand","evalpoly")]` | 0.55 (15%) :white_check_mark: | 0.96 (1%) :white_check_mark: |
| `["random","collections",("rand","RandomDevice","small IntSet")]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float32","cos_kernel")]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float32","cos_kernel")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64","cos_kernel")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) > 2.0^20*π/2","negative argument","Float64")]` | 0.42 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) > 2.0^20*π/2","positive argument","Float64")]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (hard) abs(x) < 8π/4","positive argument","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 2.0^20π/4","negative argument","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 2π/4","negative argument","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 2π/4","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 3π/4","negative argument","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 3π/4","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 4π/4","negative argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 4π/4","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 5π/4","negative argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 6π/4","negative argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 7π/4","negative argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 7π/4","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 8π/4","negative argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 8π/4","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 9π/4","negative argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (easy) abs(x) < 9π/4","positive argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) abs(x) < 2π/4","positive argument","Float64")]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) abs(x) < 4π/4","negative argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (hard) abs(x) < 6π/4","negative argument","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","rem_pio2",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","positive argument","Float64")]` | 0.40 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","sin",("argument reduction (paynehanek) abs(x) > 2.0^20*π/2","negative argument","Float64","sin_kernel")]` | 1.77 (15%) :x: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 1.29 (20%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 1.46 (30%) :x: | 1.00 (1%)  |

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
- `["scalar","arithmetic"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
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
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1213
Commit a342e0f (2017-08-03 01:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   82194866 s          0 s   14858214 s  3630489999 s         85 s
       #2  3501 MHz  336010269 s          0 s    9298822 s  3390982618 s         13 s
       #3  3501 MHz   71365484 s          0 s    8243528 s  3657068850 s         73 s
       #4  3501 MHz   68086703 s          0 s    8431766 s  3660144504 s         17 s
       
  Memory: 31.383651733398438 GB (3274.85546875 MB free)
  Uptime: 3.7384676e7 sec
  Load Avg:  1.00927734375  1.0185546875  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
