# Benchmark Report

## Job Properties

*Commit(s):* [pabloferz/julia@97cd7012aa04de8561537853db90f709b3ac06f1](https://github.com/pabloferz/julia/commit/97cd7012aa04de8561537853db90f709b3ac06f1) vs [JuliaLang/julia@f2b4ff5e68e1a46179bbd109505a41ee6b5e8972](https://github.com/JuliaLang/julia/commit/f2b4ff5e68e1a46179bbd109505a41ee6b5e8972)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23887#issuecomment-334036937)

*Tag Predicate:* `"tuple" || "scalar"`

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
| `["scalar","atan2",("x one","Float64")]` | 0.56 (15%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["broadcast","mix_scalar_tuple"]`
- `["broadcast","typeargs"]`
- `["scalar","acos"]`
- `["scalar","arithmetic"]`
- `["scalar","asin"]`
- `["scalar","atan"]`
- `["scalar","atan2"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
- `["scalar","tan"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2046
Commit 97cd701 (2017-10-03 19:35 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   88258109 s          0 s   13711693 s  4162000841 s        178 s
       #2  3501 MHz  356028937 s          0 s   14705492 s  3895290627 s         62 s
       #3  3501 MHz   73906460 s          0 s    8439590 s  4189351356 s         84 s
       #4  3501 MHz   69181890 s          0 s    8312945 s  4194604893 s         30 s
       
  Memory: 31.383651733398438 GB (3249.7265625 MB free)
  Uptime: 4.2735291e7 sec
  Load Avg:  0.9228515625  0.998046875  1.10888671875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2044
Commit f2b4ff5 (2017-10-03 19:34 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   88339125 s          0 s   13720314 s  4162249302 s        178 s
       #2  3501 MHz  356310187 s          0 s   14713299 s  3895340402 s         63 s
       #3  3501 MHz   73988880 s          0 s    8447314 s  4189599918 s         84 s
       #4  3501 MHz   69279451 s          0 s    8320727 s  4194838393 s         30 s
       
  Memory: 31.383651733398438 GB (3203.5703125 MB free)
  Uptime: 4.2738686e7 sec
  Load Avg:  0.9228515625  0.998046875  1.12890625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
