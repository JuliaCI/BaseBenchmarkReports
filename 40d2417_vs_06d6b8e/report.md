# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@40d2417efd2379213ab605b3844dfdf11db3fe5a](https://github.com/JuliaLang/julia/commit/40d2417efd2379213ab605b3844dfdf11db3fe5a) vs [JuliaLang/julia@06d6b8e291a1e7b074487c9f738a0c29642dfb62](https://github.com/JuliaLang/julia/commit/06d6b8e291a1e7b074487c9f738a0c29642dfb62)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/33434#issuecomment-537131315)

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
| `["linalg", "factorization", "(\"eigen\", \"Diagonal\", 256)"]` | 0.45 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg", "small exp #29116"]` | 0.95 (5%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["linalg"]`

## Version Info

#### Primary Build

```
Julia Version 1.4.0-DEV.224
Commit 40d2417 (2019-10-01 16:01 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  102803762 s       5044 s   11949399 s  4652672349 s         28 s
       #2  3501 MHz  709364992 s        212 s   12537101 s  4052912504 s         24 s
       #3  3501 MHz   86410494 s       3254 s    7087815 s  4681438016 s         33 s
       #4  3501 MHz   81062354 s         27 s   10087768 s  4681854351 s         22 s
       
  Memory: 31.383651733398438 GB (14294.0625 MB free)
  Uptime: 4.7783972e7 sec
  Load Avg:  0.9228515625  1.0244140625  1.306640625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.4.0-DEV.222
Commit 06d6b8e (2019-10-01 16:01 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  102915300 s       5044 s   11954305 s  4652807158 s         28 s
       #2  3501 MHz  709551460 s        212 s   12541918 s  4052972709 s         24 s
       #3  3501 MHz   86513740 s       3254 s    7092356 s  4681581589 s         33 s
       #4  3501 MHz   81158484 s         27 s   10092132 s  4682005311 s         22 s
       
  Memory: 31.383651733398438 GB (14265.3046875 MB free)
  Uptime: 4.778649e7 sec
  Load Avg:  1.25537109375  1.09423828125  1.4189453125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.1 (ORCJIT, haswell)

```
