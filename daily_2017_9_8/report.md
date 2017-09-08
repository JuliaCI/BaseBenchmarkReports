# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@bc12af5e28aa633b5e0adb004b619635a98f2721](https://github.com/JuliaLang/julia/commit/bc12af5e28aa633b5e0adb004b619635a98f2721)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/bc12af5e28aa633b5e0adb004b619635a98f2721#commitcomment-24162683)

*Tag Predicate:* `ALL`

*Daily Job:* 2017-09-08 vs 2017-09-05

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
| `["array","growth",("append!",256)]` | 0.97 (15%)  | 1.04 (1%) :x: |
| `["array","growth",("prerend!",2048)]` | 1.00 (15%)  | 1.11 (1%) :x: |
| `["array","growth",("prerend!",256)]` | 0.98 (15%)  | 1.03 (1%) :x: |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.91 (50%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",100)]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 1.32 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 1.43 (15%) :x: | 1.00 (1%)  |
| `["dates","string","DateTime"]` | 2.45 (15%) :x: | 1.11 (1%) :x: |
| `["io","serialization",("serialize","Vector{String}")]` | 3.92 (15%) :x: | 2.50 (1%) :x: |
| `["nullable","basic",("get1","Nullable{BigFloat}(1.0)")]` | 0.10 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{BigFloat}(1.0)")]` | 0.14 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(0.0)")]` | 0.12 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}(1.0)")]` | 0.12 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}(1.0)","Nullable{BigFloat}()")]` | 0.10 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}(1.0)","Nullable{BigFloat}(1.0)")]` | 0.38 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{BigFloat}(1.0)")]` | 0.09 (60%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.07 (15%)  | 1.11 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.07 (15%)  | 1.16 (1%) :x: |
| `["parallel","remotecall",("identity",4096)]` | 1.05 (15%)  | 1.05 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 1.08 (15%)  | 1.11 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.09 (15%)  | 1.16 (1%) :x: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"")]` | 3.20 (25%) :x: | 1.00 (1%)  |
| `["random","randstring",("randstring","MersenneTwister","\"qwèrtï\"",100)]` | 3.68 (25%) :x: | 1.00 (1%)  |
| `["random","types",("rand","MersenneTwister","Int32")]` | 0.81 (25%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigInt}")]` | 1.02 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Int64}")]` | 1.00 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{UInt64}")]` | 1.00 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigInt}")]` | 1.00 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigInt}")]` | 1.00 (50%)  | 0.94 (1%) :white_check_mark: |
| `["scalar","arithmetic",("rem type","BigInt","UInt64")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{BigInt}")]` | 0.98 (40%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","mod2pi",("argument reduction (easy) abs(x) < 5π/4","positive argument","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","mod2pi",("argument reduction (hard) abs(x) < 6π/4","positive argument","Float64")]` | 0.85 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float64")]` | 1.34 (25%) :x: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 2.53 (15%) :x: | 2.05 (1%) :x: |
| `["shootout","mandelbrot"]` | 1.00 (15%)  | 1.02 (1%) :x: |
| `["shootout","regex_dna"]` | 1.29 (15%) :x: | 1.37 (1%) :x: |
| `["sort","issorted",("forwards","descending")]` | 1.32 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["string","join"]` | 1.46 (40%) :x: | 1.01 (1%)  |
| `["string","replace"]` | 3.45 (15%) :x: | 17.04 (1%) :x: |
| `["tuple","reduction",("sum",(2,2))]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(2,2))]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sumabs",(4,))]` | 1.16 (15%) :x: | 1.00 (1%)  |

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
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["string","search"]`
- `["string","searchindex"]`
- `["tuple","index"]`
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.1712
Commit bc12af5 (2017-09-07 22:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   91539191 s          0 s   16262367 s  3930391123 s         92 s
       #2  3501 MHz  387844282 s          0 s   10459343 s  3649410810 s         17 s
       #3  3501 MHz   79657361 s          0 s    9058393 s  3959398738 s         75 s
       #4  3501 MHz   76152103 s          0 s    9251419 s  3962713752 s         17 s
       
  Memory: 31.383651733398438 GB (3065.609375 MB free)
  Uptime: 4.0500634e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
