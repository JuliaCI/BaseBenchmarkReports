# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@245208df4dcac86cf413dc2ed7aba5243fba1e44](https://github.com/JuliaLang/julia/commit/245208df4dcac86cf413dc2ed7aba5243fba1e44) vs [JuliaLang/julia@dd6ee639e1dea118681f57f5b5784c6e76442de5](https://github.com/JuliaLang/julia/commit/dd6ee639e1dea118681f57f5b5784c6e76442de5)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18457#issuecomment-270978401)

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
| `["array","cat",("catnd",5)]` | 1.59 (15%) :x: | 1.02 (1%) :x: |
| `["array","cat",("catnd_setind",5)]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat",5)]` | 4.20 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("vcat",5)]` | 2.53 (15%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{Colon,Colon},true}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Colon,Colon},true}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 1.58 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Colon,Colon},false}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{Colon,Colon},true}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Colon,Colon},true}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Colon,Colon,Colon},true},Tuple{}},Tuple{Colon,UnitRange{Int64}},true}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Colon,Colon},false}")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.55 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Colon,Colon},false}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.56 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Colon,Colon,Colon},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Colon,UnitRange{Int64}},false}")]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Colon,Colon},false}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Colon,Colon},false}")]` | 1.54 (50%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",1)]` | 1.51 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",2)]` | 1.55 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",3)]` | 1.51 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",4)]` | 1.54 (15%) :x: | 1.00 (1%)  |
| `["array","setindex!",("setindex!",5)]` | 1.48 (15%) :x: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("Date","ISODateFormat")]` | 1.28 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 1.21 (15%) :x: | 1.00 (1%)  |
| `["io","serialization",("deserialize","Vector{String}")]` | 2.31 (15%) :x: | 3.08 (1%) :x: |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",256)]` | 1.00 (45%)  | 0.99 (1%) :white_check_mark: |
| `["micro","randmatstat"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_any","NullableArray")]` | 1.53 (50%) :x: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.25 (15%) :x: | 1.06 (1%) :x: |
| `["parallel","remotecall",("identity",2)]` | 1.27 (15%) :x: | 1.09 (1%) :x: |
| `["parallel","remotecall",("identity",4096)]` | 1.23 (15%) :x: | 1.03 (1%) :x: |
| `["parallel","remotecall",("identity",512)]` | 1.25 (15%) :x: | 1.07 (1%) :x: |
| `["parallel","remotecall",("identity",64)]` | 1.26 (15%) :x: | 1.09 (1%) :x: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 1.33 (15%) :x: | 1.00 (1%)  |
| `["problem","raytrace","raytrace"]` | 1.41 (15%) :x: | 1.00 (1%)  |
| `["sort","issorted",("reverse","ascending")]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sort","issorted",("reverse","random")]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 1.39 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",100)]` | 1.38 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",1000)]` | 1.34 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 1.37 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",100)]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.44 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.47 (30%) :x: | 1.00 (1%)  |

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
- `["broadcast","sparse"]`
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
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","floatexp"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
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
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-dev.1976
Commit 245208d (2017-01-06 12:31 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (1734.23046875 MB free)
Uptime: 1.9382307e7 sec
Load Avg:  1.0029296875  1.0146484375  0.97607421875
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   28734443 s          0 s    6473451 s  1897475708 s         60 s
#2  3501 MHz   94505954 s          0 s    3984796 s  1838587389 s          8 s
#3  3501 MHz   26840722 s          0 s    3426341 s  1907058599 s         41 s
#4  3501 MHz   24495897 s          0 s    3532021 s  1909285448 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.1965
Commit dd6ee63 (2017-01-06 17:41 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (1869.86328125 MB free)
Uptime: 1.9389492e7 sec
Load Avg:  1.0029296875  1.0146484375  0.9814453125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   28822104 s          0 s    6483032 s  1898094698 s         60 s
#2  3501 MHz   94932887 s          0 s    3992996 s  1838870300 s          8 s
#3  3501 MHz   26905597 s          0 s    3433088 s  1907704634 s         41 s
#4  3501 MHz   24600736 s          0 s    3541242 s  1909889289 s          7 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
