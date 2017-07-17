# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@18dbb0f09b91abbfeb33f3c5b60c52923fae7c2f](https://github.com/JuliaLang/julia/commit/18dbb0f09b91abbfeb33f3c5b60c52923fae7c2f) vs [JuliaLang/julia@66ef3476310bef00616be0e2c28aca29a1b0c487](https://github.com/JuliaLang/julia/commit/66ef3476310bef00616be0e2c28aca29a1b0c487)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21984#issuecomment-315691238)

*Tag Predicate:* `"arithmetic"`

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
| `["scalar","arithmetic",("rem type","BigInt","Bool")]` | 0.54 (40%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","fastmath",("div","UInt64")]` | 1.43 (40%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates","arithmetic"]`
- `["linalg","arithmetic"]`
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["sparse","arithmetic"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1012
Commit 18dbb0f (2017-07-17 07:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   77086801 s          0 s   14150843 s  3491292696 s         84 s
       #2  3501 MHz  317216697 s          0 s    8842668 s  3264834867 s         13 s
       #3  3501 MHz   67873596 s          0 s    7904998 s  3515488267 s         70 s
       #4  3501 MHz   64710996 s          0 s    8083480 s  3518460451 s         16 s
       
  Memory: 31.383651733398438 GB (10698.8984375 MB free)
  Uptime: 3.5929979e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.3935546875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1007
Commit 66ef347 (2017-07-17 07:05 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   77163928 s          0 s   14158361 s  3491475708 s         84 s
       #2  3501 MHz  317430643 s          0 s    8849734 s  3264882057 s         13 s
       #3  3501 MHz   67967811 s          0 s    7912001 s  3515655132 s         70 s
       #4  3501 MHz   64786351 s          0 s    8090330 s  3518646433 s         16 s
       
  Memory: 31.383651733398438 GB (10609.88671875 MB free)
  Uptime: 3.5932666e7 sec
  Load Avg:  0.9970703125  1.0146484375  1.27685546875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
