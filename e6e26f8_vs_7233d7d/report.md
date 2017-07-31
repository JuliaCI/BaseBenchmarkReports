# Benchmark Report

## Job Properties

*Commit(s):* [fredrikekre/julia@e6e26f8ebf9d49e9018d1b207765411a8600c80a](https://github.com/fredrikekre/julia/commit/e6e26f8ebf9d49e9018d1b207765411a8600c80a) vs [JuliaLang/julia@7233d7d61f15935ae43662425d74f66db71def01](https://github.com/JuliaLang/julia/commit/7233d7d61f15935ae43662425d74f66db71def01)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22923#issuecomment-319185860)

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
Julia Version 0.7.0-DEV.1182
Commit e6e26f8 (2017-07-31 20:11 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   81375119 s          0 s   14742354 s  3611113450 s         85 s
       #2  3501 MHz  331499191 s          0 s    9195909 s  3375226411 s         13 s
       #3  3501 MHz   70514751 s          0 s    8165673 s  3637627199 s         72 s
       #4  3501 MHz   67286601 s          0 s    8356782 s  3640646760 s         17 s
       
  Memory: 31.383651733398438 GB (2817.9296875 MB free)
  Uptime: 3.7180873e7 sec
  Load Avg:  1.0029296875  1.12353515625  1.4599609375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1180
Commit 7233d7d (2017-07-31 20:09 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   81454645 s          0 s   14749762 s  3611228701 s         85 s
       #2  3501 MHz  331644777 s          0 s    9203091 s  3375275998 s         13 s
       #3  3501 MHz   70607296 s          0 s    8173040 s  3637729620 s         72 s
       #4  3501 MHz   67364164 s          0 s    8363919 s  3640764578 s         17 s
       
  Memory: 31.383651733398438 GB (2809.9296875 MB free)
  Uptime: 3.7182902e7 sec
  Load Avg:  0.9228515625  1.08544921875  1.57763671875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
