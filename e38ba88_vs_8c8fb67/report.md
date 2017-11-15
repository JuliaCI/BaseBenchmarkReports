# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@e38ba880159caf55743d699cfeb95fbbb632fe74](https://github.com/JuliaLang/julia/commit/e38ba880159caf55743d699cfeb95fbbb632fe74) vs [JuliaLang/julia@8c8fb6766be0f3db8ce7bb64fbc25baa275c5604](https://github.com/JuliaLang/julia/commit/8c8fb6766be0f3db8ce7bb64fbc25baa275c5604)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24113#issuecomment-344667023)

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
| `["array", "growth", "(\"prerend!\", 256)"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 7.23 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 12.82 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 6.63 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.23 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.88 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 8.77 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.28 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumeach_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 4.03 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}\")"]` | 7.00 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}\")"]` | 12.78 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 6.79 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Array{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.08 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,Array{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.95 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,Base.ReshapedArray{Float32,2,SubArray{Float32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 0.98 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.11 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Float32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.13 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 8.63 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true}\")"]` | 7.13 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,Array{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},true},Tuple{}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},true}\")"]` | 3.98 (50%) :x: | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,Base.ReshapedArray{Int32,2,SubArray{Int32,3,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false},Tuple{Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64},Base.MultiplicativeInverses.SignedMultiplicativeInverse{Int64}}},Tuple{Base.Slice{Base.OneTo{Int64}},UnitRange{Int64}},false}\")"]` | 1.09 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2},Tuple{Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.11 (50%)  | Inf (1%) :x: |
| `["array", "index", "(\"sumlinear_view\", \"SubArray{Int32,2,BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,3},Tuple{Int64,Base.Slice{Base.OneTo{Int64}},Base.Slice{Base.OneTo{Int64}}},false}\")"]` | 1.13 (50%)  | Inf (1%) :x: |
| `["array", "reductions", "(\"var\", \"Float64\")"]` | 1.00 (15%)  | 0.80 (1%) :white_check_mark: |
| `["array", "reductions", "(\"var\", \"Int64\")"]` | 1.00 (15%)  | 0.82 (1%) :white_check_mark: |
| `["dates", "parse", "DateTime"]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["io", "read", "readstring"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["linalg", "arithmetic", "(\"+\", \"Vector\", \"Vector\", 256)"]` | 1.67 (45%) :x: | 1.00 (1%)  |
| `["misc", "julia", "(\"parse\", \"array\")"]` | 1.00 (15%)  | 0.97 (1%) :white_check_mark: |
| `["misc", "julia", "(\"parse\", \"function\")"]` | 1.03 (15%)  | 0.95 (1%) :white_check_mark: |
| `["misc", "julia", "(\"parse\", \"nested\")"]` | 1.00 (15%)  | 0.98 (1%) :white_check_mark: |
| `["parallel", "remotecall", "(\"identity\", 1024)"]` | 0.99 (15%)  | 1.09 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 2)"]` | 1.01 (15%)  | 1.17 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 4096)"]` | 1.00 (15%)  | 1.04 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 512)"]` | 1.01 (15%)  | 1.12 (1%) :x: |
| `["parallel", "remotecall", "(\"identity\", 64)"]` | 1.03 (15%)  | 1.16 (1%) :x: |
| `["problem", "json", "parse_json"]` | 1.02 (15%)  | 0.97 (1%) :white_check_mark: |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{Int128}\")"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "types", "(\"rand!\", \"MersenneTwister\", \"Complex{UInt128}\")"]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ascending\")"]` | 0.97 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! forwards\", \"descending\")"]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! forwards\", \"ones\")"]` | 1.05 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! forwards\", \"random\")"]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ascending\")"]` | 1.00 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"descending\")"]` | 1.06 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"ones\")"]` | 1.04 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sort! reverse\", \"random\")"]` | 1.00 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ascending\")"]` | 1.07 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"descending\")"]` | 1.00 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"ones\")"]` | 1.01 (30%)  | 0.91 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! forwards\", \"random\")"]` | 1.00 (30%)  | 0.91 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.00 (30%)  | 0.63 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"descending\")"]` | 1.02 (30%)  | 0.63 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"ones\")"]` | 0.99 (30%)  | 0.67 (1%) :white_check_mark: |
| `["sort", "insertionsort", "(\"sortperm! reverse\", \"random\")"]` | 1.00 (30%)  | 0.67 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"reverse\", \"ascending\")"]` | 1.00 (30%)  | 0.80 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"reverse\", \"descending\")"]` | 1.00 (30%)  | 0.80 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"reverse\", \"ones\")"]` | 1.00 (30%)  | 0.80 (1%) :white_check_mark: |
| `["sort", "issorted", "(\"reverse\", \"random\")"]` | 1.00 (30%)  | 0.80 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! forwards\", \"ascending\")"]` | 1.01 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! forwards\", \"descending\")"]` | 1.03 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! forwards\", \"ones\")"]` | 1.03 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! forwards\", \"random\")"]` | 1.00 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! reverse\", \"ascending\")"]` | 1.02 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! reverse\", \"descending\")"]` | 1.01 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! reverse\", \"ones\")"]` | 0.99 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sort! reverse\", \"random\")"]` | 0.99 (30%)  | 0.60 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ascending\")"]` | 1.01 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"descending\")"]` | 1.01 (30%)  | 0.89 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"ones\")"]` | 1.00 (30%)  | 0.91 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! forwards\", \"random\")"]` | 1.00 (30%)  | 0.91 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ascending\")"]` | 1.00 (30%)  | 0.63 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"descending\")"]` | 1.00 (30%)  | 0.63 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"ones\")"]` | 0.99 (30%)  | 0.67 (1%) :white_check_mark: |
| `["sort", "quicksort", "(\"sortperm! reverse\", \"random\")"]` | 1.00 (30%)  | 0.67 (1%) :white_check_mark: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 10)"]` | 1.00 (30%)  | 1.11 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 100)"]` | 1.00 (30%)  | 1.04 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 1000)"]` | 0.96 (30%)  | 1.01 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 10)"]` | 1.00 (30%)  | 1.08 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 100)"]` | 1.00 (30%)  | 1.03 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 10)"]` | 1.00 (30%)  | 1.08 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 100)"]` | 1.00 (30%)  | 1.08 (1%) :x: |
| `["sparse", "index", "(\"spmat\", \"splogical\", 1000)"]` | 1.00 (30%)  | 1.05 (1%) :x: |
| `["string", "search", "String"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array", "bool"]`
- `["array", "cat"]`
- `["array", "comprehension"]`
- `["array", "convert"]`
- `["array", "growth"]`
- `["array", "index"]`
- `["array", "reductions"]`
- `["array", "reverse"]`
- `["array", "setindex!"]`
- `["array", "subarray"]`
- `["broadcast", "dotop"]`
- `["broadcast", "fusion"]`
- `["broadcast", "mix_scalar_tuple"]`
- `["broadcast", "sparse"]`
- `["broadcast", "typeargs"]`
- `["dates", "accessor"]`
- `["dates", "arithmetic"]`
- `["dates", "construction"]`
- `["dates", "conversion"]`
- `["dates", "parse"]`
- `["dates", "query"]`
- `["dates", "string"]`
- `["io", "read"]`
- `["io", "serialization"]`
- `["linalg", "arithmetic"]`
- `["linalg", "blas"]`
- `["linalg", "factorization"]`
- `["micro"]`
- `["misc", "afoldl"]`
- `["misc", "bitshift"]`
- `["misc", "julia"]`
- `["misc", "parse"]`
- `["misc", "repeat"]`
- `["misc", "splatting"]`
- `["nullable", "basic"]`
- `["nullable", "nullablearray"]`
- `["parallel", "remotecall"]`
- `["problem", "chaosgame"]`
- `["problem", "fem"]`
- `["problem", "go"]`
- `["problem", "grigoriadis khachiyan"]`
- `["problem", "imdb"]`
- `["problem", "json"]`
- `["problem", "laplacian"]`
- `["problem", "monte carlo"]`
- `["problem", "raytrace"]`
- `["problem", "seismic"]`
- `["problem", "simplex"]`
- `["problem", "spellcheck"]`
- `["problem", "stockcorr"]`
- `["problem", "ziggurat"]`
- `["random", "collections"]`
- `["random", "randstring"]`
- `["random", "ranges"]`
- `["random", "sequences"]`
- `["random", "types"]`
- `["scalar", "acos"]`
- `["scalar", "arithmetic"]`
- `["scalar", "asin"]`
- `["scalar", "atan"]`
- `["scalar", "atan2"]`
- `["scalar", "cos"]`
- `["scalar", "fastmath"]`
- `["scalar", "floatexp"]`
- `["scalar", "intfuncs"]`
- `["scalar", "iteration"]`
- `["scalar", "mod2pi"]`
- `["scalar", "predicate"]`
- `["scalar", "rem_pio2"]`
- `["scalar", "sin"]`
- `["scalar", "sincos"]`
- `["scalar", "tan"]`
- `["shootout"]`
- `["simd"]`
- `["sort", "insertionsort"]`
- `["sort", "issorted"]`
- `["sort", "mergesort"]`
- `["sort", "quicksort"]`
- `["sparse", "arithmetic"]`
- `["sparse", "constructors"]`
- `["sparse", "index"]`
- `["sparse", "matmul"]`
- `["sparse", "transpose"]`
- `["string"]`
- `["string", "readuntil"]`
- `["string", "search"]`
- `["string", "searchindex"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "reduction"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-DEV.2513
Commit e38ba88 (2017-11-15 17:28 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   93718172 s          0 s   14522944 s  4523466194 s        208 s
       #2  3501 MHz  375267901 s          0 s   15840421 s  4242725476 s         72 s
       #3  3501 MHz   77276881 s          0 s    8790783 s  4554088608 s         94 s
       #4  3501 MHz   72450643 s          0 s    8662120 s  4559461751 s         40 s
       
  Memory: 31.383651733398438 GB (10398.3671875 MB free)
  Uptime: 4.6420698e7 sec
  Load Avg:  0.9638671875  0.998046875  1.0400390625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.7.0-DEV.2511
Commit 8c8fb67 (2017-11-15 15:27 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   93806910 s          0 s   14533154 s  4524084662 s        208 s
       #2  3501 MHz  375920370 s          0 s   15849792 s  4242783136 s         72 s
       #3  3501 MHz   77363785 s          0 s    8798474 s  4554713420 s         94 s
       #4  3501 MHz   72551160 s          0 s    8670106 s  4560072929 s         40 s
       
  Memory: 31.383651733398438 GB (10196.640625 MB free)
  Uptime: 4.6427901e7 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```
