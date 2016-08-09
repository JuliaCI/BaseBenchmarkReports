# Benchmark Report

## Job Properties

*Commit(s):* [mbauman/julia@36527741557bde80e29e3c59a98e5023ddf993d3](https://github.com/mbauman/julia/commit/36527741557bde80e29e3c59a98e5023ddf993d3) vs [JuliaLang/julia@20374640c0305b0b0433eff35a038f76049e7e7d](https://github.com/JuliaLang/julia/commit/20374640c0305b0b0433eff35a038f76049e7e7d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/15558#issuecomment-238420692)

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
| `["array","index",("sumcolon","BitArray{2}")]` | 1.24 (40%)  | 1.56 (1%) :x: |
| `["array","index",("sumelt","100000000:-1:1")]` | 1.54 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","Array{Int32,2}")]` | 1.48 (40%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","BitArray{2}")]` | 1.25 (40%)  | 1.49 (1%) :x: |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4096)]` | 0.77 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4095)]` | 0.69 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4096)]` | 0.70 (20%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.102
Commit 3652774 (2016-08-09 00:41 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (22761.46484375 MB free)
Uptime: 6.352594e6 sec
Load Avg:  0.9169921875  0.96875  0.94921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    8486952 s          0 s    1994431 s  622938092 s         22 s
#2  3501 MHz   21781392 s          0 s    1127659 s  611906660 s          2 s
#3  3501 MHz    8084616 s          0 s    1025094 s  625858545 s         10 s
#4  3501 MHz    6535967 s          0 s    1001096 s  627419967 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.100
Commit 2037464 (2016-08-08 21:35 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (22649.25 MB free)
Uptime: 6.356475e6 sec
Load Avg:  1.0458984375  1.001953125  0.9521484375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz    8529014 s          0 s    2001206 s  623276162 s         22 s
#2  3501 MHz   21908300 s          0 s    1134686 s  612160352 s          2 s
#3  3501 MHz    8201061 s          0 s    1034200 s  626120375 s         11 s
#4  3501 MHz    6608314 s          0 s    1008628 s  627727666 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
