# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@819ffc0706b150c72aa9cbf23d21cf2a3b537f25](https://github.com/JuliaLang/julia/commit/819ffc0706b150c72aa9cbf23d21cf2a3b537f25) vs [JuliaLang/julia@6c9f5afa89f451bf2262af6f2bdd87b7b7a328d4](https://github.com/JuliaLang/julia/commit/6c9f5afa89f451bf2262af6f2bdd87b7b7a328d4)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18929#issuecomment-254056052)

*Tag Predicate:* `"linalg"`

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

- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.988
Commit 819ffc0 (2016-10-16 06:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (12936.64453125 MB free)
Uptime: 1.2283421e7 sec
Load Avg:  1.0029296875  0.9853515625  0.94580078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   20549929 s          0 s    3412286 s  1201811237 s         40 s
#2  3501 MHz   54037223 s          0 s    3788686 s  1168740405 s         12 s
#3  3501 MHz   18029678 s          0 s    2276281 s  1207441582 s         19 s
#4  3501 MHz   14927588 s          0 s    2198918 s  1210727261 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.986
Commit 6c9f5af (2016-10-16 05:19 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (13044.01171875 MB free)
Uptime: 1.2287053e7 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   20656067 s          0 s    3421682 s  1202058041 s         40 s
#2  3501 MHz   54167046 s          0 s    3797292 s  1168964671 s         12 s
#3  3501 MHz   18078536 s          0 s    2282911 s  1207748526 s         19 s
#4  3501 MHz   14975623 s          0 s    2205056 s  1211035774 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
