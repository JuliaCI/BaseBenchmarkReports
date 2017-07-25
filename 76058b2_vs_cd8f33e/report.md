# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@76058b20c8c31bf7f802a4753ecd614bfc7abeb3](https://github.com/pkofod/julia/commit/76058b20c8c31bf7f802a4753ecd614bfc7abeb3) vs [JuliaLang/julia@cd8f33ea9989a0364d01f7b55249379eec1643f0](https://github.com/JuliaLang/julia/commit/cd8f33ea9989a0364d01f7b55249379eec1643f0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22603#issuecomment-317860158)

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
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1147
Commit 76058b2 (2017-07-25 19:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   75093826 s          0 s   11667880 s  3571744624 s        124 s
       #2  3501 MHz  295097985 s          0 s   12664247 s  3352124195 s         42 s
       #3  3501 MHz   64095960 s          0 s    7416810 s  3593349603 s         59 s
       #4  3501 MHz   59536158 s          0 s    7348818 s  3598317911 s         20 s
       
  Memory: 31.383651733398438 GB (14630.6484375 MB free)
  Uptime: 3.666479e7 sec
  Load Avg:  0.9228515625  1.00390625  1.45751953125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1107
Commit cd8f33e (2017-07-24 20:10 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   75172694 s          0 s   11675908 s  3571912094 s        124 s
       #2  3501 MHz  295312752 s          0 s   12671516 s  3352157030 s         42 s
       #3  3501 MHz   64177311 s          0 s    7423900 s  3593515897 s         59 s
       #4  3501 MHz   59612686 s          0 s    7356045 s  3598489096 s         20 s
       
  Memory: 31.383651733398438 GB (14569.765625 MB free)
  Uptime: 3.6667345e7 sec
  Load Avg:  0.9169921875  1.0  1.33251953125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
