# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@ebc427d3694fadf3ce0e43bd0ae593eb608463e8](https://github.com/pkofod/julia/commit/ebc427d3694fadf3ce0e43bd0ae593eb608463e8) vs [JuliaLang/julia@e89d150c9a1bd45fda40ddba58135aa3ac2f582d](https://github.com/JuliaLang/julia/commit/e89d150c9a1bd45fda40ddba58135aa3ac2f582d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23383#issuecomment-325187636)

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
| `["array","index","7d"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 1.51 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcolon_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.79 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.63 (50%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 1.20 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.18 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",1000)]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse",("Date","DateFormat")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["problem","laplacian","laplace_iter_vec"]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["problem","stockcorr","stockcorr"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["random","ranges",("RangeGenerator","UInt128","1:1")]` | 1.58 (25%) :x: | 1.00 (1%)  |
| `["random","types",("randexp!","MersenneTwister","Float16")]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("randn!","MersenneTwister","Float32")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random","types",("randn!","MersenneTwister","Float64")]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","asin",("0.5 <= abs(x) < 0.975","negative argument","Float32")]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("0 <= abs(x) < 7/16","negative argument","Float32")]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan",("0 <= abs(x) < 7/16","positive argument","Float32")]` | 1.23 (15%) :x: | 1.00 (1%)  |
| `["scalar","atan",("11/16 <= abs(x) < 19/16","negative argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("19/16 <= abs(x) < 39/16","negative argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("39/16 <= abs(x) < 2^66","negative argument","Float64")]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("39/16 <= abs(x) < 2^66","positive argument","Float64")]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","atan",("7/16 <= abs(x) < 11/16","negative argument","Float64")]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","logical",1000)]` | 1.55 (30%) :x: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(8,8))]` | 1.18 (15%) :x: | 1.00 (1%)  |

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
Julia Version 0.7.0-DEV.1522
Commit ebc427d (2017-08-27 08:42 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   83250280 s          0 s   12743153 s  3843301177 s        154 s
       #2  3501 MHz  337849872 s          0 s   13930468 s  3589144533 s         52 s
       #3  3501 MHz   70854427 s          0 s    8076547 s  3867299474 s         72 s
       #4  3501 MHz   66109250 s          0 s    7979682 s  3872528386 s         24 s
       
  Memory: 31.383651733398438 GB (4966.046875 MB free)
  Uptime: 3.9479761e7 sec
  Load Avg:  1.1630859375  1.0478515625  1.05615234375
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.1519
Commit e89d150 (2017-08-26 22:16 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   83330547 s          0 s   12752787 s  3843834041 s        154 s
       #2  3501 MHz  338428906 s          0 s   13942028 s  3589178424 s         52 s
       #3  3501 MHz   70937004 s          0 s    8084179 s  3867833801 s         72 s
       #4  3501 MHz   66187206 s          0 s    7987423 s  3873067238 s         24 s
       
  Memory: 31.383651733398438 GB (4643.36328125 MB free)
  Uptime: 3.9486013e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
