# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@072dfc93bc00838ae37a01c48ece42f7f460cc68](https://github.com/JuliaLang/julia/commit/072dfc93bc00838ae37a01c48ece42f7f460cc68) vs [JuliaLang/julia@b0427fc1b44adf8069e23e5bbaba194148eda4e5](https://github.com/JuliaLang/julia/commit/b0427fc1b44adf8069e23e5bbaba194148eda4e5)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/30833#issuecomment-457805592)

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
Julia Version 1.2.0-DEV.220
Commit 072dfc9 (2019-01-26 06:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   43475741 s       2426 s    8389199 s  2571582613 s         12 s
       #2  3501 MHz  245179327 s         14 s    4383115 s  2379979244 s         18 s
       #3  3501 MHz   34497519 s       3143 s    3995949 s  2590893226 s         27 s
       #4  3501 MHz   33208946 s         14 s    3121476 s  2594193203 s         23 s
       
  Memory: 31.383651733398438 GB (5113.74609375 MB free)
  Uptime: 2.6316115e7 sec
  Load Avg:  1.001953125  1.2119140625  1.65576171875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.2.0-DEV.218
Commit b0427fc (2019-01-25 21:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   43598327 s       2426 s    8396843 s  2571675458 s         12 s
       #2  3501 MHz  245336128 s         14 s    4390512 s  2380038364 s         18 s
       #3  3501 MHz   34618690 s       3143 s    4003228 s  2590987812 s         27 s
       #4  3501 MHz   33318896 s         14 s    3128896 s  2594299105 s         23 s
       
  Memory: 31.383651733398438 GB (4999.78125 MB free)
  Uptime: 2.6318353e7 sec
  Load Avg:  0.9970703125  1.2021484375  1.79736328125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
