# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@cd94b4a31bc2ac76dd56953c5e7f61f60906caf2](https://github.com/JuliaLang/julia/commit/cd94b4a31bc2ac76dd56953c5e7f61f60906caf2) vs [JuliaLang/julia@6b1b4f6100677520ced65c253d02b6f22ceea1e6](https://github.com/JuliaLang/julia/commit/6b1b4f6100677520ced65c253d02b6f22ceea1e6)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18777#issuecomment-271543403)

*Tag Predicate:* `"array"`

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
| `["array","cat",("hcat",5)]` | 0.68 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hcat_setind",5)]` | 0.49 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat",5)]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("hvcat_setind",5)]` | 0.60 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat",5)]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("vcat_setind",5)]` | 0.53 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","growth",("append!",2048)]` | 0.84 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1.0:1.0:100000.0")]` | 0.95 (50%)  | 1.23 (1%) :x: |
| `["array","index",("sumcolon","1.0:1.0:100000.0")]` | 2.17 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1.0:1.0:100000.0")]` | 7.42 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1.0:1.0:100000.0")]` | 2.78 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1.0:1.0:100000.0")]` | 7.42 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumrange","1.0:1.0:100000.0")]` | 2.18 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector","1.0:1.0:100000.0")]` | 0.90 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumvector_view","1.0:1.0:100000.0")]` | 0.97 (50%)  | 1.07 (1%) :x: |
| `["array","index",("sumvector_view","Array{Int32,2}")]` | 1.77 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.57 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumvector_view","SubArray{Int32,2,Array{Int32,3},Tuple{Int64,Colon,Colon},true}")]` | 1.52 (50%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",250)]` | 1.69 (15%) :x: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",500)]` | 1.78 (15%) :x: | 1.00 (1%)  |

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
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["misc","repeat"]`
- `["misc","splatting"]`
- `["problem","laplacian"]`
- `["simd"]`
- `["sparse","arithmetic"]`
- `["sparse","index"]`
- `["sparse","transpose"]`

## Version Info

#### Primary Build

```
?
```

#### Comparison Build

```
?
```
