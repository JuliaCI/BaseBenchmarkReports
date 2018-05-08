# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@36607e9f991bd87d189094345effc6df5ddd2a37](https://github.com/JuliaLang/julia/commit/36607e9f991bd87d189094345effc6df5ddd2a37) vs [JuliaLang/julia@a6759a15e93edd324ff4dda93327d25898791451](https://github.com/JuliaLang/julia/commit/a6759a15e93edd324ff4dda93327d25898791451)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27030#issuecomment-387557331)

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
| `["problem", "chaosgame", "chaosgame"]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "go", "go_game"]` | 0.75 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["problem", "grigoriadis khachiyan", "grigoriadis_khachiyan"]` | 1.83 (15%) :x: | 1.76 (1%) :x: |
| `["problem", "imdb", "centrality"]` | 1.11 (15%)  | 1.33 (1%) :x: |
| `["problem", "json", "parse_json"]` | 3.08 (15%) :x: | 3.70 (1%) :x: |
| `["problem", "laplacian", "laplace_iter_sub"]` | 3.00 (15%) :x: | 3829.61 (1%) :x: |
| `["problem", "laplacian", "laplace_sparse_matvec"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["problem", "raytrace", "raytrace"]` | 1.46 (15%) :x: | 0.73 (1%) :white_check_mark: |
| `["problem", "seismic", "(\"seismic\", \"Float32\")"]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "simplex", "simplex"]` | 0.94 (15%)  | 0.77 (1%) :white_check_mark: |
| `["problem", "spellcheck", "spellcheck"]` | 2.82 (15%) :x: | 2.41 (1%) :x: |
| `["problem", "ziggurat", "ziggurat"]` | 2.26 (15%) :x: | 2.84 (1%) :x: |

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
Julia Version 0.7.0-DEV-Wut.3
Commit 36607e9 (2018-05-08 15:22 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   10842393 s        264 s    1325703 s  351946781 s          4 s
       #2  3501 MHz   66748606 s          0 s     964264 s  297064081 s          1 s
       #3  3501 MHz    8115944 s       2371 s     771401 s  355590186 s          6 s
       #4  3501 MHz    7825380 s          0 s     937798 s  355910917 s          1 s
       
  Memory: 31.383651733398438 GB (6059.33984375 MB free)
  Uptime: 3.650301e6 sec
  Load Avg:  0.9970703125  1.2109375  1.7138671875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.3-pre.36
Commit a6759a1 (2018-05-08 20:10 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (6575.38671875 MB free)
Uptime: 3.651989e6 sec
Load Avg:  1.0029296875  1.4990234375  2.06005859375
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   10937764 s        264 s    1334231 s  352010899 s          4 s
#2  3501 MHz   66860357 s          0 s     973302 s  297111579 s          1 s
#3  3501 MHz    8208096 s       2371 s     779903 s  355657508 s          6 s
#4  3501 MHz    7911788 s          0 s     946160 s  355984282 s          1 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
