# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@af60994dbfc717e21f849c0267bd18c6c2c98826](https://github.com/JuliaLang/julia/commit/af60994dbfc717e21f849c0267bd18c6c2c98826) vs [JuliaLang/julia@9b2a1cca2388c9fba78360b3d2c0a35e1446a308](https://github.com/JuliaLang/julia/commit/9b2a1cca2388c9fba78360b3d2c0a35e1446a308)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23117#issuecomment-320100959)

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
| `["array","cat",("catnd",5)]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat",5)]` | 0.36 (15%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 0.33 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.24 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","splatting",(3,3,3)]` | 0.03 (15%) :white_check_mark: | 0.25 (1%) :white_check_mark: |
| `["nullable","nullablearray",("perf_sum","Array","Int8")]` | 2.69 (50%) :x: | 1.00 (1%)  |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["problem","imdb","centrality"]` | 1.04 (15%)  | 0.98 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["problem","ziggurat","ziggurat"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:1)")]` | 1.02 (25%)  | 0.99 (1%) :white_check_mark: |
| `["random","ranges",("rand","MersenneTwister","BigInt","RangeGenerator(1:4294967297)")]` | 1.06 (25%)  | 1.02 (1%) :x: |
| `["random","types",("rand","RandomDevice","Float64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("rand","RandomDevice","Int64")]` | 0.69 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("randn","ImplicitRNG","Float64")]` | 0.75 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("randn","MersenneTwister","Complex{Float32}")]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("randn","MersenneTwister","Complex{Float64}")]` | 0.53 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("randn","MersenneTwister","Float64")]` | 2.30 (25%) :x: | 1.00 (1%)  |
| `["random","types",("randn","RandomDevice","Float64")]` | 0.74 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","BigInt","BigInt")]` | 0.60 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","BigInt","Bool")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","BigInt","Int64")]` | 1.48 (40%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","BigInt","UInt64")]` | 0.57 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","Bool","Int64")]` | 1.60 (40%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","Int64","Int64")]` | 0.54 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("rem type","UInt64","UInt64")]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","cos",("argument reduction (easy) abs(x) < 2.0^20π/4","positive argument","Float64","cos_kernel")]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 0.69 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.47 (30%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |

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
- `["scalar","arithmetic"]`
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
Julia Version 0.7.0-DEV.1228
Commit af60994 (2017-08-03 21:53 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   82271395 s          0 s   14876483 s  3636937324 s         86 s
       #2  3501 MHz  336633629 s          0 s    9313625 s  3396900362 s         13 s
       #3  3501 MHz   71447284 s          0 s    8252276 s  3663536003 s         73 s
       #4  3501 MHz   68163747 s          0 s    8443071 s  3666612264 s         17 s
       
  Memory: 31.383651733398438 GB (3147.3828125 MB free)
  Uptime: 3.7450276e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1226
Commit 9b2a1cc (2017-08-03 21:52 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   82350232 s          0 s   14885170 s  3637437900 s         86 s
       #2  3501 MHz  337174250 s          0 s    9324821 s  3396938214 s         13 s
       #3  3501 MHz   71523924 s          0 s    8259510 s  3664041654 s         73 s
       #4  3501 MHz   68246524 s          0 s    8450078 s  3667112241 s         17 s
       
  Memory: 31.383651733398438 GB (2860.453125 MB free)
  Uptime: 3.7456179e7 sec
  Load Avg:  1.0830078125  1.03125  1.05078125
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
