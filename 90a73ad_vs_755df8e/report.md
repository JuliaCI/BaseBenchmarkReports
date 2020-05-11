# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@90a73ad4d6433a17f7708300bc3221d2be1e1190](https://github.com/JuliaLang/julia/commit/90a73ad4d6433a17f7708300bc3221d2be1e1190) vs [JuliaLang/julia@755df8e43e84ec858900e5adaf88c3eaca766043](https://github.com/JuliaLang/julia/commit/755df8e43e84ec858900e5adaf88c3eaca766043)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/35838#issuecomment-626662890)

*Tag Predicate:* `"string"`

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
| `["dates", "string", "DateTime"]` | 0.93 (5%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates", "string"]`
- `["io", "read"]`
- `["io", "serialization"]`
- `["problem", "spellcheck"]`
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`
- `["string", "repeat"]`

## Version Info

#### Primary Build

```
Julia Version 1.6.0-DEV.16
Commit 90a73ad (2020-05-11 12:09 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   57611064 s       2449 s   20327496 s  6603444587 s         19 s
       #2  3501 MHz  361310645 s         62 s    7596400 s  6330538117 s         27 s
       #3  3501 MHz   48745970 s       3236 s    5780947 s  6642970657 s         40 s
       #4  3501 MHz   46952421 s         19 s    4464836 s  6650112246 s         37 s
       
  Memory: 31.383651733398438 GB (18790.7265625 MB free)
  Uptime: 6.7033819e7 sec
  Load Avg:  0.9970703125  1.19970703125  1.72607421875
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 1.6.0-DEV.14
Commit 755df8e (2020-05-11 10:31 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.5 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   57776224 s       2449 s   20333740 s  6603532726 s         19 s
       #2  3501 MHz  361474807 s         62 s    7603180 s  6330626967 s         27 s
       #3  3501 MHz   48896143 s       3236 s    5787173 s  6643073809 s         40 s
       #4  3501 MHz   47097722 s         19 s    4470625 s  6650220944 s         37 s
       
  Memory: 31.383651733398438 GB (18736.4375 MB free)
  Uptime: 6.703642e7 sec
  Load Avg:  1.05908203125  1.2529296875  1.8447265625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-9.0.1 (ORCJIT, haswell)

```
