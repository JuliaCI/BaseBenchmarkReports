# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b68efd34e7e3827c1c63d92d3551b57ab90ec378](https://github.com/JuliaLang/julia/commit/b68efd34e7e3827c1c63d92d3551b57ab90ec378) vs [JuliaLang/julia@0e4493d598434232bbbe61b8e4b5d2b516550271](https://github.com/JuliaLang/julia/commit/0e4493d598434232bbbe61b8e4b5d2b516550271)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/b68efd34e7e3827c1c63d92d3551b57ab90ec378#commitcomment-29364214)

*Tag Predicate:* `"simd"`

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
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 1.97 (15%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 1.37 (15%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float32\", 4095)"]` | 8.02 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float32\", 4096)"]` | 8.55 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float64\", 4095)"]` | 3.40 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Float64\", 4096)"]` | 3.37 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int32\", 4095)"]` | 7.05 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int32\", 4096)"]` | 7.20 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int64\", 4095)"]` | 1.58 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"axpy!\", \"Int64\", 4096)"]` | 1.58 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int32\", 4096)"]` | 1.45 (20%) :x: | 1.00 (1%)  |
| `["simd", "(\"conditional_loop!\", \"Int64\", 4095)"]` | 1.30 (20%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array", "index"]`
- `["problem", "seismic"]`
- `["simd"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-alpha.122
Commit b68efd3 (2018-06-13 22:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   12355951 s        256 s    2157886 s  665526440 s          5 s
       #2  3501 MHz   62031049 s          0 s    1012719 s  618317218 s          4 s
       #3  3501 MHz    8549892 s       2388 s    1144892 s  671798156 s         10 s
       #4  3501 MHz    8291962 s          4 s     821330 s  672712315 s          2 s
       
  Memory: 31.383651733398438 GB (4040.9140625 MB free)
  Uptime: 6.821048e6 sec
  Load Avg:  0.92919921875  0.998046875  1.0400390625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-alpha.126
Commit 0e4493d (2018-06-14 13:46 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   12502366 s        256 s    2167739 s  665859391 s          5 s
       #2  3501 MHz   62433763 s          0 s    1021990 s  618395619 s          4 s
       #3  3501 MHz    8664764 s       2388 s    1153442 s  672164745 s         10 s
       #4  3501 MHz    8405214 s          4 s     830044 s  673080710 s          2 s
       
  Memory: 31.383651733398438 GB (6124.3359375 MB free)
  Uptime: 6.825958e6 sec
  Load Avg:  1.00439453125  1.0146484375  1.046875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
