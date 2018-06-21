# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@c2200218fbf57f4bbf813155840fe796cb2bcf40](https://github.com/JuliaLang/julia/commit/c2200218fbf57f4bbf813155840fe796cb2bcf40) vs [JuliaLang/julia@f90d6740575b45490fab4aa218ac07f9af2431b2](https://github.com/JuliaLang/julia/commit/f90d6740575b45490fab4aa218ac07f9af2431b2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27691#issuecomment-399047750)

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
| `["problem", "json", "parse_json"]` | 0.73 (15%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["problem", "spellcheck", "spellcheck"]` | 0.84 (15%) :white_check_mark: | 0.85 (1%) :white_check_mark: |

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
Commit c220021 (2018-06-21 10:02 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   14725424 s        256 s    2420176 s  721970770 s          5 s
       #2  3501 MHz   74826595 s          0 s    1203328 s  664527314 s          5 s
       #3  3501 MHz   10539222 s       2389 s    1335563 s  728799927 s         10 s
       #4  3501 MHz   10153692 s          4 s     984829 s  729897407 s          2 s
       
  Memory: 31.383651733398438 GB (2289.9765625 MB free)
  Uptime: 7.413559e6 sec
  Load Avg:  0.9228515625  0.998046875  1.1279296875
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
       #1  3501 MHz   14837288 s        256 s    2429460 s  722269972 s          5 s
       #2  3501 MHz   75162462 s          0 s    1212009 s  664603925 s          5 s
       #3  3501 MHz   10650762 s       2389 s    1344187 s  729100681 s         10 s
       #4  3501 MHz   10297985 s          4 s     993159 s  730166011 s          2 s
       
  Memory: 31.383651733398438 GB (2345.671875 MB free)
  Uptime: 7.417778e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.10595703125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
