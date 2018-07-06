# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@45ad2df6116fcb782cc096adf20348a09a898792](https://github.com/JuliaLang/julia/commit/45ad2df6116fcb782cc096adf20348a09a898792) vs [JuliaLang/julia@6745e4fdcaad638271f930092c0c0db3de2e253f](https://github.com/JuliaLang/julia/commit/6745e4fdcaad638271f930092c0c0db3de2e253f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/27857#issuecomment-402911855)

*Tag Predicate:* `"collection" && "queries & updates"`

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
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"pop!\", \"unspecified\")"]` | 0.04 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Int\", \"pop!\", \"specified\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 0.04 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"push!\", \"overwrite\")"]` | 1.32 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Int\", \"pop!\", \"specified\")"]` | 1.39 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"Int\", \"pop!\", \"unspecified\")"]` | 1.67 (25%) :x: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["collection", "queries & updates"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-beta.158
Commit 45ad2df (2018-07-06 03:03 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   22636512 s        259 s    3207181 s  839448181 s          6 s
       #2  3501 MHz  111000911 s          0 s    1763653 s  754212084 s          6 s
       #3  3501 MHz   16696226 s       2392 s    1845630 s  848597099 s         13 s
       #4  3501 MHz   16040112 s          4 s    1446456 s  850061891 s          6 s
       
  Memory: 31.383651733398438 GB (3802.5390625 MB free)
  Uptime: 8.679349e6 sec
  Load Avg:  0.9970703125  1.23291015625  1.68896484375
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-beta.156
Commit 6745e4f (2018-07-06 02:21 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   22740984 s        259 s    3215351 s  839551184 s          6 s
       #2  3501 MHz  111137766 s          0 s    1771579 s  754283009 s          6 s
       #3  3501 MHz   16824195 s       2392 s    1853804 s  848676662 s         13 s
       #4  3501 MHz   16157255 s          4 s    1454285 s  850152859 s          6 s
       
  Memory: 31.383651733398438 GB (3742.765625 MB free)
  Uptime: 8.681513e6 sec
  Load Avg:  1.0029296875  1.23291015625  1.84814453125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
