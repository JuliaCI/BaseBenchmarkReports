# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@14b81ae2fb7ee47d9f125320f29dfb4b8f622ab5](https://github.com/JuliaLang/julia/commit/14b81ae2fb7ee47d9f125320f29dfb4b8f622ab5) vs [JuliaLang/julia@f8d3fbb1343696439e5f1a62f1c43848306d1c36](https://github.com/JuliaLang/julia/commit/f8d3fbb1343696439e5f1a62f1c43848306d1c36)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25002#issuecomment-350441793)

*Tag Predicate:* `"random"`

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

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["problem", "monte carlo"]`
- `["random", "collections"]`
- `["random", "randstring"]`
- `["random", "ranges"]`
- `["random", "sequences"]`
- `["random", "types"]`
- `["sort", "insertionsort"]`
- `["sort", "issorted"]`
- `["sort", "mergesort"]`
- `["sort", "quicksort"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2809
Commit 14b81ae (2017-12-09 10:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   98203060 s          0 s   15209177 s  4722116264 s        224 s
       #2  3501 MHz  392113632 s          0 s   16434440 s  4429332299 s         79 s
       #3  3501 MHz   80266758 s          0 s    9084035 s  4755106630 s        104 s
       #4  3501 MHz   75465745 s          0 s    8999490 s  4760391512 s         42 s
       
  Memory: 31.383651733398438 GB (2841.5 MB free)
  Uptime: 4.8464224e7 sec
  Load Avg:  1.0029296875  1.19140625  1.9755859375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2807
Commit f8d3fbb (2017-12-09 09:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   98301948 s          0 s   15217691 s  4722197414 s        224 s
       #2  3501 MHz  392241576 s          0 s   16443897 s  4429383642 s         79 s
       #3  3501 MHz   80355850 s          0 s    9091918 s  4755198213 s        104 s
       #4  3501 MHz   75549486 s          0 s    9007307 s  4760488615 s         42 s
       
  Memory: 31.383651733398438 GB (2804.0546875 MB free)
  Uptime: 4.8466118e7 sec
  Load Avg:  0.9228515625  1.20458984375  1.81982421875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
