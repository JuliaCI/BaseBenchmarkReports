# Benchmark Report

## Job Properties

*Commit(s):* [jlapeyre/julia@b253d39c855e9128f20f9fc151cf4b8413ac4934](https://github.com/jlapeyre/julia/commit/b253d39c855e9128f20f9fc151cf4b8413ac4934) vs [JuliaLang/julia@a57250432abfafcc3b3ffa9df26e79516d1f6160](https://github.com/JuliaLang/julia/commit/a57250432abfafcc3b3ffa9df26e79516d1f6160)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/28654#issuecomment-419610217)

*Tag Predicate:* `"sparse"`

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
| `["problem", "laplacian", "laplace_iter_sub"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_iter_vec"]` | 1.08 (5%) :x: | 1.00 (1%)  |
| `["problem", "laplacian", "laplace_sparse_matvec"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 10)"]` | 0.94 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"Bidiagonal\", 100)"]` | 1.15 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IJV\", 100)"]` | 0.90 (5%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"IV\", 10)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["sparse", "constructors", "(\"SymTridiagonal\", 100)"]` | 1.11 (5%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"col\", \"OneTo\", 100)"]` | 1.11 (30%)  | 1.04 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"col\", \"range\", 10)"]` | 1.09 (30%)  | 1.09 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"OneTo\", 10)"]` | 1.09 (30%)  | 1.06 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"range\", 1000)"]` | 1.26 (30%)  | 1.01 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["broadcast", "sparse"]`
- `["problem", "fem"]`
- `["problem", "laplacian"]`
- `["sparse", "arithmetic"]`
- `["sparse", "constructors"]`
- `["sparse", "index"]`
- `["sparse", "matmul"]`
- `["sparse", "transpose"]`

## Version Info

#### Primary Build

```
Julia Version 1.1.0-DEV.214
Commit b253d39 (2018-09-08 03:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   30945807 s       2407 s    4435749 s  1384199010 s          8 s
       #2  3501 MHz  142256705 s          4 s    2620395 s  1277548056 s         13 s
       #3  3501 MHz   22305892 s       3126 s    2759202 s  1397337550 s         20 s
       #4  3501 MHz   21352229 s         11 s    2163146 s  1399514496 s         12 s
       
  Memory: 31.383651733398438 GB (3704.50390625 MB free)
  Uptime: 1.4237615e7 sec
  Load Avg:  0.9970703125  1.0146484375  1.22216796875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.1.0-DEV.210
Commit a572504 (2018-09-08 03:48 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   31068451 s       2407 s    4443279 s  1384397547 s          8 s
       #2  3501 MHz  142504098 s          4 s    2627813 s  1277622555 s         13 s
       #3  3501 MHz   22428022 s       3126 s    2766808 s  1397537003 s         20 s
       #4  3501 MHz   21460889 s         11 s    2170224 s  1399728167 s         12 s
       
  Memory: 31.383651733398438 GB (5347.08984375 MB free)
  Uptime: 1.4240915e7 sec
  Load Avg:  0.9970703125  1.0146484375  1.2470703125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
