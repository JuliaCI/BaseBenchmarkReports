# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@725a14bc86db564bbb0945b00568d0740bc301f8](https://github.com/JuliaLang/julia/commit/725a14bc86db564bbb0945b00568d0740bc301f8) vs [JuliaLang/julia@379c248bb02690651a6f5cc2bbdb4f991ad3af9b](https://github.com/JuliaLang/julia/commit/379c248bb02690651a6f5cc2bbdb4f991ad3af9b)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18259#issuecomment-242910044)

*Tag Predicate:* `"string" || "problem"`

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
| `["string","join"]` | 1.45 (40%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["io","read"]`
- `["problem","fem"]`
- `["problem","go"]`
- `["problem","grigoriadis khachiyan"]`
- `["problem","imdb"]`
- `["problem","json"]`
- `["problem","laplacian"]`
- `["problem","monte carlo"]`
- `["problem","raytrace"]`
- `["problem","seismic"]`
- `["problem","simplex"]`
- `["problem","spellcheck"]`
- `["problem","stockcorr"]`
- `["problem","ziggurat"]`
- `["string"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.421
Commit 725a14b (2016-08-27 08:06 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20473.859375 MB free)
Uptime: 7.943357e6 sec
Load Avg:  1.01416015625  0.95361328125  0.92919921875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   13685196 s          0 s    2767269 s  775613082 s         28 s
#2  3501 MHz   34851847 s          0 s    1735003 s  757205114 s          4 s
#3  3501 MHz   12200154 s          0 s    1513828 s  780237208 s         17 s
#4  3501 MHz   10521110 s          0 s    1522286 s  781894747 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.419
Commit 379c248 (2016-08-27 08:05 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (20462.79296875 MB free)
Uptime: 7.946645e6 sec
Load Avg:  1.03857421875  1.009765625  0.96826171875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   13717526 s          0 s    2773729 s  775901875 s         28 s
#2  3501 MHz   34897892 s          0 s    1740378 s  757481969 s          4 s
#3  3501 MHz   12349396 s          0 s    1524725 s  780405282 s         17 s
#4  3501 MHz   10591746 s          0 s    1529946 s  782144782 s          2 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
