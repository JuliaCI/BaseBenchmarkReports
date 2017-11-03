# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@28c4e020fe99c5a2b647173a7681900b9257743e](https://github.com/JuliaLang/julia/commit/28c4e020fe99c5a2b647173a7681900b9257743e) vs [JuliaLang/julia@c7d639186461becce64de1a1905d51108d9c2852](https://github.com/JuliaLang/julia/commit/c7d639186461becce64de1a1905d51108d9c2852)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24406#issuecomment-341620625)

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
| `["problem", "json", "parse_json"]` | 0.08 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_sparse_matvec"]` | 0.62 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem", "stockcorr", "stockcorr"]` | 1.19 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.2412
Commit 28c4e02 (2017-11-02 21:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   92076428 s          0 s   14304704 s  4416577984 s        197 s
       #2  3501 MHz  366074916 s          0 s   15407075 s  4143669121 s         69 s
       #3  3501 MHz   75637274 s          0 s    8636388 s  4446967597 s         89 s
       #4  3501 MHz   70850458 s          0 s    8495156 s  4452307158 s         35 s
       
  Memory: 31.383651733398438 GB (12432.48046875 MB free)
  Uptime: 4.5331247e7 sec
  Load Avg:  0.9228515625  1.4375  1.720703125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2413
Commit c7d6391 (2017-11-02 21:30 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   92162898 s          0 s   14312645 s  4416646896 s        197 s
       #2  3501 MHz  366179508 s          0 s   15414924 s  4143720017 s         69 s
       #3  3501 MHz   75723218 s          0 s    8644046 s  4447037230 s         89 s
       #4  3501 MHz   70950463 s          0 s    8503190 s  4452362529 s         35 s
       
  Memory: 31.383651733398438 GB (12457.59765625 MB free)
  Uptime: 4.5332887e7 sec
  Load Avg:  1.0029296875  1.490234375  2.0205078125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
