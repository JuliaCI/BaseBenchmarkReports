# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@825cb515c6cb38478110c1815448ad5de5935a55](https://github.com/JuliaLang/julia/commit/825cb515c6cb38478110c1815448ad5de5935a55) vs [JuliaLang/julia@6014e7d9ef4d540b645c9b0ddd05f2998a03b31c](https://github.com/JuliaLang/julia/commit/6014e7d9ef4d540b645c9b0ddd05f2998a03b31c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27974#issuecomment-403191497)

*Tag Predicate:* `"problem"`

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
| `["problem", "imdb", "centrality"]` | 1.03 (15%)  | 0.98 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["problem", "chaosgame"]`
- `["problem", "fem"]`
- `["problem", "go"]`
- `["problem", "grigoriadis khachiyan"]`
- `["problem", "imdb"]`
- `["problem", "json"]`
- `["problem", "laplacian"]`
- `["problem", "monte carlo"]`
- `["problem", "raytrace"]`
- `["problem", "seismic"]`
- `["problem", "simplex"]`
- `["problem", "spellcheck"]`
- `["problem", "stockcorr"]`
- `["problem", "ziggurat"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta.191
Commit 825cb51 (2018-07-07 02:39 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   23324236 s        259 s    3273912 s  848372657 s          6 s
       #2  3501 MHz  114897652 s          0 s    1825415 s  759940321 s          6 s
       #3  3501 MHz   17433516 s       2392 s    1900007 s  857500375 s         13 s
       #4  3501 MHz   16717596 s          4 s    1498982 s  859028695 s          7 s
       
  Memory: 31.383651733398438 GB (4416.0078125 MB free)
  Uptime: 8.77639e6 sec
  Load Avg:  1.0029296875  1.22119140625  1.6865234375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.189
Commit 6014e7d (2018-07-07 02:38 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   23427836 s        259 s    3282239 s  848477869 s          6 s
       #2  3501 MHz  115038944 s          0 s    1833106 s  760008678 s          6 s
       #3  3501 MHz   17568224 s       2392 s    1908445 s  857574404 s         13 s
       #4  3501 MHz   16824805 s          4 s    1506538 s  859131269 s          7 s
       
  Memory: 31.383651733398438 GB (4330.8828125 MB free)
  Uptime: 8.778569e6 sec
  Load Avg:  1.05078125  1.2373046875  1.83349609375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
