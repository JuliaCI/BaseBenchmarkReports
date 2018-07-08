# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@330d857bcf4a9791d7910b49dc843b52a09daab4](https://github.com/JuliaLang/julia/commit/330d857bcf4a9791d7910b49dc843b52a09daab4) vs [JuliaLang/julia@2245a04feecfe66e6fbcf6e05fa5b2883773e4b5](https://github.com/JuliaLang/julia/commit/2245a04feecfe66e6fbcf6e05fa5b2883773e4b5)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27945#issuecomment-403255562)

*Tag Predicate:* `"sumcolon_view" || ("sumrange_view" || "seismic")`

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
| `["array", "index", "(\"sumcolon_view\", \"Array{Float32,2}\")"]` | 6.77 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumcolon_view\", \"Array{Int32,2}\")"]` | 9.33 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumrange_view\", \"Array{Float32,2}\")"]` | 1.00 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array", "index", "(\"sumrange_view\", \"Array{Int32,2}\")"]` | 0.96 (50%)  | 0.00 (1%) :white_check_mark: |
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 2.71 (15%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 2.25 (15%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array", "index"]`
- `["problem", "seismic"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta.207
Commit 330d857 (2018-07-08 01:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   23547933 s        259 s    3294420 s  855242278 s          6 s
       #2  3501 MHz  115171145 s          0 s    1842752 s  766775611 s          7 s
       #3  3501 MHz   17675627 s       2392 s    1933071 s  864338768 s         13 s
       #4  3501 MHz   16942281 s          4 s    1516078 s  865911918 s          7 s
       
  Memory: 31.383651733398438 GB (4276.85546875 MB free)
  Uptime: 8.84769e6 sec
  Load Avg:  1.0029296875  1.3115234375  1.76123046875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.204
Commit 2245a04 (2018-07-08 01:49 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   23655730 s        259 s    3302405 s  855333293 s          6 s
       #2  3501 MHz  115310410 s          0 s    1850864 s  766835156 s          7 s
       #3  3501 MHz   17786391 s       2392 s    1941316 s  864426468 s         13 s
       #4  3501 MHz   17062272 s          4 s    1523912 s  865990984 s          7 s
       
  Memory: 31.383651733398438 GB (4238.74609375 MB free)
  Uptime: 8.849765e6 sec
  Load Avg:  0.9228515625  1.2939453125  1.919921875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
