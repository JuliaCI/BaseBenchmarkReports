# Benchmark Report

## Job Properties

*Commit(s):* [mbauman/julia@1d384a9631a7991349c473367ac00522af465628](https://github.com/mbauman/julia/commit/1d384a9631a7991349c473367ac00522af465628) vs [JuliaLang/julia@2b7481daa86238ccdea7f980c5a7caab8df07d66](https://github.com/JuliaLang/julia/commit/2b7481daa86238ccdea7f980c5a7caab8df07d66)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/15558#issuecomment-252759105)

*Tag Predicate:* `"array"`

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
| `["array","cat",("vcat",5)]` | 1.01 (15%)  | 1.06 (1%) :x: |
| `["array","index",("sumcolon","BitArray{2}")]` | 1.18 (50%)  | 1.52 (1%) :x: |
| `["array","index",("sumrange","BitArray{2}")]` | 1.15 (50%)  | 1.46 (1%) :x: |
| `["array","setindex!",("setindex!",2)]` | 1.18 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["problem","laplacian"]`
- `["simd"]`
- `["sparse","index"]`
- `["sparse","transpose"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.926
Commit 1d384a9 (2016-10-10 21:56 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17220.83984375 MB free)
Uptime: 1.1786872e7 sec
Load Avg:  0.9970703125  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   19314028 s          0 s    3236649 s  1153674649 s         36 s
#2  3501 MHz   50464891 s          0 s    3588216 s  1122942318 s         11 s
#3  3501 MHz   16979175 s          0 s    2166217 s  1158969139 s         18 s
#4  3501 MHz   14309040 s          0 s    2114571 s  1161789258 s          5 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.924
Commit 2b7481d (2016-10-10 21:51 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (17100.2265625 MB free)
Uptime: 1.1790987e7 sec
Load Avg:  1.0029296875  1.001953125  0.9599609375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   19436326 s          0 s    3247496 s  1153952236 s         36 s
#2  3501 MHz   50618864 s          0 s    3596271 s  1123191136 s         11 s
#3  3501 MHz   17026763 s          0 s    2171993 s  1159326550 s         18 s
#4  3501 MHz   14365720 s          0 s    2121385 s  1162136726 s          5 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
