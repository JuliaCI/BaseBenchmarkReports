# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d360782f31321c2295291e017df1826839eeed3e](https://github.com/JuliaLang/julia/commit/d360782f31321c2295291e017df1826839eeed3e) vs [JuliaLang/julia@b21d39d7399338852113faf362061f7257103fd0](https://github.com/JuliaLang/julia/commit/b21d39d7399338852113faf362061f7257103fd0)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/32102#issuecomment-494476989)

*Tag Predicate:* `"linalg"`

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
| `["linalg", "arithmetic", "(\"sqrt\", \"NPDUpperTriangular\", 1024)"]` | 1.64 (45%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"svd\", \"Diagonal\", 1024)"]` | 1.00 (45%)  | 1.02 (1%) :x: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["linalg"]`

## Version Info

#### Primary Build

```
Julia Version 1.2.0-pre.61
Commit d360782 (2019-05-21 15:44 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   48159002 s       2434 s   11218618 s  3558474111 s         13 s
       #2  3501 MHz  282765563 s         20 s    5103697 s  3338667573 s         19 s
       #3  3501 MHz   39189918 s       3171 s    4769316 s  3582526965 s         30 s
       #4  3501 MHz   37804020 s         15 s    3573072 s  3586595914 s         26 s
       
  Memory: 31.383651733398438 GB (5100.15625 MB free)
  Uptime: 3.6292511e7 sec
  Load Avg:  0.9228515625  1.02587890625  1.33203125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.3.0-DEV.261
Commit b21d39d (2019-05-21 16:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   48266747 s       2434 s   11223379 s  3558606907 s         13 s
       #2  3501 MHz  282949328 s         20 s    5108410 s  3338724767 s         19 s
       #3  3501 MHz   39284912 s       3171 s    4773912 s  3582672889 s         30 s
       #4  3501 MHz   37911241 s         15 s    3577459 s  3586729949 s         26 s
       
  Memory: 31.383651733398438 GB (5105.37890625 MB free)
  Uptime: 3.629497e7 sec
  Load Avg:  0.9970703125  1.04052734375  1.42626953125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
