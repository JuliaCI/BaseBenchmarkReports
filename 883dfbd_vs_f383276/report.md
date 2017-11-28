# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@883dfbd4abc4ff04333aaf1569a0cd28fc536053](https://github.com/JuliaLang/julia/commit/883dfbd4abc4ff04333aaf1569a0cd28fc536053) vs [JuliaLang/julia@f383276c5b91d4d111f628c2eaa6b2db2f496421](https://github.com/JuliaLang/julia/commit/f383276c5b91d4d111f628c2eaa6b2db2f496421)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24653#issuecomment-347504628)

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
| `["array", "any/all", "(\"any\", \"Array{Float32,1}\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"Array{Float64,1} generator\")"]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array", "any/all", "(\"any\", \"UnitRange{Int64}\")"]` | 1.49 (15%) :x: | 1.00 (1%)  |
| `["array", "growth", "(\"prerend!\", 256)"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"Base.LinAlg.UnitUpperTriangular\", 1024)"]` | 2.34 (45%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"sqrt\", \"UpperTriangular\", 1024)"]` | 2.37 (45%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Diagonal\", 10)"]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"integer\", 1000)"]` | 1.33 (30%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array", "any/all"]`
- `["array", "bool"]`
- `["array", "cat"]`
- `["array", "comprehension"]`
- `["array", "convert"]`
- `["array", "equality"]`
- `["array", "growth"]`
- `["array", "index"]`
- `["array", "reductions"]`
- `["array", "reverse"]`
- `["array", "setindex!"]`
- `["array", "subarray"]`
- `["broadcast", "dotop"]`
- `["broadcast", "fusion"]`
- `["broadcast", "sparse"]`
- `["broadcast", "typeargs"]`
- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["misc", "julia"]`
- `["misc", "repeat"]`
- `["misc", "splatting"]`
- `["problem", "laplacian"]`
- `["simd"]`
- `["sparse", "arithmetic"]`
- `["sparse", "constructors"]`
- `["sparse", "index"]`
- `["sparse", "matmul"]`
- `["sparse", "transpose"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2677
Commit 883dfbd (2017-11-27 20:42 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  104690400 s          0 s   18537060 s  4615078316 s         98 s
       #2  3501 MHz  446751791 s          0 s   11849885 s  4290796103 s         22 s
       #3  3501 MHz   88456155 s          0 s   10133127 s  4651281181 s         81 s
       #4  3501 MHz   84632915 s          0 s   10320233 s  4654908230 s         21 s
       
  Memory: 31.383651733398438 GB (3936.375 MB free)
  Uptime: 4.7521454e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.07958984375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2675
Commit f383276 (2017-11-27 20:28 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  104780335 s          0 s   18545311 s  4615378080 s         98 s
       #2  3501 MHz  447084061 s          0 s   11858031 s  4290854596 s         22 s
       #3  3501 MHz   88555371 s          0 s   10140838 s  4651572873 s         81 s
       #4  3501 MHz   84713084 s          0 s   10328080 s  4655219099 s         21 s
       
  Memory: 31.383651733398438 GB (3768.62890625 MB free)
  Uptime: 4.7525448e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.0869140625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
