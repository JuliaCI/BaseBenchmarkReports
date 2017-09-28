# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@db40843478a8f3ec109074f182264dd06ca30c15](https://github.com/JuliaLang/julia/commit/db40843478a8f3ec109074f182264dd06ca30c15) vs [JuliaLang/julia@d1b6f78097aa0a948848f334ffb01fb59dedd4a3](https://github.com/JuliaLang/julia/commit/d1b6f78097aa0a948848f334ffb01fb59dedd4a3)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23912#issuecomment-332867645)

*Tag Predicate:* `ALL`

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
| `["broadcast","typeargs",("tuple",5)]` | 1.38 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","string","DateTime"]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io","serialization",("serialize","Vector{String}")]` | 0.34 (15%) :white_check_mark: | 0.44 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",1024)]` | 0.96 (15%)  | 0.90 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.97 (15%)  | 0.84 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 0.97 (15%)  | 0.95 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.97 (15%)  | 0.89 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.96 (15%)  | 0.85 (1%) :white_check_mark: |
| `["problem","stockcorr","stockcorr"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"")]` | 0.46 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"",100)]` | 0.43 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.04 (25%)  | 0.98 (1%) :white_check_mark: |
| `["scalar","acos",("one","negative argument","Float64")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","acos",("one","positive argument","Float64")]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","negative argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.975 <= abs(x) < 1.0","positive argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 0.81 (15%) :white_check_mark: | 0.54 (1%) :white_check_mark: |
| `["shootout","regex_dna"]` | 0.88 (15%)  | 0.77 (1%) :white_check_mark: |
| `["sparse","transpose",("adjoint!",(20000,20000))]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["string","readuntil","backtracking"]` | 1.00 (15%)  | 0.07 (1%) :white_check_mark: |
| `["string","readuntil","barbarian backtrack"]` | 0.97 (15%)  | 0.04 (1%) :white_check_mark: |
| `["string","readuntil","no backtracking"]` | 0.97 (15%)  | 0.05 (1%) :white_check_mark: |
| `["string","readuntil","target length 1000"]` | 0.40 (15%) :white_check_mark: | 0.62 (1%) :white_check_mark: |
| `["string","readuntil","target length 2"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["string","readuntil","target length 50000"]` | 0.28 (15%) :white_check_mark: | 0.23 (1%) :white_check_mark: |
| `["string","replace"]` | 0.50 (15%) :white_check_mark: | 0.07 (1%) :white_check_mark: |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","convert"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reductions"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["broadcast","dotop"]`
- `["broadcast","fusion"]`
- `["broadcast","mix_scalar_tuple"]`
- `["broadcast","sparse"]`
- `["broadcast","typeargs"]`
- `["dates","accessor"]`
- `["dates","arithmetic"]`
- `["dates","construction"]`
- `["dates","conversion"]`
- `["dates","parse"]`
- `["dates","query"]`
- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["misc","afoldl"]`
- `["misc","bitshift"]`
- `["misc","julia"]`
- `["misc","parse"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["nullable","basic"]`
- `["nullable","nullablearray"]`
- `["parallel","remotecall"]`
- `["problem","chaosgame"]`
- `["problem","fem"]`
- `["problem","go"]`
- `["problem","grigoriadis khachiyan"]`
- `["problem","imdb"]`
- `["problem","json"]`
- `["problem","laplacian"]`
- `["problem","monte carlo"]`
- `["problem","raytrace"]`
- `["problem","seismic"]`
- `["problem","simplex"]`
- `["problem","spellcheck"]`
- `["problem","stockcorr"]`
- `["problem","ziggurat"]`
- `["random","collections"]`
- `["random","randstring"]`
- `["random","ranges"]`
- `["random","sequences"]`
- `["random","types"]`
- `["scalar","acos"]`
- `["scalar","arithmetic"]`
- `["scalar","asin"]`
- `["scalar","atan"]`
- `["scalar","cos"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","intfuncs"]`
- `["scalar","iteration"]`
- `["scalar","mod2pi"]`
- `["scalar","predicate"]`
- `["scalar","rem_pio2"]`
- `["scalar","sin"]`
- `["scalar","tan"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","constructors"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["string","readuntil"]`
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1988
Commit db40843 (2017-09-28 15:01 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   95270642 s          0 s   16914874 s  4101911345 s         92 s
       #2  3501 MHz  408404650 s          0 s   10901530 s  3804745355 s         20 s
       #3  3501 MHz   82498854 s          0 s    9372671 s  4132593719 s         76 s
       #4  3501 MHz   78851257 s          0 s    9560852 s  4136059147 s         18 s
       
  Memory: 31.383651733398438 GB (3219.69140625 MB free)
  Uptime: 4.2264927e7 sec
  Load Avg:  0.9228515625  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1985
Commit d1b6f78 (2017-09-28 14:59 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   95350046 s          0 s   16924005 s  4102469411 s         92 s
       #2  3501 MHz  409010875 s          0 s   10912981 s  3804776168 s         20 s
       #3  3501 MHz   82576247 s          0 s    9380423 s  4133156911 s         76 s
       #4  3501 MHz   78930528 s          0 s    9568276 s  4136620951 s         18 s
       
  Memory: 31.383651733398438 GB (3018.234375 MB free)
  Uptime: 4.2271417e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
