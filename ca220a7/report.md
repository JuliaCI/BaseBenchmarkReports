# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ca220a7636ce19e387f54c641c47f77f3d0b659c](https://github.com/JuliaLang/julia/commit/ca220a7636ce19e387f54c641c47f77f3d0b659c)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25713#issuecomment-360613743)

*Tag Predicate:* `"String"`

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

| ID | time | GC time | memory | allocations |
|----|------|---------|--------|-------------|
| `["collection", "deletion", "(\"Dict\", \"String\", \"filter!\")"]` | 36.666 μs (25%) | 0.000 ns | 31.03 KiB (1%) | 993 |
| `["collection", "deletion", "(\"Dict\", \"String\", \"filter\")"]` | 55.524 μs (25%) | 0.000 ns | 55.03 KiB (1%) | 1006 |
| `["collection", "deletion", "(\"Dict\", \"String\", \"pop!\")"]` | 26.051 μs (25%) | 0.000 ns | 31.03 KiB (1%) | 993 |
| `["collection", "deletion", "(\"Set\", \"String\", \"filter!\")"]` | 27.378 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Set\", \"String\", \"filter\")"]` | 63.486 μs (25%) | 0.000 ns | 17.56 KiB (1%) | 289 |
| `["collection", "deletion", "(\"Set\", \"String\", \"pop!\")"]` | 21.860 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter!\")"]` | 6.775 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "deletion", "(\"Vector\", \"String\", \"filter\")"]` | 12.921 μs (25%) | 0.000 ns | 16.45 KiB (1%) | 10 |
| `["collection", "deletion", "(\"Vector\", \"String\", \"pop!\")"]` | 3.003 μs (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "initialization", "(\"Dict\", \"String\", \"iterator\")"]` | 69.981 μs (25%) | 0.000 ns | 92.34 KiB (1%) | 18 |
| `["collection", "initialization", "(\"Dict\", \"String\", \"loop\")"]` | 69.422 μs (25%) | 0.000 ns | 92.34 KiB (1%) | 18 |
| `["collection", "initialization", "(\"Dict\", \"String\", \"loop\", \"sizehint!\")"]` | 63.835 μs (25%) | 0.000 ns | 86.13 KiB (1%) | 12 |
| `["collection", "initialization", "(\"Set\", \"String\", \"iterator\")"]` | 92.470 μs (25%) | 0.000 ns | 63.30 KiB (1%) | 1122 |
| `["collection", "initialization", "(\"Set\", \"String\", \"loop\")"]` | 108.324 μs (25%) | 0.000 ns | 66.95 KiB (1%) | 1128 |
| `["collection", "initialization", "(\"Set\", \"String\", \"loop\", \"sizehint!\")"]` | 97.150 μs (25%) | 0.000 ns | 63.30 KiB (1%) | 1122 |
| `["collection", "initialization", "(\"Vector\", \"String\", \"iterator\")"]` | 1.956 μs (25%) | 0.000 ns | 7.94 KiB (1%) | 1 |
| `["collection", "initialization", "(\"Vector\", \"String\", \"loop\")"]` | 9.219 μs (25%) | 0.000 ns | 16.45 KiB (1%) | 10 |
| `["collection", "initialization", "(\"Vector\", \"String\", \"loop\", \"sizehint!\")"]` | 8.591 μs (25%) | 0.000 ns | 7.95 KiB (1%) | 2 |
| `["collection", "iteration", "(\"Dict\", \"String\", \"done\")"]` | 419.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"Dict\", \"String\", \"next\")"]` | 488.000 ns (25%) | 0.000 ns | 64 bytes (1%) | 2 |
| `["collection", "iteration", "(\"Dict\", \"String\", \"start\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"Set\", \"String\", \"done\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"Set\", \"String\", \"next\")"]` | 488.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["collection", "iteration", "(\"Set\", \"String\", \"start\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"Vector\", \"String\", \"done\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "iteration", "(\"Vector\", \"String\", \"next\")"]` | 488.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["collection", "iteration", "(\"Vector\", \"String\", \"start\")"]` | 419.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"getindex\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"in\", \"false\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"in\", \"true\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"pop!\", \"specified\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"pop!\", \"unspecified\")"]` | 488.000 ns (25%) | 0.000 ns | 32 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"push!\", \"new\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"push!\", \"overwrite\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"setindex!\", \"new\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"setindex!\", \"overwrite\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"in\", \"false\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"in\", \"true\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"pop!\", \"specified\")"]` | 558.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"pop!\", \"unspecified\")"]` | 558.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"push!\", \"new\")"]` | 489.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Set\", \"String\", \"push!\", \"overwrite\")"]` | 488.000 ns (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"getindex\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"false\")"]` | 1.466 μs (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"in\", \"true\")"]` | 1.676 μs (25%) | 0.000 ns | 16 bytes (1%) | 1 |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"pop!\", \"unspecified\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"push!\")"]` | 1.188 μs (25%) | 0.000 ns | 15.69 KiB (1%) | 1 |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"setindex!\")"]` | 488.000 ns (25%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["string", "search", "String"]` | 53.498 μs (15%) | 0.000 ns | 12.00 KiB (1%) | 114 |
| `["string", "searchindex", "String"]` | 54.755 μs (15%) | 0.000 ns | 12.00 KiB (1%) | 114 |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["collection", "deletion"]`
- `["collection", "initialization"]`
- `["collection", "iteration"]`
- `["collection", "queries & updates"]`
- `["string", "search"]`
- `["string", "searchindex"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.3578
Commit ca220a7 (2018-01-25 18:19 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz  105852567 s          0 s   16314515 s  5122531123 s        263 s
       #2  3501 MHz  414200911 s          0 s   17452647 s  4815682714 s         84 s
       #3  3501 MHz   83546680 s          0 s    9484404 s  5161436587 s        113 s
       #4  3501 MHz   78763906 s          0 s    9392049 s  5166747893 s         47 s
       
  Memory: 31.383651733398438 GB (3807.98046875 MB free)
  Uptime: 5.2565526e7 sec
  Load Avg:  0.9228515625  1.330078125  1.6767578125
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
