# Benchmark Report

## Job Properties

*Commit(s):* [musm/julia@5f98c36d2b482f0207efd1eab999a2fc2b524912](https://github.com/musm/julia/commit/5f98c36d2b482f0207efd1eab999a2fc2b524912) vs [JuliaLang/julia@07cb7c19a5691df36a9d45ea486343e126fd8657](https://github.com/JuliaLang/julia/commit/07cb7c19a5691df36a9d45ea486343e126fd8657)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19491#issuecomment-265574333)

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
| `["scalar","floatexp",("exponent","norm","Float64")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","subnorm","Float32")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","inf -> inf","Float32")]` | 0.19 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","inf -> inf","Float64")]` | 0.19 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float32")]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float64")]` | 0.03 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> norm","Float32")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> norm","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> subnorm","Float32")]` | 0.43 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> subnorm","Float64")]` | 0.41 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> norm","Float32")]` | 0.09 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> norm","Float64")]` | 0.09 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> subnorm","Float32")]` | 0.29 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> subnorm","Float64")]` | 0.29 (15%) :white_check_mark: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.1414
Commit 5f98c36 (2016-12-07 18:07 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (14628.16796875 MB free)
Uptime: 1.6794678e7 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   25725265 s          0 s    4281511 s  1646076173 s         51 s
#2  3501 MHz   73629987 s          0 s    5244841 s  1597947756 s         18 s
#3  3501 MHz   22682213 s          0 s    2896716 s  1653121205 s         28 s
#4  3501 MHz   18828493 s          0 s    2812244 s  1657194793 s         10 s

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
Memory: 31.383651733398438 GB (14422.33984375 MB free)
Uptime: 1.6798731e7 sec
Load Avg:  1.0029296875  0.9853515625  0.95458984375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   25770942 s          0 s    4287966 s  1646428165 s         51 s
#2  3501 MHz   73831646 s          0 s    5254608 s  1598141118 s         18 s
#3  3501 MHz   22768789 s          0 s    2905330 s  1653430582 s         28 s
#4  3501 MHz   18869118 s          0 s    2818943 s  1657552178 s         10 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
