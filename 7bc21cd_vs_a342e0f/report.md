# Benchmark Report

## Job Properties

*Commit(s):* [fredrikekre/julia@7bc21cde15d96fcc8950096c68965adba14ba5fa](https://github.com/fredrikekre/julia/commit/7bc21cde15d96fcc8950096c68965adba14ba5fa) vs [JuliaLang/julia@a342e0ffe32f3297f8d88bb08c9fec473ee938cb](https://github.com/JuliaLang/julia/commit/a342e0ffe32f3297f8d88bb08c9fec473ee938cb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22925#issuecomment-319843524)

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
Julia Version 0.7.0-DEV.1215
Commit 7bc21cd (2017-08-03 01:33 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   82030682 s          0 s   14841392 s  3629444112 s         85 s
       #2  3501 MHz  335246429 s          0 s    9280550 s  3390534801 s         13 s
       #3  3501 MHz   71205571 s          0 s    8228933 s  3656013604 s         73 s
       #4  3501 MHz   67928634 s          0 s    8417464 s  3659086867 s         17 s
       
  Memory: 31.383651733398438 GB (3489.01953125 MB free)
  Uptime: 3.7372365e7 sec
  Load Avg:  1.0029296875  1.11083984375  1.44775390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1213
Commit a342e0f (2017-08-03 01:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   82120780 s          0 s   14848651 s  3629539404 s         85 s
       #2  3501 MHz  335384990 s          0 s    9287523 s  3390582253 s         13 s
       #3  3501 MHz   71284266 s          0 s    8236329 s  3656120294 s         73 s
       #4  3501 MHz   68007370 s          0 s    8424438 s  3659194160 s         17 s
       
  Memory: 31.383651733398438 GB (3437.00390625 MB free)
  Uptime: 3.7374299e7 sec
  Load Avg:  1.0029296875  1.1416015625  1.64013671875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
