# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a398e83e741d8773bdcafecbc1679d0d987e75b7](https://github.com/JuliaLang/julia/commit/a398e83e741d8773bdcafecbc1679d0d987e75b7) vs [JuliaLang/julia@f90d6740575b45490fab4aa218ac07f9af2431b2](https://github.com/JuliaLang/julia/commit/f90d6740575b45490fab4aa218ac07f9af2431b2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27685#issuecomment-399048012)

*Tag Predicate:* `"shootout" || ("string" || "problem")`

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
| `["problem", "imdb", "centrality"]` | 0.46 (15%) :white_check_mark: | 0.39 (1%) :white_check_mark: |
| `["problem", "spellcheck", "spellcheck"]` | 0.52 (15%) :white_check_mark: | 0.79 (1%) :white_check_mark: |
| `["shootout", "k_nucleotide"]` | 0.43 (15%) :white_check_mark: | 0.44 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates", "string"]`
- `["io", "read"]`
- `["io", "serialization"]`
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
- `["shootout"]`
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-alpha.219
Commit a398e83 (2018-06-21 10:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   32069715 s        277 s    3394716 s  703266991 s          6 s
       #2  3501 MHz  140946994 s          0 s    1966158 s  597722115 s          4 s
       #3  3501 MHz   18890896 s       2375 s    1586991 s  719830846 s         10 s
       #4  3501 MHz   17645900 s          0 s    1858508 s  720944447 s          7 s
       
  Memory: 31.383651733398438 GB (3960.38671875 MB free)
  Uptime: 7.410593e6 sec
  Load Avg:  0.9970703125  1.0146484375  1.0966796875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-alpha.217
Commit f90d674 (2018-06-21 10:01 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   32185034 s        277 s    3404500 s  703563887 s          6 s
       #2  3501 MHz  141306695 s          0 s    1975060 s  597776428 s          4 s
       #3  3501 MHz   19011512 s       2375 s    1596082 s  720123720 s         10 s
       #4  3501 MHz   17757529 s          0 s    1867311 s  721246623 s          7 s
       
  Memory: 31.383651733398438 GB (3867.71875 MB free)
  Uptime: 7.414827e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.107421875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
