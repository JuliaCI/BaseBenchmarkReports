# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5a7a596aa45649c09eb028dac98924e5b7a871df](https://github.com/JuliaLang/julia/commit/5a7a596aa45649c09eb028dac98924e5b7a871df) vs [JuliaLang/julia@bd84fa1bad1e08b5c368999aa9b07e4382f54910](https://github.com/JuliaLang/julia/commit/bd84fa1bad1e08b5c368999aa9b07e4382f54910)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21694#issuecomment-299337756)

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
| `["array","bool","boolarray_bool_load!"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("catnd",5)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hcat",5)]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","sub2ind"]` | 0.13 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BitArray{2}")]` | 0.40 (50%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 0.40 (50%) :white_check_mark: | 0.76 (1%) :white_check_mark: |
| `["array","reverse","rev_load_slow!"]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup")]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(10,"scal_tup_x3")]` | 0.05 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup")]` | 0.09 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(3,"scal_tup_x3")]` | 0.39 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(3,"tup_tup")]` | 0.75 (15%) :white_check_mark: | 1.00 (1%)  |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup")]` | 0.09 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","mix_scalar_tuple",(5,"scal_tup_x3")]` | 0.45 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),2)]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["broadcast","sparse",((10000000,),2)]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["broadcast","typeargs",("tuple",10)]` | 0.04 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","typeargs",("tuple",3)]` | 0.43 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","typeargs",("tuple",5)]` | 0.48 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","arithmetic",("Date","Month")]` | 1.00 (15%)  | Inf (1%) :x: |
| `["dates","arithmetic",("Date","Year")]` | 1.37 (15%) :x: | Inf (1%) :x: |
| `["dates","arithmetic",("DateTime","Month")]` | 1.05 (15%)  | Inf (1%) :x: |
| `["dates","arithmetic",("DateTime","Year")]` | 1.21 (15%) :x: | Inf (1%) :x: |
| `["dates","construction","Date"]` | 1.58 (15%) :x: | Inf (1%) :x: |
| `["dates","construction","DateTime"]` | 1.66 (15%) :x: | Inf (1%) :x: |
| `["dates","parse","Date"]` | 1.20 (15%) :x: | Inf (1%) :x: |
| `["dates","parse","DateTime"]` | 1.17 (15%) :x: | Inf (1%) :x: |
| `["dates","parse",("Date","DateFormat")]` | 0.81 (15%) :white_check_mark: | 0.98 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 1.16 (15%) :x: | Inf (1%) :x: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.84 (15%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 1.23 (15%) :x: | Inf (1%) :x: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 1.06 (15%)  | 1.17 (1%) :x: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 1.00 (15%)  | 1.07 (1%) :x: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 1.06 (15%)  | 1.17 (1%) :x: |
| `["dates","query",("dayofweek","Date")]` | 0.33 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("dayofweek","DateTime")]` | 0.35 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","Date")]` | 0.32 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","DateTime")]` | 0.39 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","Date")]` | 0.30 (25%) :white_check_mark: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","DateTime")]` | 0.39 (25%) :white_check_mark: | 1.00 (1%)  |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.63 (15%) :white_check_mark: | 0.89 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Vector{String}")]` | 0.64 (15%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["linalg","blas","dotc"]` | 0.94 (40%)  | 0.33 (1%) :white_check_mark: |
| `["linalg","blas","dotu"]` | 0.93 (40%)  | 0.33 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Matrix",1024)]` | 0.51 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eig","Matrix",256)]` | 0.44 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",1024)]` | 0.51 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 0.44 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("schur","Matrix",1024)]` | 0.47 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("schur","Matrix",256)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",1024)]` | 0.48 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",256)]` | 0.42 (45%) :white_check_mark: | 1.00 (1%)  |
| `["misc","parse","DateTime"]` | 1.17 (15%) :x: | Inf (1%) :x: |
| `["misc","repeat",(200,1,24)]` | 0.30 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","repeat",(200,24,1)]` | 0.69 (15%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 1.01 (15%)  | 0.62 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 1.06 (15%)  | 0.46 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 1.01 (15%)  | 0.79 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 1.02 (15%)  | 0.55 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 1.04 (15%)  | 0.47 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 0.04 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","k_nucleotide"]` | 1.03 (15%)  | 0.99 (1%) :white_check_mark: |
| `["shootout","regex_dna"]` | 0.89 (15%)  | 0.88 (1%) :white_check_mark: |
| `["shootout","revcomp"]` | 0.26 (25%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4095)]` | 1.82 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 1.96 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4095)]` | 1.74 (20%) :x: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4096)]` | 1.76 (20%) :x: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 0.02 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 0.02 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 0.02 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 0.02 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 0.07 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 0.07 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 0.07 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 0.06 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 0.03 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 0.03 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 0.03 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 0.03 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4095)]` | 0.15 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields",4096)]` | 0.15 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4095)]` | 0.15 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields",4096)]` | 0.15 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","issorted",("reverse","ascending")]` | 0.18 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sort","issorted",("reverse","random")]` | 0.20 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 0.02 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",100)]` | 0.04 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",1000)]` | 0.08 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 0.03 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",100)]` | 0.07 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",1000)]` | 0.38 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","array",1000)]` | 0.38 (30%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(2,2))]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","reduction",("sum",(4,))]` | 1.21 (15%) :x: | 1.00 (1%)  |

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
- `["scalar","intfuncs"]`
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
- `["tuple","linear algebra"]`
- `["tuple","reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.beta.474
Commit 5a7a596 (2017-05-04 22:50 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (9215.4765625 MB free)
Uptime: 2.9596222e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   61544812 s          0 s    9482370 s  2882260306 s         86 s
#2  3501 MHz  235358939 s          0 s   10476145 s  2708301842 s         35 s
#3  3501 MHz   52455331 s          0 s    6099132 s  2899737523 s         45 s
#4  3501 MHz   47980796 s          0 s    6040748 s  2904549152 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-pre.beta.0
Commit bd84fa1 (2017-03-31 12:58 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (8501.328125 MB free)
Uptime: 2.960171e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   61641988 s          0 s    9492908 s  2882699426 s         86 s
#2  3501 MHz  235852355 s          0 s   10485322 s  2708347416 s         35 s
#3  3501 MHz   52537065 s          0 s    6108056 s  2900194904 s         45 s
#4  3501 MHz   48065674 s          0 s    6049508 s  2905003690 s         16 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
