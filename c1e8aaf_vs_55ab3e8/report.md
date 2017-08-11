# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c1e8aaf41d219b72c001304d425e33222c3bc370](https://github.com/JuliaLang/julia/commit/c1e8aaf41d219b72c001304d425e33222c3bc370) vs [JuliaLang/julia@55ab3e81b37e9d2159a16b4dfa75dcede0a144df](https://github.com/JuliaLang/julia/commit/55ab3e81b37e9d2159a16b4dfa75dcede0a144df)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22612#issuecomment-321784968)

*Tag Predicate:* `"random"`

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
| `["random","collections",("rand","ImplicitRNG","'a':'z'")]` | 0.61 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","ImplicitRNG","large Vector")]` | 0.38 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","ImplicitRNG","small Vector")]` | 0.44 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","MersenneTwister","'a':'z'")]` | 0.60 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","MersenneTwister","large Vector")]` | 0.37 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","collections",("rand","MersenneTwister","small Vector")]` | 0.43 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","ImplicitRNG","Int","1:1000")]` | 0.29 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.06 (25%)  | 0.99 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","Int","1:1000")]` | 0.28 (25%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["problem","monte carlo"]`
- `["random","collections"]`
- `["random","randstring"]`
- `["random","ranges"]`
- `["random","sequences"]`
- `["random","types"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1326
Commit c1e8aaf (2017-08-11 11:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   84573014 s          0 s   15202087 s  3698864333 s         87 s
       #2  3501 MHz  350724249 s          0 s    9635612 s  3447193375 s         13 s
       #3  3501 MHz   73800804 s          0 s    8480426 s  3725661602 s         73 s
       #4  3501 MHz   70488798 s          0 s    8667809 s  3728775733 s         17 s
       
  Memory: 31.383651733398438 GB (3407.828125 MB free)
  Uptime: 3.8097744e7 sec
  Load Avg:  1.0029296875  1.12060546875  1.44921875
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1324
Commit 55ab3e8 (2017-08-11 11:01 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   84655256 s          0 s   15209302 s  3698969202 s         87 s
       #2  3501 MHz  350869630 s          0 s    9646080 s  3447232156 s         13 s
       #3  3501 MHz   73881548 s          0 s    8487648 s  3725768062 s         73 s
       #4  3501 MHz   70564866 s          0 s    8674966 s  3728887116 s         17 s
       
  Memory: 31.383651733398438 GB (3305.25390625 MB free)
  Uptime: 3.8099694e7 sec
  Load Avg:  1.00439453125  1.13037109375  1.61865234375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
