# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f7708260fdb34c7c9b79c6f5e475f470b6bcd5a2](https://github.com/JuliaLang/julia/commit/f7708260fdb34c7c9b79c6f5e475f470b6bcd5a2) vs [JuliaLang/julia@474d05d0bef8bd2fad984db0223162de922f0315](https://github.com/JuliaLang/julia/commit/474d05d0bef8bd2fad984db0223162de922f0315)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20726#issuecomment-281495843)

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
| `["array","index",("sumlogical_view","1.0:0.00010001000100010001:2.0")]` | 2.29 (50%) :x: | 1.05 (1%) :x: |
| `["array","index",("sumlogical_view","Array{Float32,2}")]` | 30.51 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","Array{Int32,2}")]` | 30.56 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 30.44 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 30.38 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 30.39 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 30.41 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 30.62 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 30.44 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","BitArray{2}")]` | 29.75 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 30.37 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 29.81 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 150.22 (50%) :x: | 6.13 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 137.40 (50%) :x: | 6.13 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 30.35 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 27.93 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 30.57 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}")]` | 29.97 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}")]` | 151.83 (50%) :x: | 6.13 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}")]` | 141.59 (50%) :x: | 6.13 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 30.46 (50%) :x: | 1.95 (1%) :x: |
| `["array","index",("sumlogical_view","SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}")]` | 30.03 (50%) :x: | 1.95 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",100)]` | 1.30 (15%) :x: | 1.01 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 1.30 (15%) :x: | 1.01 (1%)  |
| `["broadcast","sparse",((1000,1000),1)]` | 1.43 (15%) :x: | 1.02 (1%) :x: |
| `["broadcast","sparse",((1000,1000),2)]` | 1.39 (15%) :x: | 1.01 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 4.47 (45%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 8.91 (45%) :x: | 1.26 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 4.51 (45%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 9.25 (45%) :x: | 1.26 (1%) :x: |
| `["linalg","arithmetic",("*","Matrix","Vector",1024)]` | 1.02 (45%)  | 1.07 (1%) :x: |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 1.32 (45%)  | 1.26 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 2.46 (45%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 4.86 (45%) :x: | 1.26 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 2.63 (45%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 5.30 (45%) :x: | 1.26 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 2.67 (45%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 4.34 (45%) :x: | 1.13 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 4.17 (45%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 8.49 (45%) :x: | 1.26 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 4.05 (45%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 7.73 (45%) :x: | 1.26 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 3.35 (45%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 6.68 (45%) :x: | 1.19 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 4.12 (45%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 7.01 (45%) :x: | 1.26 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 2.78 (45%) :x: | 1.03 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 3.94 (45%) :x: | 1.13 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 3.94 (45%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 8.05 (45%) :x: | 1.26 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 4.17 (45%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 6.96 (45%) :x: | 1.26 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 3.31 (45%) :x: | 1.05 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 6.71 (45%) :x: | 1.19 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 4.19 (45%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 6.96 (45%) :x: | 1.26 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 2.19 (45%) :x: | 1.07 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 4.45 (45%) :x: | 1.26 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 54.41 (45%) :x: | 1.88 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 163.87 (45%) :x: | 4.35 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 54.53 (45%) :x: | 1.88 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 166.35 (45%) :x: | 4.38 (1%) :x: |
| `["linalg","arithmetic",("sqrtm","Base.LinAlg.UnitUpperTriangular",1024)]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.41 (45%) :white_check_mark: | 1.00 (1%)  |
| `["micro","mandel"]` | 1.13 (15%)  | 1.25 (1%) :x: |
| `["micro","randmatstat"]` | 3.27 (15%) :x: | 1.21 (1%) :x: |
| `["misc","repeat",(200,1,24)]` | 1.41 (15%) :x: | 1.03 (1%) :x: |
| `["misc","repeat",(200,24,1)]` | 1.22 (15%) :x: | 1.02 (1%) :x: |
| `["problem","spellcheck","spellcheck"]` | 1.37 (15%) :x: | 1.05 (1%) :x: |
| `["shootout","revcomp"]` | 1.76 (25%) :x: | 3.02 (1%) :x: |
| `["sparse","index",("spmat","col","range",10)]` | 129.43 (30%) :x: | 4.60 (1%) :x: |
| `["sparse","index",("spmat","col","range",100)]` | 114.28 (30%) :x: | 4.00 (1%) :x: |
| `["sparse","index",("spmat","col","range",1000)]` | 73.99 (30%) :x: | 2.16 (1%) :x: |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.62 (30%) :x: | 1.00 (1%)  |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.49 (30%) :x: | 1.00 (1%)  |

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
Julia Version 0.6.0-dev.2896
Commit f770826 (2017-02-21 22:00 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (3041.37890625 MB free)
Uptime: 2.336668e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   39502981 s          0 s    8329207 s  2282072593 s         67 s
#2  3501 MHz  140051854 s          0 s    4949776 s  2190315087 s          9 s
#3  3501 MHz   35348627 s          0 s    4336611 s  2295898278 s         49 s
#4  3501 MHz   32990939 s          0 s    4479267 s  2298102274 s          8 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.6.0-dev.2894
Commit 474d05d (2017-02-21 18:13 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (2813.93359375 MB free)
Uptime: 2.3372882e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   39585391 s          0 s    8339150 s  2282597938 s         67 s
#2  3501 MHz  140614796 s          0 s    4958509 s  2190362991 s          9 s
#3  3501 MHz   35444995 s          0 s    4344673 s  2296413370 s         49 s
#4  3501 MHz   33073558 s          0 s    4487576 s  2298630934 s          8 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
