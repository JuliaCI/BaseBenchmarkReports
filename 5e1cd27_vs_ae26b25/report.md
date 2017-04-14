# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5e1cd27535692eeaedcb0bd6ecebf444c0c5db0d](https://github.com/JuliaLang/julia/commit/5e1cd27535692eeaedcb0bd6ecebf444c0c5db0d) vs [JuliaLang/julia@ae26b25d43317d7dd3ca05f60b70677aab9c0e08](https://github.com/JuliaLang/julia/commit/ae26b25d43317d7dd3ca05f60b70677aab9c0e08)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20993#issuecomment-294009183)

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
| `["array","bool","bitarray_bool_load!"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","bool","boolarray_bool_load!"]` | 0.65 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","bool","boolarray_true_fill!"]` | 0.22 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","bool","boolarray_true_load!"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","cat",("catnd",5)]` | 0.67 (15%) :white_check_mark: | 0.75 (1%) :white_check_mark: |
| `["array","cat",("catnd_setind",5)]` | 1.40 (15%) :x: | 1.00 (1%)  |
| `["array","cat",("hcat",5)]` | 0.16 (15%) :white_check_mark: | 0.94 (1%) :white_check_mark: |
| `["array","cat",("hcat_setind",5)]` | 1.00 (15%)  | 1.06 (1%) :x: |
| `["array","cat",("hvcat",5)]` | 0.81 (15%) :white_check_mark: | 0.95 (1%) :white_check_mark: |
| `["array","cat",("vcat",5)]` | 0.22 (15%) :white_check_mark: | 0.90 (1%) :white_check_mark: |
| `["array","cat",("vcat_setind",5)]` | 0.93 (15%)  | 1.06 (1%) :x: |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 1.30 (15%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_indexing","Array{Float64,1}")]` | 1.43 (30%) :x: | 1.00 (1%)  |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 1.27 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Float64","Int")]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","convert",("Int","Complex{Float64}")]` | 1.19 (15%) :x: | 1.00 (1%)  |
| `["array","convert",("Int","Float64")]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["array","growth",("push_single!",2048)]` | 2.09 (15%) :x: | 1.01 (1%) :x: |
| `["array","growth",("push_single!",256)]` | 2.15 (15%) :x: | 1.02 (1%) :x: |
| `["array","growth",("push_single!",8)]` | 2.18 (15%) :x: | 1.02 (1%) :x: |
| `["array","index","2d"]` | 0.67 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","3d"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","4d"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","5d"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","index","7d"]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","index","sub2ind"]` | 0.28 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sum","3dsubarray")]` | 0.62 (50%)  | Inf (1%) :x: |
| `["array","index",("sumcartesian","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian","1:100000")]` | 3.98 (50%) :x: | 1.00 (1%)  |
| `["array","index",("sumcartesian","BitArray{2}")]` | 0.56 (50%)  | 2.00 (1%) :x: |
| `["array","index",("sumcartesian_view","1.0:1.0:100000.0")]` | 0.19 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.28 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.28 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.35 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.34 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.36 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.34 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcartesian_view","BitArray{2}")]` | 0.52 (50%)  | 1.25 (1%) :x: |
| `["array","index",("sumcolon","1.0:1.0:100000.0")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumcolon","Array{Float32,2}")]` | 1.26 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","Array{Int32,2}")]` | 1.25 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.22 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.23 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.27 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.28 (50%)  | 1.04 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.25 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.25 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumcolon","BitArray{2}")]` | 0.87 (50%)  | 1.08 (1%) :x: |
| `["array","index",("sumcolon_view","1.0:1.0:100000.0")]` | 0.54 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","100000:-1:1")]` | 0.57 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","1:100000")]` | 0.53 (50%)  | 0.00 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","Array{Float32,2}")]` | 0.31 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","Array{Int32,2}")]` | 0.30 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.26 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.25 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.23 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.20 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.21 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.24 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array","index",("sumcolon_view","BitArray{2}")]` | 0.37 (50%) :white_check_mark: | 0.43 (1%) :white_check_mark: |
| `["array","index",("sumeach","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","Array{Int32,2}")]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach","BitArray{2}")]` | 0.53 (50%)  | 2.00 (1%) :x: |
| `["array","index",("sumeach_view","1.0:1.0:100000.0")]` | 0.19 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","Array{Float32,2}")]` | 6.01 (50%) :x: | 2.67 (1%) :x: |
| `["array","index",("sumeach_view","Array{Float64,3}")]` | 3.14 (50%) :x: | 2.67 (1%) :x: |
| `["array","index",("sumeach_view","Array{Int32,2}")]` | 6.18 (50%) :x: | 2.67 (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.21 (50%)  | 1.67 (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.20 (50%)  | 1.67 (1%) :x: |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.39 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumeach_view","BitArray{2}")]` | 14.97 (50%) :x: | 4.25 (1%) :x: |
| `["array","index",("sumelt","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","Array{Int32,2}")]` | 0.19 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt","BitArray{2}")]` | 0.54 (50%)  | 2.00 (1%) :x: |
| `["array","index",("sumelt_boundscheck","100000:-1:1")]` | 0.06 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","1:100000")]` | 0.41 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","Array{Int32,2}")]` | 0.19 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.40 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 0.58 (50%)  | 2.00 (1%) :x: |
| `["array","index",("sumlinear","1.0:1.0:100000.0")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","Array{Int32,2}")]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear","BitArray{2}")]` | 0.52 (50%)  | 2.00 (1%) :x: |
| `["array","index",("sumlinear_view","1.0:1.0:100000.0")]` | 0.19 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","100000:-1:1")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","1:100000")]` | 0.00 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumlinear_view","Array{Float32,2}")]` | 5.98 (50%) :x: | 2.67 (1%) :x: |
| `["array","index",("sumlinear_view","Array{Float64,3}")]` | 3.15 (50%) :x: | 2.67 (1%) :x: |
| `["array","index",("sumlinear_view","Array{Int32,2}")]` | 5.94 (50%) :x: | 2.67 (1%) :x: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.23 (50%)  | 1.67 (1%) :x: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.19 (50%)  | 1.67 (1%) :x: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 3.48 (50%) :x: | 2.33 (1%) :x: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 3.40 (50%) :x: | 2.33 (1%) :x: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 3.49 (50%) :x: | 2.33 (1%) :x: |
| `["array","index",("sumlinear_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 3.43 (50%) :x: | 2.33 (1%) :x: |
| `["array","index",("sumlinear_view","BitArray{2}")]` | 15.13 (50%) :x: | 4.25 (1%) :x: |
| `["array","index",("sumlogical","1.0:1.0:100000.0")]` | 0.59 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","100000:-1:1")]` | 0.75 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","1:100000")]` | 0.70 (50%)  | 0.52 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 0.57 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 0.56 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.56 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.56 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.56 (50%)  | 0.40 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.56 (50%)  | 0.40 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.55 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.56 (50%)  | 0.39 (1%) :white_check_mark: |
| `["array","index",("sumlogical","BitArray{2}")]` | 0.88 (50%)  | 0.15 (1%) :white_check_mark: |
| `["array","index",("sumlogical_view","Array{Float32,2}")]` | 0.73 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumlogical_view","Array{Int32,2}")]` | 0.73 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.70 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.71 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.72 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.72 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.72 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumlogical_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.72 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumlogical_view","BitArray{2}")]` | 0.69 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","1.0:1.0:100000.0")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange","Array{Float32,2}")]` | 1.03 (50%)  | 1.02 (1%) :x: |
| `["array","index",("sumrange","Array{Int32,2}")]` | 1.04 (50%)  | 1.02 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.19 (50%)  | 1.02 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.11 (50%)  | 1.02 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.20 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.21 (50%)  | 1.01 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.17 (50%)  | 1.02 (1%) :x: |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.18 (50%)  | 1.02 (1%) :x: |
| `["array","index",("sumrange","BitArray{2}")]` | 0.82 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.39 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.41 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.35 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.34 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.38 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumrange_view","BitArray{2}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["array","index",("sumvector","1.0:1.0:100000.0")]` | 0.68 (50%)  | 1.05 (1%) :x: |
| `["array","index",("sumvector","BitArray{2}")]` | 0.85 (50%)  | 1.12 (1%) :x: |
| `["array","index",("sumvector_view","1.0:1.0:100000.0")]` | 0.72 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","100000:-1:1")]` | 0.77 (50%)  | 0.94 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","1:100000")]` | 0.71 (50%)  | 0.88 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","Array{Float32,2}")]` | 0.42 (50%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","Array{Int32,2}")]` | 0.50 (50%)  | 0.71 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 0.42 (50%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 0.29 (50%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 0.31 (50%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 0.41 (50%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 0.29 (50%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 0.35 (50%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["array","index",("sumvector_view","BitArray{2}")]` | 0.39 (50%) :white_check_mark: | 0.71 (1%) :white_check_mark: |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.norm1","Float64")]` | 0.89 (15%)  | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.norm1","Int64")]` | 0.50 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.norminf","Float64")]` | 1.13 (15%)  | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.norminf","Int64")]` | 0.76 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.perf_mapreduce","Float64")]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.perf_mapreduce","Int64")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.perf_reduce","Float64")]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("BaseBenchmarks.ArrayBenchmarks.perf_reduce","Int64")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("maxabs","Float64")]` | 0.06 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("maxabs","Int64")]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("mean","Float64")]` | 0.56 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("mean","Int64")]` | 0.43 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("norm","Float64")]` | 0.95 (15%)  | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("norm","Int64")]` | 0.40 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sum","Float64")]` | 0.53 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sum","Int64")]` | 0.42 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sumabs","Float64")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sumabs","Int64")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sumabs2","Float64")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("sumabs2","Int64")]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["array","reductions",("var","Float64")]` | 0.74 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","reductions",("var","Int64")]` | 0.96 (15%)  | 1.13 (1%) :x: |
| `["array","setindex!",("setindex!",1)]` | 0.96 (15%)  | 1.38 (1%) :x: |
| `["array","setindex!",("setindex!",2)]` | 0.97 (15%)  | 1.38 (1%) :x: |
| `["array","setindex!",("setindex!",3)]` | 1.06 (15%)  | 1.38 (1%) :x: |
| `["array","setindex!",("setindex!",4)]` | 1.04 (15%)  | 1.38 (1%) :x: |
| `["array","setindex!",("setindex!",5)]` | 0.93 (15%)  | 1.38 (1%) :x: |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 0.78 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",250)]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivCopy!",500)]` | 0.76 (15%) :white_check_mark: | 1.00 (1%)  |
| `["array","subarray",("lucompletepivSub!",100)]` | 0.07 (15%) :white_check_mark: | 0.23 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivSub!",1000)]` | 0.08 (15%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivSub!",250)]` | 0.06 (15%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["array","subarray",("lucompletepivSub!",500)]` | 0.08 (15%) :white_check_mark: | 0.20 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000,1000),2)]` | 0.15 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),1)]` | 0.02 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","dotop",("Float64",(1000000,),2)]` | 0.03 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000,1000),2)]` | 0.04 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000,1000),3)]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000000,),1)]` | 0.07 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","fusion",("Float64",(1000000,),2)]` | 0.29 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),1)]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["broadcast","sparse",((1000,1000),2)]` | 0.00 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["dates","accessor","hour"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","minute"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","accessor","second"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("Date","Day")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Day")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Hour")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Millisecond")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Minute")]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","arithmetic",("DateTime","Second")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","construction","DateTime"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","conversion","Date -> DateTime"]` | 0.72 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","conversion","DateTime -> Date"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates","parse","Date"]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse","DateTime"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("Date","DateFormat")]` | 0.47 (15%) :white_check_mark: | 0.41 (1%) :white_check_mark: |
| `["dates","parse",("Date","ISODateFormat")]` | 0.01 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","DateFormat")]` | 0.43 (15%) :white_check_mark: | 0.60 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","ISODateTimeFormat")]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Lowercase")]` | 0.02 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Mixedcase")]` | 0.04 (15%) :white_check_mark: | 0.14 (1%) :white_check_mark: |
| `["dates","parse",("DateTime","RFC1123Format","Titlecase")]` | 0.02 (15%) :white_check_mark: | 0.06 (1%) :white_check_mark: |
| `["dates","query",("dayofweek","Date")]` | 2.99 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("dayofweek","DateTime")]` | 2.08 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","Date")]` | 3.06 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("firstdayofweek","DateTime")]` | 2.00 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","Date")]` | 3.14 (25%) :x: | 1.00 (1%)  |
| `["dates","query",("lastdayofweek","DateTime")]` | 2.08 (25%) :x: | 1.00 (1%)  |
| `["dates","string","Date"]` | 0.61 (15%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["dates","string","DateTime"]` | 0.47 (15%) :white_check_mark: | 0.74 (1%) :white_check_mark: |
| `["io","read","read"]` | 0.77 (15%) :white_check_mark: | 1.00 (1%)  |
| `["io","read","readstring"]` | 0.35 (15%) :white_check_mark: | 0.55 (1%) :white_check_mark: |
| `["io","serialization",("deserialize","Vector{String}")]` | 0.63 (15%) :white_check_mark: | 0.61 (1%) :white_check_mark: |
| `["io","serialization",("serialize","Matrix{Float64}")]` | 2.95 (15%) :x: | 1.00 (1%)  |
| `["io","serialization",("serialize","Vector{String}")]` | 0.55 (15%) :white_check_mark: | 0.66 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 0.61 (45%)  | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 0.58 (45%)  | 0.91 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 0.62 (45%)  | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 0.53 (45%) :white_check_mark: | 0.91 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",1024)]` | 0.98 (45%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",256)]` | 0.97 (45%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","LowerTriangular","Vector",256)]` | 1.02 (45%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 1.01 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 1.44 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 1.31 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",1024)]` | 0.97 (45%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",256)]` | 0.96 (45%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("*","UpperTriangular","Vector",256)]` | 1.04 (45%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 2.55 (45%) :x: | 2.00 (1%) :x: |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 3.71 (45%) :x: | 2.02 (1%) :x: |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 1.53 (45%) :x: | 1.01 (1%) :x: |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 1.55 (45%) :x: | 1.01 (1%) :x: |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 1.72 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 1.51 (45%) :x: | 1.01 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 2.53 (45%) :x: | 2.00 (1%) :x: |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 3.78 (45%) :x: | 2.02 (1%) :x: |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 1.52 (45%) :x: | 1.01 (1%) :x: |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 1.57 (45%) :x: | 1.01 (1%) :x: |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 1.69 (45%) :x: | 1.02 (1%) :x: |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 1.54 (45%) :x: | 1.01 (1%) :x: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 0.49 (45%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 0.46 (45%) :white_check_mark: | 0.91 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",1024)]` | 0.98 (45%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",256)]` | 0.97 (45%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",1024)]` | 0.96 (45%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",256)]` | 0.96 (45%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("A_mul_B!","Matrix{Float32}","Matrix{Float64}","Matrix{Float64}",1024)]` | 0.03 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("A_mul_B!","Matrix{Float32}","Matrix{Float64}","Matrix{Float64}",256)]` | 0.03 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Bidiagonal","Vector",256)]` | 0.92 (45%)  | 1.02 (1%) :x: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 0.49 (45%) :white_check_mark: | 0.97 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 0.45 (45%) :white_check_mark: | 0.91 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 0.43 (45%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 0.45 (45%) :white_check_mark: | 0.49 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","HermitianSparseWithNonZeroPivots","Vector",1024)]` | 0.93 (45%)  | 1.04 (1%) :x: |
| `["linalg","arithmetic",("\\","HermitianSparseWithNonZeroPivots","Vector",256)]` | 0.88 (45%)  | 1.04 (1%) :x: |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",1024)]` | 0.97 (45%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",256)]` | 0.97 (45%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 1.01 (45%)  | 1.01 (1%) :x: |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",1024)]` | 0.95 (45%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",256)]` | 0.97 (45%)  | 0.50 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",1024)]` | 0.02 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","NPDUpperTriangular",256)]` | 0.02 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",1024)]` | 0.01 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","arithmetic",("sqrtm","UpperTriangular",256)]` | 0.01 (45%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["linalg","blas","axpy!"]` | 0.55 (40%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","dot"]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["linalg","blas","dotc"]` | 0.67 (40%)  | 1.20 (1%) :x: |
| `["linalg","blas","dotu"]` | 0.67 (40%)  | 1.20 (1%) :x: |
| `["linalg","factorization",("eig","Bidiagonal",1024)]` | 0.03 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 0.04 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Matrix",1024)]` | 1.90 (45%) :x: | 0.40 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","Matrix",256)]` | 2.22 (45%) :x: | 0.41 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","SymTridiagonal",1024)]` | 1.57 (45%) :x: | 0.51 (1%) :white_check_mark: |
| `["linalg","factorization",("eig","SymTridiagonal",256)]` | 1.61 (45%) :x: | 0.53 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Bidiagonal",1024)]` | 0.03 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 0.04 (45%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Matrix",1024)]` | 1.85 (45%) :x: | 0.40 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 2.22 (45%) :x: | 0.41 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","SymTridiagonal",1024)]` | 1.58 (45%) :x: | 0.51 (1%) :white_check_mark: |
| `["linalg","factorization",("eigfact","SymTridiagonal",256)]` | 1.61 (45%) :x: | 0.53 (1%) :white_check_mark: |
| `["linalg","factorization",("lufact","Tridiagonal",256)]` | 1.15 (45%)  | 1.02 (1%) :x: |
| `["linalg","factorization",("schur","Matrix",1024)]` | 2.07 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schur","Matrix",256)]` | 2.33 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",1024)]` | 2.08 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("schurfact","Matrix",256)]` | 2.33 (45%) :x: | 1.00 (1%)  |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 0.60 (45%)  | 0.67 (1%) :white_check_mark: |
| `["linalg","factorization",("svd","Diagonal",256)]` | 1.76 (45%) :x: | 0.68 (1%) :white_check_mark: |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 0.68 (45%)  | 0.72 (1%) :white_check_mark: |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 1.62 (45%) :x: | 0.73 (1%) :white_check_mark: |
| `["micro","fib"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["micro","mandel"]` | 0.92 (15%)  | 1.02 (1%) :x: |
| `["micro","parseint"]` | 0.88 (15%)  | 0.75 (1%) :white_check_mark: |
| `["micro","pisum"]` | 0.54 (15%) :white_check_mark: | 1.00 (1%)  |
| `["micro","randmatmul"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["micro","randmatstat"]` | 0.79 (15%) :white_check_mark: | 0.99 (1%) :white_check_mark: |
| `["misc","afoldl","Int"]` | 1.31 (15%) :x: | 1.00 (1%)  |
| `["misc","bitshift",("Int","Int")]` | 0.06 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("Int","UInt")]` | 0.06 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt","UInt")]` | 0.06 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","bitshift",("UInt32","UInt32")]` | 0.29 (15%) :white_check_mark: | 1.00 (1%)  |
| `["misc","parse","DateTime"]` | 0.00 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["misc","repeat",(200,1,24)]` | 0.01 (15%) :white_check_mark: | 0.03 (1%) :white_check_mark: |
| `["misc","repeat",(200,24,1)]` | 0.03 (15%) :white_check_mark: | 0.04 (1%) :white_check_mark: |
| `["nullable","basic",("get2","Nullable{Bool}()")]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Float32}()")]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Float64}()")]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int64}()")]` | 0.50 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("get2","Nullable{Int8}()")]` | 0.60 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{BigFloat}()","Nullable{BigFloat}()")]` | 0.38 (60%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Bool}()","Nullable{Bool}()")]` | 0.39 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float32}()","Nullable{Float32}()")]` | 0.53 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Float64}()","Nullable{Float64}()")]` | 0.53 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int64}()","Nullable{Int64}()")]` | 0.41 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isequal","Nullable{Int8}()","Nullable{Int8}()")]` | 0.39 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","basic",("isnull","Nullable{Int64}()")]` | 0.63 (30%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Bool")]` | 0.21 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Float32")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Float64")]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int64")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","Array","Int8")]` | 0.23 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Bool")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float32")]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Float64")]` | 0.49 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int64")]` | 0.35 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countequals","NullableArray","Int8")]` | 0.34 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Bool")]` | 0.13 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Float32")]` | 0.10 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_countnulls","Array","Int8")]` | 0.13 (50%) :white_check_mark: | 1.00 (1%)  |
| `["nullable","nullablearray",("perf_sum","Array","Int8")]` | 0.06 (50%) :white_check_mark: | 1.00 (1%)  |
| `["parallel","remotecall",("identity",1024)]` | 0.93 (15%)  | 0.92 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",2)]` | 0.94 (15%)  | 0.89 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",4096)]` | 0.93 (15%)  | 0.92 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",512)]` | 0.95 (15%)  | 0.82 (1%) :white_check_mark: |
| `["parallel","remotecall",("identity",64)]` | 0.95 (15%)  | 0.81 (1%) :white_check_mark: |
| `["problem","go","go_game"]` | 0.93 (15%)  | 1.29 (1%) :x: |
| `["problem","imdb","centrality"]` | 0.66 (15%) :white_check_mark: | 0.88 (1%) :white_check_mark: |
| `["problem","json","parse_json"]` | 0.81 (15%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_sub"]` | 0.20 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_iter_vec"]` | 0.35 (15%) :white_check_mark: | 0.40 (1%) :white_check_mark: |
| `["problem","laplacian","laplace_sparse_matvec"]` | 5.46 (15%) :x: | 0.99 (1%)  |
| `["problem","monte carlo","euro_option_devec"]` | 0.79 (15%) :white_check_mark: | 0.50 (1%) :white_check_mark: |
| `["problem","monte carlo","euro_option_vec"]` | 0.46 (15%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["problem","raytrace","raytrace"]` | 0.80 (15%) :white_check_mark: | 1.02 (1%) :x: |
| `["problem","seismic",("seismic","Float32")]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","seismic",("seismic","Float64")]` | 0.79 (15%) :white_check_mark: | 1.00 (1%)  |
| `["problem","spellcheck","spellcheck"]` | 0.54 (15%) :white_check_mark: | 0.73 (1%) :white_check_mark: |
| `["problem","stockcorr","stockcorr"]` | 1.20 (15%) :x: | 1.01 (1%)  |
| `["problem","ziggurat","ziggurat"]` | 1.16 (15%) :x: | 1.03 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","BigInt")]` | 0.78 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigInt}")]` | 0.70 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float32}")]` | 0.72 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float64}")]` | 0.71 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Float32")]` | 0.80 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigFloat","Float64")]` | 0.80 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","BigFloat")]` | 0.78 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","BigInt","Complex{BigFloat}")]` | 0.78 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigInt")]` | 0.79 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigInt}")]` | 0.70 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float32}")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float64}")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float32")]` | 0.80 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float64")]` | 0.80 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigFloat")]` | 0.70 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigFloat}")]` | 0.71 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","BigFloat")]` | 0.71 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigFloat}")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float32}","Float64")]` | 0.41 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Float64}","BigFloat")]` | 0.70 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigFloat}")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("add","Complex{Int64}","Float32")]` | 0.32 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","Float64")]` | 0.35 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{Int64}","UInt64")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float32")]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float64")]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","BigFloat")]` | 0.79 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Float32","Complex{BigFloat}")]` | 0.83 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("add","Float32","Complex{Int64}")]` | 0.34 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Complex{UInt64}")]` | 0.43 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float32","Float32")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","BigFloat")]` | 0.80 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","Complex{BigFloat}")]` | 0.80 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("add","Float64","Complex{Float32}")]` | 0.41 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{Int64}")]` | 0.39 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Float64","Complex{UInt64}")]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","Int64","Int64")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","Complex{Int64}")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("add","UInt64","UInt64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","BigFloat","BigInt")]` | 0.80 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 0.70 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 2.11 (50%) :x: | 4.29 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 2.11 (50%) :x: | 4.29 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 2.12 (50%) :x: | 4.29 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 2.14 (50%) :x: | 4.29 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Float32")]` | 0.82 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","BigFloat","Float64")]` | 0.83 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 0.72 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 0.67 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 1.46 (50%)  | 1.88 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 1.45 (50%)  | 1.88 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 1.54 (50%) :x: | 2.10 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 1.53 (50%) :x: | 2.10 (1%) :x: |
| `["scalar","arithmetic",("div","BigInt","Int64")]` | 0.36 (50%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","BigInt","UInt64")]` | 0.36 (50%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigInt")]` | 0.79 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float32")]` | 0.79 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float64")]` | 0.79 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigInt}")]` | 0.72 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Int64}")]` | 0.69 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{UInt64}")]` | 0.67 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 0.39 (50%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 0.40 (50%) :white_check_mark: | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Float32}","BigFloat")]` | 0.81 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Float64}","BigFloat")]` | 0.81 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 0.55 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigInt}")]` | 0.71 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Int64}")]` | 0.71 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 0.54 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigInt}")]` | 0.68 (50%)  | 1.05 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","BigFloat")]` | 0.87 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 0.71 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{BigInt}")]` | 0.69 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float32","Complex{UInt64}")]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Float64","BigFloat")]` | 0.88 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 0.71 (50%)  | 1.07 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 0.70 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Float64","Complex{Float32}")]` | 1.60 (50%) :x: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","Int64","BigInt")]` | 0.62 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 0.68 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 0.68 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","Int64","Int64")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("div","UInt64","BigInt")]` | 0.62 (50%)  | 0.93 (1%) :white_check_mark: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 0.68 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 0.67 (50%)  | 1.03 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","BigInt")]` | 0.77 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigInt}")]` | 0.75 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float32}")]` | 0.75 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float64}")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Float32")]` | 0.79 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","BigFloat","Float64")]` | 0.79 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","BigFloat")]` | 0.77 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigFloat}")]` | 0.75 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigInt")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigInt}")]` | 0.70 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float32}")]` | 0.69 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float64}")]` | 0.70 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float32")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float64")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigFloat")]` | 0.75 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigFloat}")]` | 0.70 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigFloat")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigFloat}")]` | 0.68 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Int64}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigFloat")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigFloat}")]` | 0.69 (50%)  | 1.09 (1%) :x: |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float32}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float64}")]` | 0.47 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Float32","BigFloat")]` | 0.79 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","Float32","Complex{BigFloat}")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","BigFloat")]` | 0.79 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","Complex{BigFloat}")]` | 0.76 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("mul","Float64","Float64")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","Int64","Int64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("mul","UInt64","UInt64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","BigFloat","BigInt")]` | 0.76 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigInt}")]` | 0.66 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float32}")]` | 0.67 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float64}")]` | 0.68 (50%)  | 1.04 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Float32")]` | 0.79 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigFloat","Float64")]` | 0.78 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","BigFloat")]` | 0.76 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigFloat}")]` | 0.70 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigInt")]` | 0.76 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigInt}")]` | 0.70 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float32}")]` | 0.75 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float64}")]` | 0.75 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float32")]` | 0.78 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float64")]` | 0.77 (50%)  | 1.11 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigFloat")]` | 0.70 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigFloat}")]` | 0.71 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigFloat")]` | 0.71 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigFloat}")]` | 0.77 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float32}","Float64")]` | 0.41 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigFloat")]` | 0.70 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigFloat}")]` | 0.77 (50%)  | 1.12 (1%) :x: |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float32")]` | 0.44 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float64")]` | 0.33 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{Int64}","UInt64")]` | 0.37 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigInt")]` | 0.48 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float32")]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float64")]` | 0.42 (50%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float32","BigFloat")]` | 0.78 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Float32","Complex{BigFloat}")]` | 0.71 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Float32","Float32")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","arithmetic",("sub","Float64","BigFloat")]` | 0.78 (50%)  | 1.13 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","Complex{BigFloat}")]` | 0.72 (50%)  | 1.06 (1%) :x: |
| `["scalar","arithmetic",("sub","Float64","Float64")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("add","Complex{BigFloat}")]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{BigInt}")]` | 0.86 (40%)  | 1.06 (1%) :x: |
| `["scalar","fastmath",("div","Complex{Float32}")]` | 0.53 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Complex{Float64}")]` | 0.48 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("div","Int64")]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","BigFloat")]` | 0.60 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("mul","Complex{UInt64}")]` | 0.56 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","fastmath",("sub","BigFloat")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp","normal path, k = 2","Float 64")]` | 0.39 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exp","small argument path","Float 32")]` | 0.26 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("exponent","subnorm","Float32")]` | 0.58 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","inf","Float32")]` | 1.44 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","inf","Float64")]` | 1.53 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("frexp","norm","Float32")]` | 1.44 (40%) :x: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","inf -> inf","Float32")]` | 0.16 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","inf -> inf","Float64")]` | 0.17 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float32")]` | 0.03 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> inf","Float64")]` | 0.03 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> subnorm","Float32")]` | 0.42 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","norm -> subnorm","Float64")]` | 0.41 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> norm","Float32")]` | 0.07 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> norm","Float64")]` | 0.08 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> subnorm","Float32")]` | 0.29 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","floatexp",("ldexp","subnorm -> subnorm","Float64")]` | 0.28 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","intfuncs",("nextpow2","Int64","+")]` | 0.16 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","intfuncs",("nextpow2","Int64","-")]` | 0.16 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","intfuncs",("nextpow2","UInt64","+")]` | 0.11 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","intfuncs",("nextpow2","UInt64","-")]` | 0.12 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","intfuncs",("prevpow2","BigInt","+")]` | 0.59 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","intfuncs",("prevpow2","Int64","+")]` | 0.11 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","intfuncs",("prevpow2","Int64","-")]` | 0.11 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","intfuncs",("prevpow2","UInt64","+")]` | 0.09 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","intfuncs",("prevpow2","UInt64","-")]` | 0.08 (25%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["scalar","iteration","in"]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Complex{Int64}")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","Int64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isequal","UInt64")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("iseven","Int64")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("iseven","UInt64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","BigInt")]` | 0.01 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Float32}")]` | 0.44 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Float64}")]` | 0.41 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{Int64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Complex{UInt64}")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Float32")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","Int64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isfinite","UInt64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float32}")]` | 0.47 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Float64}")]` | 0.50 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{Int64}")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Complex{UInt64}")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Float64")]` | 0.67 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","Int64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinf","UInt64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","BigInt")]` | 0.01 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{Float32}")]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{Float64}")]` | 0.70 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{Int64}")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Complex{UInt64}")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Float32")]` | 0.51 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Float64")]` | 0.75 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","Int64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isinteger","UInt64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isless","Int64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isless","UInt64")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","BigInt")]` | 0.01 (40%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{Float64}")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{Int64}")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Complex{UInt64}")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Float32")]` | 0.63 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Float64")]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","Int64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isnan","UInt64")]` | 0.01 (25%) :white_check_mark: | 1.00 (1%)  |
| `["scalar","predicate",("isodd","Int64")]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","fannkuch"]` | 0.82 (15%) :white_check_mark: | 1.17 (1%) :x: |
| `["shootout","fasta"]` | 1.08 (15%)  | 0.99 (1%) :white_check_mark: |
| `["shootout","k_nucleotide"]` | 0.58 (15%) :white_check_mark: | 0.37 (1%) :white_check_mark: |
| `["shootout","mandelbrot"]` | 0.99 (15%)  | 0.98 (1%) :white_check_mark: |
| `["shootout","nbody"]` | 0.94 (15%)  | 1.04 (1%) :x: |
| `["shootout","nbody_vec"]` | 0.02 (15%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["shootout","pidigits"]` | 0.73 (15%) :white_check_mark: | 1.00 (1%)  |
| `["shootout","regex_dna"]` | 1.01 (15%)  | 1.05 (1%) :x: |
| `["shootout","revcomp"]` | 21.75 (25%) :x: | 1.20 (1%) :x: |
| `["shootout","spectralnorm"]` | 1.00 (15%)  | 1.35 (1%) :x: |
| `["simd",("axpy!","Float32",4095)]` | 0.37 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Float32",4096)]` | 0.35 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Float64",4095)]` | 0.36 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Float64",4096)]` | 0.36 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Int32",4095)]` | 0.47 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Int32",4096)]` | 0.45 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Int64",4095)]` | 0.75 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("axpy!","Int64",4096)]` | 0.76 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4095)]` | 0.45 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float32",4096)]` | 0.44 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4095)]` | 0.20 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Float64",4096)]` | 0.20 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4095)]` | 0.19 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int32",4096)]` | 0.19 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4095)]` | 0.20 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("conditional_loop!","Int64",4096)]` | 0.20 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4095)]` | 0.43 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float32",4096)]` | 0.38 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4095)]` | 0.40 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Float64",4096)]` | 0.41 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Int32",4095)]` | 0.52 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("inner","Int32",4096)]` | 0.50 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("local_arrays","Float32",4095)]` | 19.74 (20%) :x: | 5.40 (1%) :x: |
| `["simd",("local_arrays","Float32",4096)]` | 20.85 (20%) :x: | 5.40 (1%) :x: |
| `["simd",("local_arrays","Float64",4095)]` | 21.06 (20%) :x: | 3.61 (1%) :x: |
| `["simd",("local_arrays","Float64",4096)]` | 19.41 (20%) :x: | 3.61 (1%) :x: |
| `["simd",("local_arrays","Int32",4095)]` | 31.31 (20%) :x: | 5.40 (1%) :x: |
| `["simd",("local_arrays","Int32",4096)]` | 30.50 (20%) :x: | 5.40 (1%) :x: |
| `["simd",("local_arrays","Int64",4095)]` | 20.57 (20%) :x: | 3.60 (1%) :x: |
| `["simd",("local_arrays","Int64",4096)]` | 19.69 (20%) :x: | 3.60 (1%) :x: |
| `["simd",("manual_example!","Float32",4095)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float32",4096)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4095)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Float64",4096)]` | 0.39 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Int32",4095)]` | 0.38 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Int32",4096)]` | 0.38 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Int64",4095)]` | 0.44 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("manual_example!","Int64",4096)]` | 0.44 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float32",4095)]` | 0.71 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4095)]` | 0.60 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Float64",4096)]` | 0.49 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4095)]` | 0.44 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int32",4096)]` | 0.44 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int64",4095)]` | 0.45 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("sum_reduce","Int64",4096)]` | 0.44 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int64",4095)]` | 0.34 (20%) :white_check_mark: | 1.00 (1%)  |
| `["simd",("two_reductions","Int64",4096)]` | 0.34 (20%) :white_check_mark: | 1.00 (1%)  |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 1.47 (30%) :x: | 1.20 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","descending")]` | 0.98 (30%)  | 1.20 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","ones")]` | 0.69 (30%) :white_check_mark: | 1.20 (1%) :x: |
| `["sort","insertionsort",("sort! forwards","random")]` | 0.80 (30%)  | 1.20 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ascending")]` | 0.98 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","descending")]` | 0.63 (30%) :white_check_mark: | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","ones")]` | 0.78 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sort! reverse","random")]` | 0.80 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 1.35 (30%) :x: | 1.00 (1%)  |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 0.85 (30%)  | 1.17 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 1.35 (30%) :x: | 1.17 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 0.88 (30%)  | 1.13 (1%) :x: |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 1.29 (30%)  | 1.13 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 1.35 (30%) :x: | 1.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 0.86 (30%)  | 1.14 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 0.92 (30%)  | 1.11 (1%) :x: |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 1.30 (30%)  | 1.11 (1%) :x: |
| `["sort","issorted",("forwards","ascending")]` | 0.54 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sort","issorted",("reverse","ascending")]` | 3.27 (30%) :x: | 1.20 (1%) :x: |
| `["sort","issorted",("reverse","descending")]` | 0.57 (30%) :white_check_mark: | 1.20 (1%) :x: |
| `["sort","issorted",("reverse","ones")]` | 0.83 (30%)  | 1.20 (1%) :x: |
| `["sort","issorted",("reverse","random")]` | 3.18 (30%) :x: | 1.20 (1%) :x: |
| `["sort","quicksort",("sort forwards","ones")]` | 0.67 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sort","quicksort",("sort! forwards","ascending")]` | 0.86 (30%)  | 1.20 (1%) :x: |
| `["sort","quicksort",("sort! forwards","descending")]` | 0.88 (30%)  | 1.20 (1%) :x: |
| `["sort","quicksort",("sort! forwards","ones")]` | 0.66 (30%) :white_check_mark: | 1.20 (1%) :x: |
| `["sort","quicksort",("sort! forwards","random")]` | 0.87 (30%)  | 1.20 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ascending")]` | 0.82 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! reverse","descending")]` | 0.79 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! reverse","ones")]` | 0.81 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sort! reverse","random")]` | 0.87 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 1.20 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 1.18 (30%)  | 1.17 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 1.12 (30%)  | 1.13 (1%) :x: |
| `["sort","quicksort",("sortperm! forwards","random")]` | 1.01 (30%)  | 1.13 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 1.18 (30%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 1.21 (30%)  | 1.14 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 1.11 (30%)  | 1.11 (1%) :x: |
| `["sort","quicksort",("sortperm! reverse","random")]` | 1.00 (30%)  | 1.11 (1%) :x: |
| `["sparse","arithmetic",("unary minus",(20000,20000))]` | 1.96 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",10)]` | 6.32 (30%) :x: | 1.02 (1%) :x: |
| `["sparse","index",("spmat","array",100)]` | 5.60 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","array",1000)]` | 4.50 (30%) :x: | 1.00 (1%)  |
| `["sparse","index",("spmat","col","array",10)]` | 6.16 (30%) :x: | 1.11 (1%) :x: |
| `["sparse","index",("spmat","col","array",100)]` | 4.87 (30%) :x: | 1.02 (1%) :x: |
| `["sparse","index",("spmat","col","array",1000)]` | 1.72 (30%) :x: | 1.01 (1%)  |
| `["sparse","index",("spmat","col","logical",10)]` | 1.01 (30%)  | 1.18 (1%) :x: |
| `["sparse","index",("spmat","col","logical",100)]` | 0.92 (30%)  | 1.04 (1%) :x: |
| `["sparse","index",("spmat","col","logical",1000)]` | 0.83 (30%)  | 1.03 (1%) :x: |
| `["sparse","index",("spmat","col","range",10)]` | 0.67 (30%) :white_check_mark: | 0.80 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",100)]` | 0.73 (30%)  | 0.83 (1%) :white_check_mark: |
| `["sparse","index",("spmat","col","range",1000)]` | 0.78 (30%)  | 0.98 (1%) :white_check_mark: |
| `["sparse","index",("spmat","logical",10)]` | 0.89 (30%)  | 1.09 (1%) :x: |
| `["sparse","index",("spmat","logical",100)]` | 1.31 (30%) :x: | 1.01 (1%)  |
| `["sparse","index",("spmat","range",10)]` | 0.89 (30%)  | 1.02 (1%) :x: |
| `["sparse","index",("spmat","row","array",10)]` | 0.66 (30%) :white_check_mark: | 0.51 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",100)]` | 0.43 (30%) :white_check_mark: | 0.35 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","array",1000)]` | 0.33 (30%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",10)]` | 0.61 (30%) :white_check_mark: | 0.67 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",100)]` | 0.44 (30%) :white_check_mark: | 0.37 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","logical",1000)]` | 0.29 (30%) :white_check_mark: | 0.29 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","range",10)]` | 0.49 (30%) :white_check_mark: | 0.46 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","range",100)]` | 0.31 (30%) :white_check_mark: | 0.21 (1%) :white_check_mark: |
| `["sparse","index",("spmat","row","range",1000)]` | 0.26 (30%) :white_check_mark: | 0.08 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",10)]` | 0.68 (30%) :white_check_mark: | 0.81 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",100)]` | 0.84 (30%)  | 0.81 (1%) :white_check_mark: |
| `["sparse","index",("spmat","splogical",1000)]` | 0.86 (30%)  | 0.88 (1%) :white_check_mark: |
| `["sparse","index",("spvec","array",1000)]` | 1.91 (30%) :x: | 1.69 (1%) :x: |
| `["sparse","index",("spvec","array",10000)]` | 0.95 (30%)  | 1.53 (1%) :x: |
| `["sparse","index",("spvec","array",100000)]` | 0.47 (30%) :white_check_mark: | 1.51 (1%) :x: |
| `["sparse","index",("spvec","integer",1000)]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",10000)]` | 0.54 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","integer",100000)]` | 0.57 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse","index",("spvec","logical",1000)]` | 1.57 (30%) :x: | 0.61 (1%) :white_check_mark: |
| `["sparse","index",("spvec","logical",10000)]` | 0.82 (30%)  | 0.52 (1%) :white_check_mark: |
| `["sparse","index",("spvec","logical",100000)]` | 0.81 (30%)  | 0.50 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",1000)]` | 0.00 (30%) :white_check_mark: | 0.05 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",10000)]` | 0.00 (30%) :white_check_mark: | 0.01 (1%) :white_check_mark: |
| `["sparse","index",("spvec","range",100000)]` | 0.00 (30%) :white_check_mark: | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 1.04 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 1.04 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(600,400))]` | 0.96 (30%)  | 0.01 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose!",(600,600))]` | 0.88 (30%)  | 0.01 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose",(600,400))]` | 0.97 (30%)  | 0.93 (1%) :white_check_mark: |
| `["sparse","transpose",("ctranspose",(600,600))]` | 0.99 (30%)  | 0.95 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose!",(20000,10000))]` | 1.00 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 1.00 (30%)  | 0.00 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose!",(600,400))]` | 0.91 (30%)  | 0.01 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose!",(600,600))]` | 0.93 (30%)  | 0.01 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose",(600,400))]` | 0.98 (30%)  | 0.90 (1%) :white_check_mark: |
| `["sparse","transpose",("transpose",(600,600))]` | 0.96 (30%)  | 0.93 (1%) :white_check_mark: |
| `["tuple","index",("sumelt","NTuple",30,Float32)]` | 0.29 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",30,Float64)]` | 0.29 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",60,Float32)]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",60,Float64)]` | 0.43 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","NTuple",8,Float64)]` | 0.53 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",3,Float32)]` | 0.50 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float32)]` | 0.04 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 0.02 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",60,Float32)]` | 0.02 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",60,Float64)]` | 0.02 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",8,Float32)]` | 0.13 (40%) :white_check_mark: | 1.00 (1%)  |
| `["tuple","index",("sumelt","TupleWrapper",8,Float64)]` | 0.15 (40%) :white_check_mark: | 1.00 (1%)  |

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

## Version Info

#### Primary Build

```
Julia Version 0.6.0-pre.beta.129
Commit 5e1cd27 (2017-04-13 19:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (4603.3203125 MB free)
Uptime: 2.7765814e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   56775370 s          0 s    8798923 s  2705045850 s         82 s
#2  3501 MHz  211489923 s          0 s    9641625 s  2550316124 s         30 s
#3  3501 MHz   47521194 s          0 s    5558128 s  2722256978 s         44 s
#4  3501 MHz   43114173 s          0 s    5503020 s  2726976681 s         15 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.9.1 (ORCJIT, haswell)

```

#### Comparison Build

```
Julia Version 0.4.7
Commit ae26b25 (2016-09-18 16:17 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (5379.34375 MB free)
Uptime: 2.7770758e7 sec
Load Avg:  1.0029296875  1.0146484375  1.04541015625
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz   56844907 s          0 s    8807412 s  2705460277 s         82 s
#2  3501 MHz  211931562 s          0 s    9648878 s  2550360855 s         30 s
#3  3501 MHz   47606256 s          0 s    5565148 s  2722658506 s         44 s
#4  3501 MHz   43184857 s          0 s    5509994 s  2727392751 s         15 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.3

```
