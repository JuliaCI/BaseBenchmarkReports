# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@b33286e62bbbf743909755bb7aa8b1fb85594f45](https://github.com/JuliaLang/julia/commit/b33286e62bbbf743909755bb7aa8b1fb85594f45)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23582#issuecomment-327040286)

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

| ID | time | GC time | memory | allocations |
|----|------|---------|--------|-------------|
| `["dates","string","Date"]` | 231.530 ns (15%) | 0.000 ns | 384 bytes (1%) | 9 |
| `["dates","string","DateTime"]` | 582.010 ns (15%) | 0.000 ns | 1.02 KiB (1%) | 19 |
| `["io","read","read"]` | 8.835 μs (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["io","read","readstring"]` | 35.060 ns (15%) | 0.000 ns | 96 bytes (1%) | 2 |
| `["io","serialization",("deserialize","Matrix{Float64}")]` | 661.956 μs (15%) | 0.000 ns | 7.63 MiB (1%) | 25 |
| `["io","serialization",("deserialize","Vector{String}")]` | 123.828 μs (15%) | 0.000 ns | 122.34 KiB (1%) | 2995 |
| `["io","serialization",("serialize","Matrix{Float64}")]` | 4.199 ms (15%) | 0.000 ns | 7.63 MiB (1%) | 11 |
| `["io","serialization",("serialize","Vector{String}")]` | 63.136 μs (15%) | 0.000 ns | 71.58 KiB (1%) | 21 |
| `["problem","spellcheck","spellcheck"]` | 5.357 s (15%) | 802.517 ms | 2.26 GiB (1%) | 46575484 |
| `["string","join"]` | 193.335 ms (40%) | 35.583 ms | 156.27 MiB (1%) | 21 |
| `["string","replace"]` | 121.244 μs (15%) | 0.000 ns | 12.06 KiB (1%) | 6 |
| `["string","search","Char"]` | 12.234 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["string","search","String"]` | 18.965 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["string","searchindex","Char"]` | 12.164 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |
| `["string","searchindex","String"]` | 16.935 ns (15%) | 0.000 ns | 0 bytes (1%) | 0 |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["problem","spellcheck"]`
- `["string"]`
- `["string","search"]`
- `["string","searchindex"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1640
Commit b33286e (2017-09-04 23:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   84583163 s          0 s   12945750 s  3915286849 s        158 s
       #2  3501 MHz  342248500 s          0 s   14120316 s  3658148722 s         54 s
       #3  3501 MHz   71557469 s          0 s    8186955 s  3940156924 s         74 s
       #4  3501 MHz   66860842 s          0 s    8058171 s  3945389115 s         26 s
       
  Memory: 31.383651733398438 GB (2168.02734375 MB free)
  Uptime: 4.0216794e7 sec
  Load Avg:  0.9970703125  1.47412109375  1.70751953125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
