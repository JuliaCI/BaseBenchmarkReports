# Benchmark Report

## Job Properties

*Commit(s):* [musm/julia@9c33452171a3b31c3723fbeb8454422a4a2e243a](https://github.com/musm/julia/commit/9c33452171a3b31c3723fbeb8454422a4a2e243a) vs [JuliaLang/julia@07cb7c19a5691df36a9d45ea486343e126fd8657](https://github.com/JuliaLang/julia/commit/07cb7c19a5691df36a9d45ea486343e126fd8657)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19512#issuecomment-265574274)

*Tag Predicate:* `"scalar"`

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

- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1413
Commit 9c33452 (2016-12-07 18:06 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (14702.6953125 MB free)
Uptime: 1.6794731e7 sec
Load Avg:  0.9970703125  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   22284605 s          0 s    5355333 s  1647016603 s         50 s
#2  3501 MHz   67723838 s          0 s    3220618 s  1607523303 s          7 s
#3  3501 MHz   22014355 s          0 s    2808542 s  1653880902 s         33 s
#4  3501 MHz   19042510 s          0 s    2846722 s  1656799797 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1410
Commit 07cb7c1 (2016-12-07 16:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (14563.8203125 MB free)
Uptime: 1.6798779e7 sec
Load Avg:  0.9169921875  0.96875  0.94921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   22340847 s          0 s    5362678 s  1647356634 s         50 s
#2  3501 MHz   67871497 s          0 s    3228179 s  1607772493 s          7 s
#3  3501 MHz   22043944 s          0 s    2813848 s  1654250023 s         33 s
#4  3501 MHz   19183107 s          0 s    2857457 s  1657052810 s          6 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
