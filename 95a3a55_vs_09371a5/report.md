# Benchmark Report

## Job Properties

*Commit(s):* [musm/julia@95a3a553744e5dd5ddd33ea589d70f92eb65e37b](https://github.com/musm/julia/commit/95a3a553744e5dd5ddd33ea589d70f92eb65e37b) vs [JuliaLang/julia@09371a5c904348b4f7883dac8e3e034818678e87](https://github.com/JuliaLang/julia/commit/09371a5c904348b4f7883dac8e3e034818678e87)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23046#issuecomment-319107436)

*Tag Predicate:* `"rand"`

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
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:2^10000)")]` | 1.26 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","Complex{Float32}")]` | 1.26 (25%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["micro"]`
- `["random","collections"]`
- `["random","ranges"]`
- `["random","types"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1172
Commit 95a3a55 (2017-07-31 13:43 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   81037436 s          0 s   14711645 s  3609750480 s         85 s
       #2  3501 MHz  330941150 s          0 s    9156846 s  3374089325 s         13 s
       #3  3501 MHz   70183382 s          0 s    8136182 s  3636254655 s         72 s
       #4  3501 MHz   66975133 s          0 s    8328128 s  3639252623 s         17 s
       
  Memory: 31.383651733398438 GB (2774.85546875 MB free)
  Uptime: 3.7163509e7 sec
  Load Avg:  0.9228515625  1.14013671875  1.53955078125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1169
Commit 09371a5 (2017-07-31 13:38 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   81131946 s          0 s   14718934 s  3609837077 s         85 s
       #2  3501 MHz  331069016 s          0 s    9167296 s  3374139638 s         13 s
       #3  3501 MHz   70261903 s          0 s    8143417 s  3636357419 s         72 s
       #4  3501 MHz   67052779 s          0 s    8335193 s  3639356585 s         17 s
       
  Memory: 31.383651733398438 GB (2787.78515625 MB free)
  Uptime: 3.71654e7 sec
  Load Avg:  0.9970703125  1.14599609375  1.6708984375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
