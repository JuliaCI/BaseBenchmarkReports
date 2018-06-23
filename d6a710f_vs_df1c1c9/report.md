# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d6a710f60a4851b8030d559a8493bd693aa64a5c](https://github.com/JuliaLang/julia/commit/d6a710f60a4851b8030d559a8493bd693aa64a5c) vs [JuliaLang/julia@df1c1c939bf1c582cf040b5ad235933242aeacfb](https://github.com/JuliaLang/julia/commit/df1c1c939bf1c582cf040b5ad235933242aeacfb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27030#issuecomment-399679428)

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
| `["dates", "string", "DateTime"]` | 1.15 (15%) :x: | 0.97 (1%) :white_check_mark: |
| `["io", "serialization", "(\"deserialize\", \"Vector{String}\")"]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io", "serialization", "(\"serialize\", \"Matrix{Float64}\")"]` | 0.99 (15%)  | 0.95 (1%) :white_check_mark: |
| `["io", "serialization", "(\"serialize\", \"Vector{String}\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "chaosgame", "chaosgame"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "go", "go_game"]` | 0.70 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.55 (15%) :x: | 1.76 (1%) :x: |
| `["problem", "imdb", "centrality"]` | 1.00 (15%)  | 1.32 (1%) :x: |
| `["problem", "json", "parse_json"]` | 1.71 (15%) :x: | 2.63 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_sub"]` | 2.74 (15%) :x: | 3829.61 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_vec"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_devec"]` | 1.53 (15%) :x: | 1.00 (1%)  |
| `["problem", "monte carlo", "euro_option_vec"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 0.90 (15%)  | 0.73 (1%) :white_check_mark: |
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 1.73 (15%) :x: | 1.00 (1%)  |
| `["problem", "seismic", "(\"seismic\", \"Float64\")"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["problem", "simplex", "simplex"]` | 0.67 (15%) :white_check_mark: | 0.77 (1%) :white_check_mark: |
| `["problem", "spellcheck", "spellcheck"]` | 1.72 (15%) :x: | 2.20 (1%) :x: |
| `["problem", "ziggurat", "ziggurat"]` | 1.94 (15%) :x: | 2.83 (1%) :x: |
| `["shootout", "binary_trees"]` | 0.70 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["shootout", "mandelbrot"]` | 0.97 (15%)  | 1.05 (1%) :x: |
| `["shootout", "meteor_contest"]` | 0.61 (15%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["shootout", "nbody"]` | 0.66 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "nbody_vec"]` | 0.57 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout", "regex_dna"]` | 60.65 (15%) :x: | 1.00 (1%)  |
| `["shootout", "revcomp"]` | 1.65 (25%) :x: | 0.94 (1%) :white_check_mark: |
| `["shootout", "spectralnorm"]` | 1.00 (15%)  | 0.22 (1%) :white_check_mark: |
| `["string", "join"]` | 1.25 (40%)  | 1.22 (1%) :x: |
| `["string", "readuntil", "backtracking"]` | 0.00 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["string", "readuntil", "barbarian backtrack"]` | 0.01 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["string", "readuntil", "no backtracking"]` | 0.01 (15%) :white_check_mark: | 0.87 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 1"]` | 0.28 (15%) :white_check_mark: | 0.33 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 1000"]` | 0.07 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 2"]` | 0.23 (15%) :white_check_mark: | 0.23 (1%) :white_check_mark: |
| `["string", "readuntil", "target length 50000"]` | 0.10 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["string", "replace"]` | 1.18 (15%) :x: | 1.00 (1%)  |

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
- `["string"]`
- `["string", "readuntil"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-alpha-Wut.109
Commit d6a710f (2018-06-23 13:42 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   15897382 s        256 s    2538661 s  738907159 s          5 s
       #2  3501 MHz   80598662 s          0 s    1308463 s  676933738 s          5 s
       #3  3501 MHz   11724082 s       2389 s    1433374 s  745795847 s         11 s
       #4  3501 MHz   11369687 s          4 s    1075928 s  746875068 s          3 s
       
  Memory: 31.383651733398438 GB (3592.3203125 MB free)
  Uptime: 7.59653e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.099609375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.4-pre.7
Commit df1c1c9 (2018-06-19 17:36 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4046.03515625 MB free)
Uptime: 7.59831e6 sec
Load Avg:  0.9970703125  1.359375  1.861328125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   15980880 s        256 s    2547422 s  738991983 s          5 s
#2  3501 MHz   80716890 s          0 s    1317072 s  676984362 s          5 s
#3  3501 MHz   11827052 s       2389 s    1441970 s  745861745 s         11 s
#4  3501 MHz   11458622 s          4 s    1084458 s  746955046 s          4 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell MAX_THREADS=16)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
