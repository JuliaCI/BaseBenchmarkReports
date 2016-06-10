# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@4f65737874bb60b9ce627aa8089657007ee0d232](https://github.com/JuliaLang/julia/commit/4f65737874bb60b9ce627aa8089657007ee0d232)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/4f65737874bb60b9ce627aa8089657007ee0d232#commitcomment-17816579)

*Tag Predicate:* `ALL`

*Daily Job:* 2016-06-10

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

| ID | time | GC time | memory | allocations |
|----|------|---------|--------|-------------|
| `["array","bool","bitarray_bool_load!"]` | 3.30 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","bool","bitarray_true_fill!"]` | 3.12 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","bool","bitarray_true_load!"]` | 2.41 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","bool","boolarray_bool_load!"]` | 1.30 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","bool","boolarray_true_fill!"]` | 33.37 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","bool","boolarray_true_load!"]` | 325.46 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","cat",("catnd",5)]` | 28.05 μs (15%) | 0.00 ns | 19.06 kb (1%) | 98 |
| `["array","cat",("catnd",500)]` | 1.85 ms (15%) | 0.00 ns | 11.46 mb (1%) | 110 |
| `["array","cat",("catnd_setind",5)]` | 10.42 μs (15%) | 0.00 ns | 15.98 kb (1%) | 40 |
| `["array","cat",("catnd_setind",500)]` | 1.56 ms (15%) | 0.00 ns | 11.46 mb (1%) | 43 |
| `["array","cat",("hcat",5)]` | 397.00 ns (15%) | 0.00 ns | 976.00 bytes (1%) | 3 |
| `["array","cat",("hcat",500)]` | 597.60 μs (15%) | 0.00 ns | 7.63 mb (1%) | 4 |
| `["array","cat",("hcat_setind",5)]` | 208.00 ns (15%) | 0.00 ns | 1.00 kb (1%) | 5 |
| `["array","cat",("hcat_setind",500)]` | 852.76 μs (15%) | 0.00 ns | 7.63 mb (1%) | 6 |
| `["array","cat",("hvcat",5)]` | 283.00 ns (15%) | 0.00 ns | 1.16 kb (1%) | 10 |
| `["array","cat",("hvcat",500)]` | 946.56 μs (15%) | 0.00 ns | 7.63 mb (1%) | 11 |
| `["array","cat",("hvcat_setind",5)]` | 258.00 ns (15%) | 0.00 ns | 1.13 kb (1%) | 9 |
| `["array","cat",("hvcat_setind",500)]` | 947.40 μs (15%) | 0.00 ns | 7.63 mb (1%) | 10 |
| `["array","cat",("vcat",5)]` | 678.00 ns (15%) | 0.00 ns | 1.08 kb (1%) | 7 |
| `["array","cat",("vcat",500)]` | 915.78 μs (15%) | 0.00 ns | 7.63 mb (1%) | 9 |
| `["array","cat",("vcat_setind",5)]` | 210.00 ns (15%) | 0.00 ns | 1.00 kb (1%) | 5 |
| `["array","cat",("vcat_setind",500)]` | 903.76 μs (15%) | 0.00 ns | 7.63 mb (1%) | 6 |
| `["array","comprehension",("collect","Array{Float64,1}")]` | 13.38 ms (15%) | 0.00 ns | 76.29 mb (1%) | 3 |
| `["array","comprehension",("collect","FloatRange{Float64}")]` | 40.02 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("collect","LinSpace{Float64}")]` | 40.01 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_collect","Array{Float64,1}")]` | 12.96 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_collect","FloatRange{Float64}")]` | 24.33 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_collect","LinSpace{Float64}")]` | 24.34 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_indexing","Array{Float64,1}")]` | 78.36 ms (30%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_indexing","FloatRange{Float64}")]` | 216.05 ms (30%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_indexing","LinSpace{Float64}")]` | 245.07 ms (30%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_iteration","Array{Float64,1}")]` | 79.14 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_iteration","FloatRange{Float64}")]` | 104.54 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","comprehension",("comprehension_iteration","LinSpace{Float64}")]` | 117.99 ms (15%) | 0.00 ns | 76.29 mb (1%) | 2 |
| `["array","growth",("append!",2048)]` | 3.53 μs (15%) | 0.00 ns | 53.36 kb (1%) | 0 |
| `["array","growth",("append!",256)]` | 430.00 ns (15%) | 0.00 ns | 4.75 kb (1%) | 0 |
| `["array","growth",("append!",8)]` | 27.00 ns (15%) | 0.00 ns | 132.00 bytes (1%) | 0 |
| `["array","growth",("prerend!",2048)]` | 2.61 μs (15%) | 0.00 ns | 49.80 kb (1%) | 0 |
| `["array","growth",("prerend!",256)]` | 693.00 ns (15%) | 0.00 ns | 5.08 kb (1%) | 0 |
| `["array","growth",("prerend!",8)]` | 42.00 ns (15%) | 0.00 ns | 132.00 bytes (1%) | 0 |
| `["array","growth",("push_multiple!",2048)]` | 7.94 μs (15%) | 0.00 ns | 32.04 kb (1%) | 0 |
| `["array","growth",("push_multiple!",256)]` | 1.17 μs (15%) | 0.00 ns | 6.02 kb (1%) | 0 |
| `["array","growth",("push_multiple!",8)]` | 37.00 ns (15%) | 0.00 ns | 132.00 bytes (1%) | 0 |
| `["array","growth",("push_single!",2048)]` | 2.99 μs (15%) | 0.00 ns | 10.45 kb (1%) | 8 |
| `["array","growth",("push_single!",256)]` | 2.84 μs (15%) | 0.00 ns | 7.34 kb (1%) | 8 |
| `["array","growth",("push_single!",8)]` | 2.81 μs (15%) | 0.00 ns | 6.94 kb (1%) | 8 |
| `["array","index","ind2sub"]` | 1.57 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index","sub2ind"]` | 1.34 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","1.0:1.0:1.0e8")]` | 616.83 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","100000000:-1:1")]` | 51.29 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","1:100000000")]` | 51.72 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","Array{Float32,2}")]` | 1.05 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","Array{Int32,2}")]` | 1.00 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 1.10 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 1.06 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.10 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.06 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.10 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.06 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","BitArray{2}")]` | 6.63 ms (40%) | 0.00 ns | 3.81 mb (1%) | 249489 |
| `["array","index",("sumcartesian","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.08 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.01 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcartesian","linspace(1.0,2.0,10000000)")]` | 94.97 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumcolon","1.0:1.0:1.0e8")]` | 245.73 ms (40%) | 0.00 ns | 762.94 mb (1%) | 4 |
| `["array","index",("sumcolon","100000000:-1:1")]` | 93.60 ms (40%) | 0.00 ns | 762.94 mb (1%) | 4 |
| `["array","index",("sumcolon","1:100000000")]` | 88.94 ms (40%) | 0.00 ns | 762.94 mb (1%) | 4 |
| `["array","index",("sumcolon","Array{Float32,2}")]` | 227.82 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1000 |
| `["array","index",("sumcolon","Array{Int32,2}")]` | 182.91 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1000 |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 238.12 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1000 |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 219.20 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1000 |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 255.04 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1500 |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 194.71 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1500 |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 236.91 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1000 |
| `["array","index",("sumcolon","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 192.38 μs (40%) | 0.00 ns | 1.05 mb (1%) | 1000 |
| `["array","index",("sumcolon","BitArray{2}")]` | 140.07 μs (40%) | 0.00 ns | 101.56 kb (1%) | 2000 |
| `["array","index",("sumcolon","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 318.64 μs (40%) | 0.00 ns | 1.08 mb (1%) | 1500 |
| `["array","index",("sumcolon","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 206.13 μs (40%) | 0.00 ns | 1.08 mb (1%) | 1500 |
| `["array","index",("sumcolon","linspace(1.0,2.0,10000000)")]` | 40.00 ms (40%) | 0.00 ns | 76.29 mb (1%) | 4 |
| `["array","index",("sumeach","1.0:1.0:1.0e8")]` | 616.21 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","100000000:-1:1")]` | 15.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","1:100000000")]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","Array{Float32,2}")]` | 192.34 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","Array{Int32,2}")]` | 20.02 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 192.37 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 94.95 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 1.10 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 1.06 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 1.10 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 1.06 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","BitArray{2}")]` | 5.37 ms (40%) | 0.00 ns | 3.81 mb (1%) | 249489 |
| `["array","index",("sumeach","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.08 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.01 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumeach","linspace(1.0,2.0,10000000)")]` | 96.03 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","1.0:1.0:1.0e8")]` | 615.53 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","100000000:-1:1")]` | 25.65 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","1:100000000")]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","Array{Float32,2}")]` | 192.34 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","Array{Int32,2}")]` | 87.13 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 192.35 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 102.63 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 3.29 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 3.29 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 3.29 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 3.29 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","BitArray{2}")]` | 5.22 ms (40%) | 0.00 ns | 3.81 mb (1%) | 249489 |
| `["array","index",("sumelt","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 4.17 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 4.14 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt","linspace(1.0,2.0,10000000)")]` | 94.89 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","1.0:1.0:1.0e8")]` | 615.59 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","100000000:-1:1")]` | 517.94 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","1:100000000")]` | 257.87 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","Array{Float32,2}")]` | 192.34 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","Array{Int32,2}")]` | 86.81 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 192.35 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 102.63 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 415.19 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 439.73 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 418.72 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 439.74 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","BitArray{2}")]` | 5.75 ms (40%) | 0.00 ns | 3.81 mb (1%) | 249489 |
| `["array","index",("sumelt_boundscheck","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.46 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.45 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumelt_boundscheck","linspace(1.0,2.0,10000000)")]` | 94.89 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","1.0:1.0:1.0e8")]` | 616.22 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","100000000:-1:1")]` | 15.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","1:100000000")]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","Array{Float32,2}")]` | 192.34 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","Array{Int32,2}")]` | 19.99 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 192.37 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 94.78 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 193.55 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 152.62 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 193.55 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 152.62 μs (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","BitArray{2}")]` | 5.37 ms (40%) | 0.00 ns | 3.81 mb (1%) | 249489 |
| `["array","index",("sumlinear","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.13 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 2.00 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlinear","linspace(1.0,2.0,10000000)")]` | 96.03 ms (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","index",("sumlogical","1.0:1.0:1.0e8")]` | 273.18 ms (40%) | 4.61 ms | 393.39 mb (1%) | 13 |
| `["array","index",("sumlogical","100000000:-1:1")]` | 242.12 ms (40%) | 4.62 ms | 393.39 mb (1%) | 13 |
| `["array","index",("sumlogical","1:100000000")]` | 240.77 ms (40%) | 4.62 ms | 393.39 mb (1%) | 13 |
| `["array","index",("sumlogical","Array{Float32,2}")]` | 269.22 μs (40%) | 0.00 ns | 843.98 kb (1%) | 1505 |
| `["array","index",("sumlogical","Array{Int32,2}")]` | 269.92 μs (40%) | 0.00 ns | 843.98 kb (1%) | 1505 |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 273.16 μs (40%) | 0.00 ns | 843.98 kb (1%) | 1505 |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 271.43 μs (40%) | 0.00 ns | 843.98 kb (1%) | 1505 |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 279.74 μs (40%) | 0.00 ns | 851.80 kb (1%) | 2005 |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 277.15 μs (40%) | 0.00 ns | 851.80 kb (1%) | 2005 |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 273.12 μs (40%) | 0.00 ns | 843.98 kb (1%) | 1505 |
| `["array","index",("sumlogical","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 272.85 μs (40%) | 0.00 ns | 843.98 kb (1%) | 1505 |
| `["array","index",("sumlogical","BitArray{2}")]` | 490.57 μs (40%) | 0.00 ns | 601.80 kb (1%) | 2005 |
| `["array","index",("sumlogical","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 521.22 μs (40%) | 0.00 ns | 1.40 mb (1%) | 4005 |
| `["array","index",("sumlogical","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 522.45 μs (40%) | 0.00 ns | 1.40 mb (1%) | 4005 |
| `["array","index",("sumlogical","linspace(1.0,2.0,10000000)")]` | 28.36 ms (40%) | 0.00 ns | 39.34 mb (1%) | 13 |
| `["array","index",("sumrange","1.0:1.0:1.0e8")]` | 251.02 ms (40%) | 6.23 ms | 762.94 mb (1%) | 6 |
| `["array","index",("sumrange","100000000:-1:1")]` | 112.58 ms (40%) | 6.23 ms | 762.94 mb (1%) | 6 |
| `["array","index",("sumrange","1:100000000")]` | 102.14 ms (40%) | 6.24 ms | 762.94 mb (1%) | 6 |
| `["array","index",("sumrange","Array{Float32,2}")]` | 237.92 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2000 |
| `["array","index",("sumrange","Array{Int32,2}")]` | 199.11 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2000 |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 241.22 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2000 |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 196.93 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2000 |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 245.76 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2500 |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 224.97 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2500 |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 231.31 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2000 |
| `["array","index",("sumrange","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 194.47 μs (40%) | 0.00 ns | 1.08 mb (1%) | 2000 |
| `["array","index",("sumrange","BitArray{2}")]` | 145.66 μs (40%) | 0.00 ns | 132.81 kb (1%) | 3000 |
| `["array","index",("sumrange","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 318.43 μs (40%) | 0.00 ns | 1.08 mb (1%) | 1500 |
| `["array","index",("sumrange","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 212.67 μs (40%) | 0.00 ns | 1.08 mb (1%) | 1500 |
| `["array","index",("sumrange","linspace(1.0,2.0,10000000)")]` | 43.56 ms (40%) | 3.49 ms | 76.29 mb (1%) | 6 |
| `["array","index",("sumvector","1.0:1.0:1.0e8")]` | 185.00 ns (40%) | 0.00 ns | 336.00 bytes (1%) | 4 |
| `["array","index",("sumvector","100000000:-1:1")]` | 208.00 ns (40%) | 0.00 ns | 320.00 bytes (1%) | 4 |
| `["array","index",("sumvector","1:100000000")]` | 174.00 ns (40%) | 0.00 ns | 320.00 bytes (1%) | 4 |
| `["array","index",("sumvector","Array{Float32,2}")]` | 30.01 μs (40%) | 0.00 ns | 62.63 kb (1%) | 1001 |
| `["array","index",("sumvector","Array{Int32,2}")]` | 30.18 μs (40%) | 0.00 ns | 62.63 kb (1%) | 1001 |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Float32,2}")]` | 30.93 μs (40%) | 0.00 ns | 62.63 kb (1%) | 1001 |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLF{Int32,2}")]` | 30.58 μs (40%) | 0.00 ns | 62.63 kb (1%) | 1001 |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Float32,2}")]` | 35.73 μs (40%) | 0.00 ns | 70.44 kb (1%) | 1501 |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLSLS{Int32,2}")]` | 35.70 μs (40%) | 0.00 ns | 70.44 kb (1%) | 1501 |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Float32,2}")]` | 30.92 μs (40%) | 0.00 ns | 62.63 kb (1%) | 1001 |
| `["array","index",("sumvector","BaseBenchmarks.ArrayBenchmarks.ArrayLS{Int32,2}")]` | 31.01 μs (40%) | 0.00 ns | 62.63 kb (1%) | 1001 |
| `["array","index",("sumvector","BitArray{2}")]` | 111.81 μs (40%) | 0.00 ns | 70.44 kb (1%) | 1501 |
| `["array","index",("sumvector","SubArray{Float32,2,Array{Float32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 64.38 μs (40%) | 0.00 ns | 187.63 kb (1%) | 3501 |
| `["array","index",("sumvector","SubArray{Int32,2,Array{Int32,2},Tuple{UnitRange{Int64},UnitRange{Int64}},false}")]` | 64.65 μs (40%) | 0.00 ns | 187.63 kb (1%) | 3501 |
| `["array","index",("sumvector","linspace(1.0,2.0,10000000)")]` | 193.00 ns (40%) | 0.00 ns | 336.00 bytes (1%) | 4 |
| `["array","reverse","rev_load_fast!"]` | 669.60 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","reverse","rev_load_slow!"]` | 1.82 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","reverse","rev_loadmul_fast!"]` | 3.10 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","reverse","rev_loadmul_slow!"]` | 3.35 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["array","setindex!",("setindex!",1)]` | 800.00 ns (15%) | 0.00 ns | 352.00 bytes (1%) | 8 |
| `["array","setindex!",("setindex!",2)]` | 778.00 ns (15%) | 0.00 ns | 352.00 bytes (1%) | 8 |
| `["array","setindex!",("setindex!",3)]` | 865.00 ns (15%) | 0.00 ns | 352.00 bytes (1%) | 8 |
| `["array","setindex!",("setindex!",4)]` | 865.00 ns (15%) | 0.00 ns | 352.00 bytes (1%) | 8 |
| `["array","setindex!",("setindex!",5)]` | 833.00 ns (15%) | 0.00 ns | 352.00 bytes (1%) | 8 |
| `["array","subarray",("lucompletepivCopy!",100)]` | 1.96 ms (15%) | 0.00 ns | 5.84 mb (1%) | 2225 |
| `["array","subarray",("lucompletepivCopy!",1000)]` | 2.85 s (15%) | 999.52 ms | 5.03 gb (1%) | 26829 |
| `["array","subarray",("lucompletepivCopy!",250)]` | 40.61 ms (15%) | 14.05 ms | 83.61 mb (1%) | 5675 |
| `["array","subarray",("lucompletepivCopy!",500)]` | 340.83 ms (15%) | 130.05 ms | 651.65 mb (1%) | 11425 |
| `["array","subarray",("lucompletepivSub!",100)]` | 1.97 ms (15%) | 0.00 ns | 5.84 mb (1%) | 2225 |
| `["array","subarray",("lucompletepivSub!",1000)]` | 2.85 s (15%) | 1.00 s | 5.03 gb (1%) | 26829 |
| `["array","subarray",("lucompletepivSub!",250)]` | 40.61 ms (15%) | 14.02 ms | 83.61 mb (1%) | 5675 |
| `["array","subarray",("lucompletepivSub!",500)]` | 340.45 ms (15%) | 130.07 ms | 651.65 mb (1%) | 11425 |
| `["io","read","readstring"]` | 32.00 ns (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["io","read"]` | 14.59 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","arithmetic",("*","Bidiagonal","Bidiagonal",1024)]` | 49.38 ms (30%) | 0.00 ns | 24.00 mb (1%) | 7 |
| `["linalg","arithmetic",("*","Bidiagonal","Bidiagonal",256)]` | 920.73 μs (30%) | 0.00 ns | 1.50 mb (1%) | 7 |
| `["linalg","arithmetic",("*","Bidiagonal","Vector",1024)]` | 1.04 ms (30%) | 0.00 ns | 8.01 mb (1%) | 4 |
| `["linalg","arithmetic",("*","Bidiagonal","Vector",256)]` | 56.10 μs (30%) | 0.00 ns | 514.22 kb (1%) | 4 |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",1024)]` | 1.89 μs (30%) | 0.00 ns | 8.30 kb (1%) | 7 |
| `["linalg","arithmetic",("*","Diagonal","Diagonal",256)]` | 1.14 μs (30%) | 0.00 ns | 2.28 kb (1%) | 6 |
| `["linalg","arithmetic",("*","Diagonal","Vector",1024)]` | 1.94 μs (30%) | 0.00 ns | 8.30 kb (1%) | 7 |
| `["linalg","arithmetic",("*","Diagonal","Vector",256)]` | 1.15 μs (30%) | 0.00 ns | 2.28 kb (1%) | 6 |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",1024)]` | 34.60 ms (30%) | 0.00 ns | 8.00 mb (1%) | 4 |
| `["linalg","arithmetic",("*","LowerTriangular","LowerTriangular",256)]` | 1.07 ms (30%) | 0.00 ns | 512.13 kb (1%) | 4 |
| `["linalg","arithmetic",("*","LowerTriangular","Vector",1024)]` | 114.89 μs (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","LowerTriangular","Vector",256)]` | 9.07 μs (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","Matrix","Matrix",1024)]` | 47.51 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("*","Matrix","Matrix",256)]` | 827.50 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("*","Matrix","Vector",1024)]` | 220.04 μs (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","Matrix","Vector",256)]` | 11.64 μs (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","SymTridiagonal","SymTridiagonal",1024)]` | 49.37 ms (30%) | 0.00 ns | 24.00 mb (1%) | 7 |
| `["linalg","arithmetic",("*","SymTridiagonal","SymTridiagonal",256)]` | 916.91 μs (30%) | 0.00 ns | 1.50 mb (1%) | 7 |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",1024)]` | 1.78 μs (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","SymTridiagonal","Vector",256)]` | 660.00 ns (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","Tridiagonal","Tridiagonal",1024)]` | 49.40 ms (30%) | 0.00 ns | 24.00 mb (1%) | 9 |
| `["linalg","arithmetic",("*","Tridiagonal","Tridiagonal",256)]` | 921.84 μs (30%) | 0.00 ns | 1.50 mb (1%) | 9 |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",1024)]` | 1.94 μs (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","Tridiagonal","Vector",256)]` | 646.00 ns (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",1024)]` | 34.66 ms (30%) | 0.00 ns | 8.00 mb (1%) | 4 |
| `["linalg","arithmetic",("*","UpperTriangular","UpperTriangular",256)]` | 1.07 ms (30%) | 0.00 ns | 512.13 kb (1%) | 4 |
| `["linalg","arithmetic",("*","UpperTriangular","Vector",1024)]` | 105.03 μs (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("*","UpperTriangular","Vector",256)]` | 8.78 μs (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",1024)]` | 3.81 μs (30%) | 0.00 ns | 32.59 kb (1%) | 9 |
| `["linalg","arithmetic",("+","Bidiagonal","Bidiagonal",256)]` | 1.52 μs (30%) | 0.00 ns | 8.59 kb (1%) | 9 |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",1024)]` | 883.00 ns (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("+","Diagonal","Diagonal",256)]` | 364.00 ns (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",1024)]` | 1.14 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("+","LowerTriangular","LowerTriangular",256)]` | 48.16 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("+","Matrix","Matrix",1024)]` | 1.13 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("+","Matrix","Matrix",256)]` | 49.27 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",1024)]` | 1.76 μs (30%) | 0.00 ns | 16.31 kb (1%) | 5 |
| `["linalg","arithmetic",("+","SymTridiagonal","SymTridiagonal",256)]` | 774.00 ns (30%) | 0.00 ns | 4.31 kb (1%) | 5 |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",1024)]` | 3.55 μs (30%) | 0.00 ns | 32.59 kb (1%) | 8 |
| `["linalg","arithmetic",("+","Tridiagonal","Tridiagonal",256)]` | 1.52 μs (30%) | 0.00 ns | 8.59 kb (1%) | 8 |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",1024)]` | 1.14 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("+","UpperTriangular","UpperTriangular",256)]` | 48.85 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("+","Vector","Vector",1024)]` | 920.00 ns (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("+","Vector","Vector",256)]` | 343.00 ns (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",1024)]` | 3.72 μs (30%) | 0.00 ns | 32.59 kb (1%) | 9 |
| `["linalg","arithmetic",("-","Bidiagonal","Bidiagonal",256)]` | 1.57 μs (30%) | 0.00 ns | 8.59 kb (1%) | 9 |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",1024)]` | 895.00 ns (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("-","Diagonal","Diagonal",256)]` | 406.00 ns (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",1024)]` | 1.14 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("-","LowerTriangular","LowerTriangular",256)]` | 47.93 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("-","Matrix","Matrix",1024)]` | 1.13 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("-","Matrix","Matrix",256)]` | 48.66 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",1024)]` | 1.67 μs (30%) | 0.00 ns | 16.31 kb (1%) | 5 |
| `["linalg","arithmetic",("-","SymTridiagonal","SymTridiagonal",256)]` | 832.00 ns (30%) | 0.00 ns | 4.31 kb (1%) | 5 |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",1024)]` | 3.60 μs (30%) | 0.00 ns | 32.59 kb (1%) | 8 |
| `["linalg","arithmetic",("-","Tridiagonal","Tridiagonal",256)]` | 1.30 μs (30%) | 0.00 ns | 8.59 kb (1%) | 8 |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",1024)]` | 1.13 ms (30%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","arithmetic",("-","UpperTriangular","UpperTriangular",256)]` | 47.70 μs (30%) | 0.00 ns | 512.11 kb (1%) | 3 |
| `["linalg","arithmetic",("-","Vector","Vector",1024)]` | 916.00 ns (30%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","arithmetic",("-","Vector","Vector",256)]` | 343.00 ns (30%) | 0.00 ns | 2.14 kb (1%) | 2 |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",1024)]` | 4.67 μs (30%) | 0.00 ns | 8.30 kb (1%) | 7 |
| `["linalg","arithmetic",("/","Diagonal","Diagonal",256)]` | 1.84 μs (30%) | 0.00 ns | 2.28 kb (1%) | 6 |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",1024)]` | 38.43 ms (30%) | 0.00 ns | 8.00 mb (1%) | 4 |
| `["linalg","arithmetic",("/","LowerTriangular","LowerTriangular",256)]` | 1.30 ms (30%) | 0.00 ns | 512.13 kb (1%) | 4 |
| `["linalg","arithmetic",("/","Matrix","Matrix",1024)]` | 102.74 ms (30%) | 5.04 ms | 40.01 mb (1%) | 20 |
| `["linalg","arithmetic",("/","Matrix","Matrix",256)]` | 2.52 ms (30%) | 0.00 ns | 2.50 mb (1%) | 20 |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",1024)]` | 33.65 ms (30%) | 0.00 ns | 8.00 mb (1%) | 4 |
| `["linalg","arithmetic",("/","UpperTriangular","UpperTriangular",256)]` | 1.04 ms (30%) | 0.00 ns | 512.13 kb (1%) | 4 |
| `["linalg","arithmetic",("\\","Bidiagonal","Vector",1024)]` | 8.40 μs (30%) | 0.00 ns | 8.13 kb (1%) | 1 |
| `["linalg","arithmetic",("\\","Bidiagonal","Vector",256)]` | 2.21 μs (30%) | 0.00 ns | 2.13 kb (1%) | 1 |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",1024)]` | 4.69 μs (30%) | 0.00 ns | 8.30 kb (1%) | 7 |
| `["linalg","arithmetic",("\\","Diagonal","Diagonal",256)]` | 1.84 μs (30%) | 0.00 ns | 2.28 kb (1%) | 6 |
| `["linalg","arithmetic",("\\","Diagonal","Vector",1024)]` | 4.71 μs (30%) | 0.00 ns | 8.30 kb (1%) | 7 |
| `["linalg","arithmetic",("\\","Diagonal","Vector",256)]` | 1.82 μs (30%) | 0.00 ns | 2.28 kb (1%) | 6 |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",1024)]` | 37.45 ms (30%) | 0.00 ns | 8.00 mb (1%) | 5 |
| `["linalg","arithmetic",("\\","LowerTriangular","LowerTriangular",256)]` | 1.24 ms (30%) | 0.00 ns | 512.14 kb (1%) | 5 |
| `["linalg","arithmetic",("\\","LowerTriangular","Vector",1024)]` | 524.34 μs (30%) | 0.00 ns | 8.16 kb (1%) | 3 |
| `["linalg","arithmetic",("\\","LowerTriangular","Vector",256)]` | 32.50 μs (30%) | 0.00 ns | 2.16 kb (1%) | 3 |
| `["linalg","arithmetic",("\\","Matrix","Matrix",1024)]` | 87.15 ms (30%) | 0.00 ns | 16.01 mb (1%) | 11 |
| `["linalg","arithmetic",("\\","Matrix","Matrix",256)]` | 2.25 ms (30%) | 0.00 ns | 1.00 mb (1%) | 11 |
| `["linalg","arithmetic",("\\","Matrix","Vector",1024)]` | 24.79 ms (30%) | 0.00 ns | 8.02 mb (1%) | 10 |
| `["linalg","arithmetic",("\\","Matrix","Vector",256)]` | 681.00 μs (30%) | 0.00 ns | 516.45 kb (1%) | 10 |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",1024)]` | 17.01 μs (30%) | 0.00 ns | 24.55 kb (1%) | 10 |
| `["linalg","arithmetic",("\\","SymTridiagonal","Vector",256)]` | 4.71 μs (30%) | 0.00 ns | 6.55 kb (1%) | 10 |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",1024)]` | 38.34 μs (30%) | 0.00 ns | 58.19 kb (1%) | 28 |
| `["linalg","arithmetic",("\\","Tridiagonal","Vector",256)]` | 14.28 μs (30%) | 0.00 ns | 21.66 kb (1%) | 20 |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",1024)]` | 37.63 ms (30%) | 0.00 ns | 8.00 mb (1%) | 5 |
| `["linalg","arithmetic",("\\","UpperTriangular","UpperTriangular",256)]` | 1.25 ms (30%) | 0.00 ns | 512.14 kb (1%) | 5 |
| `["linalg","arithmetic",("\\","UpperTriangular","Vector",1024)]` | 504.83 μs (30%) | 0.00 ns | 8.16 kb (1%) | 3 |
| `["linalg","arithmetic",("\\","UpperTriangular","Vector",256)]` | 31.34 μs (30%) | 0.00 ns | 2.16 kb (1%) | 3 |
| `["linalg","blas","asum"]` | 134.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","axpy!"]` | 202.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","blascopy!"]` | 137.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","dot"]` | 98.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","dotc"]` | 259.00 ns (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["linalg","blas","dotu"]` | 259.00 ns (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["linalg","blas","gbmv!"]` | 181.89 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","gbmv"]` | 183.37 μs (15%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","blas","gemm!"]` | 47.55 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","gemm"]` | 47.59 ms (15%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","blas","gemv!"]` | 249.19 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","gemv"]` | 236.60 μs (15%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","blas","ger!"]` | 793.23 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","her!"]` | 1.94 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","herk!"]` | 113.00 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","herk"]` | 112.84 ms (15%) | 0.00 ns | 16.00 mb (1%) | 3 |
| `["linalg","blas","nrm2"]` | 271.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","sbmv!"]` | 202.22 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","sbmv"]` | 205.96 μs (15%) | 0.00 ns | 8.14 kb (1%) | 2 |
| `["linalg","blas","scal!"]` | 212.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","scal"]` | 967.00 ns (15%) | 0.00 ns | 8.13 kb (1%) | 1 |
| `["linalg","blas","symm!"]` | 47.54 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","symm"]` | 47.62 ms (15%) | 0.00 ns | 8.00 mb (1%) | 2 |
| `["linalg","blas","symv!"]` | 111.64 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","symv"]` | 111.80 μs (15%) | 0.00 ns | 8.13 kb (1%) | 1 |
| `["linalg","blas","syr!"]` | 572.72 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","syrk!"]` | 28.40 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","syrk"]` | 28.61 ms (15%) | 0.00 ns | 8.00 mb (1%) | 3 |
| `["linalg","blas","trmm!"]` | 27.78 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","trmm"]` | 29.05 ms (15%) | 0.00 ns | 8.00 mb (1%) | 2 |
| `["linalg","blas","trmv!"]` | 112.25 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","trmv"]` | 110.00 μs (15%) | 0.00 ns | 8.13 kb (1%) | 1 |
| `["linalg","blas","trsm!"]` | 30.90 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","trsm"]` | 31.92 ms (15%) | 0.00 ns | 8.00 mb (1%) | 2 |
| `["linalg","blas","trsv!"]` | 113.89 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["linalg","blas","trsv"]` | 112.92 μs (20%) | 0.00 ns | 8.13 kb (1%) | 1 |
| `["linalg","factorization",("chol","Matrix",1024)]` | 12.83 ms (25%) | 0.00 ns | 8.00 mb (1%) | 6 |
| `["linalg","factorization",("chol","Matrix",256)]` | 391.36 μs (25%) | 0.00 ns | 512.17 kb (1%) | 6 |
| `["linalg","factorization",("cholfact","Matrix",1024)]` | 12.98 ms (25%) | 0.00 ns | 8.00 mb (1%) | 6 |
| `["linalg","factorization",("cholfact","Matrix",256)]` | 388.92 μs (25%) | 0.00 ns | 512.17 kb (1%) | 6 |
| `["linalg","factorization",("eig","Bidiagonal",1024)]` | 165.06 ms (25%) | 29.49 ms | 102.31 mb (1%) | 4591914 |
| `["linalg","factorization",("eig","Bidiagonal",256)]` | 8.06 ms (25%) | 0.00 ns | 6.07 mb (1%) | 262433 |
| `["linalg","factorization",("eig","Diagonal",1024)]` | 813.39 μs (25%) | 0.00 ns | 8.03 mb (1%) | 2061 |
| `["linalg","factorization",("eig","Diagonal",256)]` | 61.04 μs (25%) | 0.00 ns | 516.47 kb (1%) | 265 |
| `["linalg","factorization",("eig","LowerTriangular",1024)]` | 74.25 ms (25%) | 5.01 ms | 32.03 mb (1%) | 20 |
| `["linalg","factorization",("eig","LowerTriangular",256)]` | 2.27 ms (25%) | 0.00 ns | 2.01 mb (1%) | 19 |
| `["linalg","factorization",("eig","Matrix",1024)]` | 1.48 s (25%) | 5.11 ms | 32.32 mb (1%) | 115 |
| `["linalg","factorization",("eig","Matrix",256)]` | 51.76 ms (25%) | 0.00 ns | 2.09 mb (1%) | 78 |
| `["linalg","factorization",("eig","SymTridiagonal",1024)]` | 108.45 ms (25%) | 0.00 ns | 16.28 mb (1%) | 57 |
| `["linalg","factorization",("eig","SymTridiagonal",256)]` | 5.70 ms (25%) | 0.00 ns | 1.07 mb (1%) | 53 |
| `["linalg","factorization",("eig","UpperTriangular",1024)]` | 65.87 ms (25%) | 4.95 ms | 24.03 mb (1%) | 17 |
| `["linalg","factorization",("eig","UpperTriangular",256)]` | 1.94 ms (25%) | 0.00 ns | 1.51 mb (1%) | 16 |
| `["linalg","factorization",("eigfact","Bidiagonal",1024)]` | 164.76 ms (25%) | 29.15 ms | 102.31 mb (1%) | 4591914 |
| `["linalg","factorization",("eigfact","Bidiagonal",256)]` | 8.05 ms (25%) | 0.00 ns | 6.07 mb (1%) | 262433 |
| `["linalg","factorization",("eigfact","Diagonal",1024)]` | 822.36 μs (25%) | 0.00 ns | 8.03 mb (1%) | 2061 |
| `["linalg","factorization",("eigfact","Diagonal",256)]` | 59.35 μs (25%) | 0.00 ns | 516.47 kb (1%) | 265 |
| `["linalg","factorization",("eigfact","LowerTriangular",1024)]` | 74.19 ms (25%) | 4.89 ms | 32.03 mb (1%) | 20 |
| `["linalg","factorization",("eigfact","LowerTriangular",256)]` | 2.27 ms (25%) | 0.00 ns | 2.01 mb (1%) | 19 |
| `["linalg","factorization",("eigfact","Matrix",1024)]` | 1.48 s (25%) | 5.14 ms | 32.32 mb (1%) | 113 |
| `["linalg","factorization",("eigfact","Matrix",256)]` | 51.72 ms (25%) | 0.00 ns | 2.09 mb (1%) | 76 |
| `["linalg","factorization",("eigfact","SymTridiagonal",1024)]` | 108.49 ms (25%) | 0.00 ns | 16.28 mb (1%) | 57 |
| `["linalg","factorization",("eigfact","SymTridiagonal",256)]` | 5.70 ms (25%) | 0.00 ns | 1.07 mb (1%) | 53 |
| `["linalg","factorization",("eigfact","UpperTriangular",1024)]` | 65.92 ms (25%) | 4.91 ms | 24.03 mb (1%) | 17 |
| `["linalg","factorization",("eigfact","UpperTriangular",256)]` | 1.94 ms (25%) | 0.00 ns | 1.51 mb (1%) | 16 |
| `["linalg","factorization",("lu","Matrix",1024)]` | 32.38 ms (25%) | 4.91 ms | 24.02 mb (1%) | 24 |
| `["linalg","factorization",("lu","Matrix",256)]` | 807.35 μs (25%) | 0.00 ns | 1.50 mb (1%) | 24 |
| `["linalg","factorization",("lu","Tridiagonal",1024)]` | 13.54 ms (25%) | 5.12 ms | 24.64 mb (1%) | 13335 |
| `["linalg","factorization",("lu","Tridiagonal",256)]` | 491.54 μs (25%) | 0.00 ns | 1.64 mb (1%) | 2577 |
| `["linalg","factorization",("lufact","Matrix",1024)]` | 24.30 ms (25%) | 0.00 ns | 8.01 mb (1%) | 7 |
| `["linalg","factorization",("lufact","Matrix",256)]` | 660.69 μs (25%) | 0.00 ns | 514.30 kb (1%) | 7 |
| `["linalg","factorization",("lufact","Tridiagonal",1024)]` | 13.49 μs (25%) | 0.00 ns | 40.75 kb (1%) | 8 |
| `["linalg","factorization",("lufact","Tridiagonal",256)]` | 4.03 μs (25%) | 0.00 ns | 10.75 kb (1%) | 8 |
| `["linalg","factorization",("qr","Matrix",1024)]` | 159.80 ms (25%) | 4.89 ms | 32.60 mb (1%) | 2097 |
| `["linalg","factorization",("qr","Matrix",256)]` | 3.81 ms (25%) | 0.00 ns | 2.15 mb (1%) | 294 |
| `["linalg","factorization",("qrfact","Matrix",1024)]` | 63.16 ms (25%) | 0.00 ns | 8.56 mb (1%) | 17 |
| `["linalg","factorization",("qrfact","Matrix",256)]` | 1.82 ms (25%) | 0.00 ns | 656.44 kb (1%) | 13 |
| `["linalg","factorization",("schur","Matrix",1024)]` | 1.26 s (25%) | 0.00 ns | 16.30 mb (1%) | 25 |
| `["linalg","factorization",("schur","Matrix",256)]` | 47.62 ms (25%) | 0.00 ns | 1.08 mb (1%) | 21 |
| `["linalg","factorization",("schurfact","Matrix",1024)]` | 1.25 s (25%) | 0.00 ns | 16.30 mb (1%) | 25 |
| `["linalg","factorization",("schurfact","Matrix",256)]` | 47.73 ms (25%) | 0.00 ns | 1.08 mb (1%) | 21 |
| `["linalg","factorization",("svd","Bidiagonal",1024)]` | 63.62 ms (25%) | 8.25 ms | 48.13 mb (1%) | 30 |
| `["linalg","factorization",("svd","Bidiagonal",256)]` | 5.47 ms (25%) | 0.00 ns | 3.03 mb (1%) | 29 |
| `["linalg","factorization",("svd","Diagonal",1024)]` | 17.78 ms (25%) | 10.13 ms | 48.42 mb (1%) | 8240 |
| `["linalg","factorization",("svd","Diagonal",256)]` | 516.73 μs (25%) | 0.00 ns | 3.09 mb (1%) | 1317 |
| `["linalg","factorization",("svd","LowerTriangular",1024)]` | 572.20 ms (25%) | 10.18 ms | 64.13 mb (1%) | 26 |
| `["linalg","factorization",("svd","LowerTriangular",256)]` | 16.61 ms (25%) | 0.00 ns | 4.03 mb (1%) | 25 |
| `["linalg","factorization",("svd","Matrix",1024)]` | 595.38 ms (25%) | 9.86 ms | 56.13 mb (1%) | 24 |
| `["linalg","factorization",("svd","Matrix",256)]` | 17.60 ms (25%) | 0.00 ns | 3.53 mb (1%) | 23 |
| `["linalg","factorization",("svd","UpperTriangular",1024)]` | 573.44 ms (25%) | 10.03 ms | 64.13 mb (1%) | 26 |
| `["linalg","factorization",("svd","UpperTriangular",256)]` | 16.79 ms (25%) | 0.00 ns | 4.03 mb (1%) | 25 |
| `["linalg","factorization",("svdfact","Bidiagonal",1024)]` | 56.35 ms (25%) | 4.88 ms | 40.13 mb (1%) | 25 |
| `["linalg","factorization",("svdfact","Bidiagonal",256)]` | 5.39 ms (25%) | 0.00 ns | 2.53 mb (1%) | 24 |
| `["linalg","factorization",("svdfact","Diagonal",1024)]` | 21.52 ms (25%) | 10.37 ms | 56.42 mb (1%) | 8244 |
| `["linalg","factorization",("svdfact","Diagonal",256)]` | 609.50 μs (25%) | 0.00 ns | 3.59 mb (1%) | 1321 |
| `["linalg","factorization",("svdfact","LowerTriangular",1024)]` | 562.34 ms (25%) | 9.82 ms | 56.13 mb (1%) | 21 |
| `["linalg","factorization",("svdfact","LowerTriangular",256)]` | 16.53 ms (25%) | 0.00 ns | 3.53 mb (1%) | 20 |
| `["linalg","factorization",("svdfact","Matrix",1024)]` | 594.19 ms (25%) | 10.04 ms | 48.13 mb (1%) | 19 |
| `["linalg","factorization",("svdfact","Matrix",256)]` | 17.51 ms (25%) | 0.00 ns | 3.03 mb (1%) | 18 |
| `["linalg","factorization",("svdfact","UpperTriangular",1024)]` | 575.51 ms (25%) | 10.28 ms | 56.13 mb (1%) | 21 |
| `["linalg","factorization",("svdfact","UpperTriangular",256)]` | 16.69 ms (25%) | 0.00 ns | 3.53 mb (1%) | 20 |
| `["micro","fib"]` | 36.27 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["micro","mandel"]` | 115.33 μs (15%) | 0.00 ns | 4.44 kb (1%) | 1 |
| `["micro","parseint"]` | 213.69 μs (15%) | 0.00 ns | 140.59 kb (1%) | 3998 |
| `["micro","pisum"]` | 34.54 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["micro","quicksort"]` | 267.85 μs (15%) | 0.00 ns | 39.14 kb (1%) | 2 |
| `["micro","randmatmul"]` | 45.74 ms (15%) | 0.00 ns | 22.89 mb (1%) | 9 |
| `["micro","randmatstat"]` | 8.25 ms (15%) | 0.00 ns | 15.63 mb (1%) | 29019 |
| `["parallel","remotecall",("identity",1024)]` | 81.25 μs (15%) | 0.00 ns | 6.28 kb (1%) | 117 |
| `["parallel","remotecall",("identity",2)]` | 79.75 μs (15%) | 0.00 ns | 4.11 kb (1%) | 113 |
| `["parallel","remotecall",("identity",4096)]` | 89.48 μs (15%) | 0.00 ns | 12.44 kb (1%) | 122 |
| `["parallel","remotecall",("identity",512)]` | 81.51 μs (15%) | 0.00 ns | 5.31 kb (1%) | 121 |
| `["parallel","remotecall",("identity",64)]` | 80.71 μs (15%) | 0.00 ns | 4.28 kb (1%) | 115 |
| `["problem","fem","sparse_fem"]` | 219.32 ms (15%) | 13.95 ms | 119.02 mb (1%) | 201 |
| `["problem","go","go_game"]` | 721.50 ms (15%) | 113.60 ms | 388.15 mb (1%) | 3018122 |
| `["problem","grigoriadis khachiyan","grigoriadis_khachiyan"]` | 1.16 s (15%) | 506.56 ms | 2.04 gb (1%) | 1849188 |
| `["problem","imdb","centrality"]` | 868.84 ms (15%) | 39.32 ms | 81.95 mb (1%) | 683598 |
| `["problem","json","parse_json"]` | 1.09 ms (15%) | 0.00 ns | 502.77 kb (1%) | 15648 |
| `["problem","laplacian","laplace_iter_devec"]` | 13.81 ms (15%) | 0.00 ns | 64.17 kb (1%) | 5 |
| `["problem","laplacian","laplace_iter_sub"]` | 141.88 ms (15%) | 38.80 ms | 181.34 mb (1%) | 21507 |
| `["problem","laplacian","laplace_iter_vec"]` | 102.43 ms (15%) | 62.86 ms | 302.22 mb (1%) | 46083 |
| `["problem","laplacian","laplace_sparse_matvec"]` | 140.14 ms (15%) | 5.27 ms | 24.73 mb (1%) | 98694 |
| `["problem","monte carlo","euro_option_devec"]` | 33.10 ms (15%) | 0.00 ns | 19.40 mb (1%) | 508 |
| `["problem","monte carlo","euro_option_vec"]` | 60.42 ms (15%) | 18.78 ms | 95.81 mb (1%) | 4008 |
| `["problem","raytrace"]` | 1.13 s (15%) | 94.27 ms | 267.38 mb (1%) | 7277262 |
| `["problem","seismic",("seismic","Float32")]` | 613.37 μs (15%) | 0.00 ns | 938.16 kb (1%) | 15 |
| `["problem","seismic",("seismic","Float64")]` | 1.13 ms (15%) | 0.00 ns | 1.83 mb (1%) | 13 |
| `["problem","simplex"]` | 38.49 ms (15%) | 0.00 ns | 326.11 kb (1%) | 2414 |
| `["problem","spellcheck"]` | 9.50 s (15%) | 1.62 s | 4.34 gb (1%) | 80760530 |
| `["problem","stockcorr"]` | 430.01 ms (15%) | 236.24 ms | 231.63 mb (1%) | 30016 |
| `["problem","ziggurat"]` | 5.04 s (15%) | 1.73 s | 6.65 gb (1%) | 13000002 |
| `["scalar","arithmetic",("add","BigFloat","BigFloat")]` | 114.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","BigFloat","BigInt")]` | 202.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigFloat}")]` | 116.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","BigFloat","Complex{BigInt}")]` | 296.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float32}")]` | 310.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","BigFloat","Complex{Float64}")]` | 308.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","BigFloat","Complex{Int64}")]` | 241.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","BigFloat","Complex{UInt64}")]` | 233.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","BigFloat","Float32")]` | 213.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigFloat","Float64")]` | 213.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigFloat","Int64")]` | 141.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","BigFloat","UInt64")]` | 140.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","BigInt","BigFloat")]` | 202.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigInt","BigInt")]` | 134.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigInt","Complex{BigFloat}")]` | 204.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigInt","Complex{BigInt}")]` | 137.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigInt","Complex{Float32}")]` | 460.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","BigInt","Complex{Float64}")]` | 463.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","BigInt","Complex{Int64}")]` | 225.00 ns (50%) | 0.00 ns | 152.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","BigInt","Complex{UInt64}")]` | 209.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","BigInt","Float32")]` | 353.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","BigInt","Float64")]` | 353.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","BigInt","Int64")]` | 131.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","BigInt","UInt64")]` | 128.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigFloat")]` | 116.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","BigInt")]` | 204.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigFloat}")]` | 223.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{BigInt}")]` | 306.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float32}")]` | 388.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Float64}")]` | 387.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{Int64}")]` | 253.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Complex{UInt64}")]` | 245.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float32")]` | 215.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Float64")]` | 215.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","Int64")]` | 142.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","Complex{BigFloat}","UInt64")]` | 142.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigFloat")]` | 298.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{BigInt}","BigInt")]` | 137.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigFloat}")]` | 308.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{BigInt}")]` | 224.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float32}")]` | 664.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Float64}")]` | 670.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{Int64}")]` | 220.00 ns (50%) | 0.00 ns | 152.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Complex{UInt64}")]` | 213.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float32")]` | 457.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Float64")]` | 456.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","Complex{BigInt}","Int64")]` | 142.00 ns (50%) | 0.00 ns | 96.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{BigInt}","UInt64")]` | 130.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Complex{Float32}","BigFloat")]` | 312.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{Float32}","BigInt")]` | 456.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigFloat}")]` | 387.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{BigInt}")]` | 668.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float32}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","BigFloat")]` | 311.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{Float64}","BigInt")]` | 458.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigFloat}")]` | 387.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{BigInt}")]` | 669.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Float64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","BigFloat")]` | 241.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{Int64}","BigInt")]` | 223.00 ns (50%) | 0.00 ns | 152.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigFloat}")]` | 250.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{BigInt}")]` | 221.00 ns (50%) | 0.00 ns | 152.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{Int64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigFloat")]` | 234.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{UInt64}","BigInt")]` | 209.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigFloat}")]` | 248.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{BigInt}")]` | 213.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Complex{UInt64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","BigFloat")]` | 213.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Float32","BigInt")]` | 353.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Float32","Complex{BigFloat}")]` | 215.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Float32","Complex{BigInt}")]` | 458.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","Float32","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float32","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","BigFloat")]` | 213.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Float64","BigInt")]` | 354.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("add","Float64","Complex{BigFloat}")]` | 214.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Float64","Complex{BigInt}")]` | 457.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("add","Float64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Float64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","BigFloat")]` | 141.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","Int64","BigInt")]` | 131.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","Int64","Complex{BigFloat}")]` | 143.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","Int64","Complex{BigInt}")]` | 142.00 ns (50%) | 0.00 ns | 96.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("add","Int64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","Int64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","BigFloat")]` | 140.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","UInt64","BigInt")]` | 128.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","UInt64","Complex{BigFloat}")]` | 142.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("add","UInt64","Complex{BigInt}")]` | 131.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("add","UInt64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("add","UInt64","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","BigFloat","BigFloat")]` | 234.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("div","BigFloat","BigInt")]` | 234.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigFloat}")]` | 1.07 μs (50%) | 0.00 ns | 864.00 bytes (1%) | 17 |
| `["scalar","arithmetic",("div","BigFloat","Complex{BigInt}")]` | 1.28 μs (50%) | 0.00 ns | 1.11 kb (1%) | 23 |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float32}")]` | 390.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigFloat","Complex{Float64}")]` | 397.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigFloat","Complex{Int64}")]` | 398.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigFloat","Complex{UInt64}")]` | 390.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigFloat","Float32")]` | 246.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("div","BigFloat","Float64")]` | 246.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("div","BigFloat","Int64")]` | 102.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("div","BigFloat","UInt64")]` | 100.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("div","BigInt","BigFloat")]` | 348.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("div","BigInt","BigInt")]` | 455.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigInt","Complex{BigFloat}")]` | 1.19 μs (50%) | 0.00 ns | 928.00 bytes (1%) | 19 |
| `["scalar","arithmetic",("div","BigInt","Complex{BigInt}")]` | 1.43 μs (50%) | 0.00 ns | 1.17 kb (1%) | 25 |
| `["scalar","arithmetic",("div","BigInt","Complex{Float32}")]` | 715.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","BigInt","Complex{Float64}")]` | 718.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","BigInt","Complex{Int64}")]` | 720.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","BigInt","Complex{UInt64}")]` | 719.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","BigInt","Float32")]` | 478.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigInt","Float64")]` | 481.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","BigInt","Int64")]` | 358.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("div","BigInt","UInt64")]` | 357.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigFloat")]` | 346.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","BigInt")]` | 416.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{BigFloat}")]` | 1.30 μs (50%) | 0.00 ns | 1.15 kb (1%) | 23 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{BigInt}")]` | 1.57 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Float32}")]` | 1.54 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Float64}")]` | 1.55 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{Int64}")]` | 1.52 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Complex{UInt64}")]` | 1.60 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float32")]` | 434.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Float64")]` | 435.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","Int64")]` | 211.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("div","Complex{BigFloat}","UInt64")]` | 210.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigFloat")]` | 554.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("div","Complex{BigInt}","BigInt")]` | 757.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigFloat}")]` | 1.56 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{BigInt}")]` | 1.83 μs (50%) | 0.00 ns | 1.41 kb (1%) | 32 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Float32}")]` | 1.80 μs (50%) | 0.00 ns | 1.62 kb (1%) | 33 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Float64}")]` | 1.80 μs (50%) | 0.00 ns | 1.62 kb (1%) | 33 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{Int64}")]` | 2.00 μs (50%) | 0.00 ns | 1.59 kb (1%) | 38 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Complex{UInt64}")]` | 1.99 μs (50%) | 0.00 ns | 1.59 kb (1%) | 38 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float32")]` | 812.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Float64")]` | 810.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","Complex{BigInt}","Int64")]` | 649.00 ns (50%) | 0.00 ns | 480.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("div","Complex{BigInt}","UInt64")]` | 649.00 ns (50%) | 0.00 ns | 480.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("div","Complex{Float32}","BigFloat")]` | 491.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Complex{Float32}","BigInt")]` | 796.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{BigFloat}")]` | 1.54 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{BigInt}")]` | 1.82 μs (50%) | 0.00 ns | 1.62 kb (1%) | 33 |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Float32}")]` | 11.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Float64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{Int64}")]` | 20.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","Complex{UInt64}")]` | 20.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float32}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","BigFloat")]` | 491.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Complex{Float64}","BigInt")]` | 801.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{BigFloat}")]` | 1.54 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{BigInt}")]` | 1.83 μs (50%) | 0.00 ns | 1.62 kb (1%) | 33 |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{Float32}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{Float64}")]` | 13.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{Int64}")]` | 17.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","Complex{UInt64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Float64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","BigFloat")]` | 350.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("div","Complex{Int64}","BigInt")]` | 718.00 ns (50%) | 0.00 ns | 480.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigFloat}")]` | 1.52 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{BigInt}")]` | 2.00 μs (50%) | 0.00 ns | 1.59 kb (1%) | 38 |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Float32}")]` | 25.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Float64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{Int64}")]` | 10.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","Complex{UInt64}")]` | 8.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{Int64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigFloat")]` | 348.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("div","Complex{UInt64}","BigInt")]` | 714.00 ns (50%) | 0.00 ns | 480.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigFloat}")]` | 1.57 μs (50%) | 0.00 ns | 1.41 kb (1%) | 29 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{BigInt}")]` | 2.00 μs (50%) | 0.00 ns | 1.59 kb (1%) | 38 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{Float32}")]` | 13.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{Float64}")]` | 15.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{Int64}")]` | 8.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Complex{UInt64}")]` | 7.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Complex{UInt64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","BigFloat")]` | 318.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("div","Float32","BigInt")]` | 483.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Float32","Complex{BigFloat}")]` | 1.21 μs (50%) | 0.00 ns | 928.00 bytes (1%) | 19 |
| `["scalar","arithmetic",("div","Float32","Complex{BigInt}")]` | 1.44 μs (50%) | 0.00 ns | 1.17 kb (1%) | 25 |
| `["scalar","arithmetic",("div","Float32","Complex{Float32}")]` | 5.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","Complex{Float64}")]` | 7.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","Complex{Int64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","Complex{UInt64}")]` | 10.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float32","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","BigFloat")]` | 318.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("div","Float64","BigInt")]` | 478.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("div","Float64","Complex{BigFloat}")]` | 1.21 μs (50%) | 0.00 ns | 928.00 bytes (1%) | 19 |
| `["scalar","arithmetic",("div","Float64","Complex{BigInt}")]` | 1.49 μs (50%) | 0.00 ns | 1.17 kb (1%) | 25 |
| `["scalar","arithmetic",("div","Float64","Complex{Float32}")]` | 5.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","Complex{Float64}")]` | 7.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","Complex{Int64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","Complex{UInt64}")]` | 10.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Float64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","BigFloat")]` | 247.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("div","Int64","BigInt")]` | 427.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("div","Int64","Complex{BigFloat}")]` | 1.02 μs (50%) | 0.00 ns | 864.00 bytes (1%) | 17 |
| `["scalar","arithmetic",("div","Int64","Complex{BigInt}")]` | 1.27 μs (50%) | 0.00 ns | 1.11 kb (1%) | 23 |
| `["scalar","arithmetic",("div","Int64","Complex{Float32}")]` | 5.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","Complex{Float64}")]` | 7.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","Complex{Int64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","Complex{UInt64}")]` | 10.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","Int64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","BigFloat")]` | 246.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("div","UInt64","BigInt")]` | 440.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("div","UInt64","Complex{BigFloat}")]` | 991.00 ns (50%) | 0.00 ns | 864.00 bytes (1%) | 17 |
| `["scalar","arithmetic",("div","UInt64","Complex{BigInt}")]` | 1.23 μs (50%) | 0.00 ns | 1.11 kb (1%) | 23 |
| `["scalar","arithmetic",("div","UInt64","Complex{Float32}")]` | 5.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","Complex{Float64}")]` | 7.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","Complex{Int64}")]` | 14.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","Complex{UInt64}")]` | 10.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("div","UInt64","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","BigFloat","BigFloat")]` | 148.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("mul","BigFloat","BigInt")]` | 202.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigFloat}")]` | 252.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","BigFloat","Complex{BigInt}")]` | 357.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float32}")]` | 371.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Float64}")]` | 384.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","BigFloat","Complex{Int64}")]` | 203.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","BigFloat","Complex{UInt64}")]` | 203.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","BigFloat","Float32")]` | 212.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","BigFloat","Float64")]` | 213.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","BigFloat","Int64")]` | 101.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("mul","BigFloat","UInt64")]` | 99.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("mul","BigInt","BigFloat")]` | 201.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","BigInt","BigInt")]` | 133.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigFloat}")]` | 378.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","BigInt","Complex{BigInt}")]` | 217.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float32}")]` | 706.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","BigInt","Complex{Float64}")]` | 705.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","BigInt","Complex{Int64}")]` | 223.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","BigInt","Complex{UInt64}")]` | 224.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","BigInt","Float32")]` | 384.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","BigInt","Float64")]` | 387.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","BigInt","Int64")]` | 132.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","BigInt","UInt64")]` | 131.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigFloat")]` | 252.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","BigInt")]` | 377.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigFloat}")]` | 652.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{BigInt}")]` | 911.00 ns (50%) | 0.00 ns | 752.00 bytes (1%) | 16 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float32}")]` | 951.00 ns (50%) | 0.00 ns | 752.00 bytes (1%) | 16 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Float64}")]` | 958.00 ns (50%) | 0.00 ns | 752.00 bytes (1%) | 16 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{Int64}")]` | 604.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Complex{UInt64}")]` | 593.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float32")]` | 402.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Float64")]` | 402.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","Int64")]` | 205.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","Complex{BigFloat}","UInt64")]` | 202.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigFloat")]` | 365.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","BigInt")]` | 215.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigFloat}")]` | 917.00 ns (50%) | 0.00 ns | 752.00 bytes (1%) | 16 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{BigInt}")]` | 613.00 ns (50%) | 0.00 ns | 352.00 bytes (1%) | 14 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float32}")]` | 1.52 μs (50%) | 0.00 ns | 1.42 kb (1%) | 28 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Float64}")]` | 1.54 μs (50%) | 0.00 ns | 1.42 kb (1%) | 28 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{Int64}")]` | 613.00 ns (50%) | 0.00 ns | 352.00 bytes (1%) | 14 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Complex{UInt64}")]` | 600.00 ns (50%) | 0.00 ns | 352.00 bytes (1%) | 14 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float32")]` | 722.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Float64")]` | 721.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","Int64")]` | 223.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","Complex{BigInt}","UInt64")]` | 215.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigFloat")]` | 383.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Complex{Float32}","BigInt")]` | 707.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigFloat}")]` | 962.00 ns (50%) | 0.00 ns | 752.00 bytes (1%) | 16 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{BigInt}")]` | 1.52 μs (50%) | 0.00 ns | 1.42 kb (1%) | 28 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float32}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigFloat")]` | 385.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Complex{Float64}","BigInt")]` | 697.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigFloat}")]` | 942.00 ns (50%) | 0.00 ns | 752.00 bytes (1%) | 16 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{BigInt}")]` | 1.53 μs (50%) | 0.00 ns | 1.42 kb (1%) | 28 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Float64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigFloat")]` | 203.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","Complex{Int64}","BigInt")]` | 214.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{BigFloat}")]` | 598.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{BigInt}")]` | 617.00 ns (50%) | 0.00 ns | 352.00 bytes (1%) | 14 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{Int64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigFloat")]` | 202.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","BigInt")]` | 211.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{BigFloat}")]` | 589.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{BigInt}")]` | 610.00 ns (50%) | 0.00 ns | 352.00 bytes (1%) | 14 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Complex{UInt64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","BigFloat")]` | 213.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","Float32","BigInt")]` | 385.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Float32","Complex{BigFloat}")]` | 402.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Float32","Complex{BigInt}")]` | 718.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Float32","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float32","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","BigFloat")]` | 213.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","Float64","BigInt")]` | 387.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Float64","Complex{BigFloat}")]` | 398.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("mul","Float64","Complex{BigInt}")]` | 719.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("mul","Float64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Float64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","BigFloat")]` | 101.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("mul","Int64","BigInt")]` | 132.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","Int64","Complex{BigFloat}")]` | 203.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","Int64","Complex{BigInt}")]` | 221.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","Int64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","Int64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","BigFloat")]` | 99.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("mul","UInt64","BigInt")]` | 131.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigFloat}")]` | 201.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("mul","UInt64","Complex{BigInt}")]` | 215.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("mul","UInt64","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","BigFloat","BigFloat")]` | 101.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","BigFloat","BigInt")]` | 181.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigFloat}")]` | 197.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","BigFloat","Complex{BigInt}")]` | 373.00 ns (50%) | 0.00 ns | 344.00 bytes (1%) | 7 |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float32}")]` | 387.00 ns (50%) | 0.00 ns | 344.00 bytes (1%) | 7 |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Float64}")]` | 389.00 ns (50%) | 0.00 ns | 344.00 bytes (1%) | 7 |
| `["scalar","arithmetic",("sub","BigFloat","Complex{Int64}")]` | 318.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","BigFloat","Complex{UInt64}")]` | 318.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","BigFloat","Float32")]` | 190.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","BigFloat","Float64")]` | 191.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","BigFloat","Int64")]` | 120.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","BigFloat","UInt64")]` | 118.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","BigInt","BigFloat")]` | 182.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","BigInt","BigInt")]` | 134.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigFloat}")]` | 277.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","BigInt","Complex{BigInt}")]` | 220.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float32}")]` | 546.00 ns (50%) | 0.00 ns | 520.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("sub","BigInt","Complex{Float64}")]` | 547.00 ns (50%) | 0.00 ns | 520.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("sub","BigInt","Complex{Int64}")]` | 299.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("sub","BigInt","Complex{UInt64}")]` | 299.00 ns (50%) | 0.00 ns | 176.00 bytes (1%) | 7 |
| `["scalar","arithmetic",("sub","BigInt","Float32")]` | 340.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","BigInt","Float64")]` | 339.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","BigInt","Int64")]` | 131.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","BigInt","UInt64")]` | 130.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigFloat")]` | 102.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","BigInt")]` | 182.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigFloat}")]` | 212.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{BigInt}")]` | 288.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float32}")]` | 362.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Float64}")]` | 364.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{Int64}")]` | 225.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Complex{UInt64}")]` | 225.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float32")]` | 192.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Float64")]` | 193.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","Int64")]` | 122.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","Complex{BigFloat}","UInt64")]` | 120.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigFloat")]` | 276.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","BigInt")]` | 137.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigFloat}")]` | 290.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{BigInt}")]` | 229.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float32}")]` | 654.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Float64}")]` | 658.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{Int64}")]` | 221.00 ns (50%) | 0.00 ns | 152.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Complex{UInt64}")]` | 222.00 ns (50%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float32")]` | 441.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Float64")]` | 445.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","Int64")]` | 143.00 ns (50%) | 0.00 ns | 96.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{BigInt}","UInt64")]` | 132.00 ns (50%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigFloat")]` | 290.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{Float32}","BigInt")]` | 453.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigFloat}")]` | 358.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{BigInt}")]` | 655.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float32}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigFloat")]` | 288.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{Float64}","BigInt")]` | 450.00 ns (50%) | 0.00 ns | 416.00 bytes (1%) | 8 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigFloat}")]` | 355.00 ns (50%) | 0.00 ns | 272.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{BigInt}")]` | 639.00 ns (50%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Float64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigFloat")]` | 219.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{Int64}","BigInt")]` | 172.00 ns (50%) | 0.00 ns | 144.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigFloat}")]` | 233.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{BigInt}")]` | 173.00 ns (50%) | 0.00 ns | 144.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{Int64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigFloat")]` | 218.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","BigInt")]` | 163.00 ns (50%) | 0.00 ns | 112.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigFloat}")]` | 231.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{BigInt}")]` | 176.00 ns (50%) | 0.00 ns | 112.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Complex{UInt64}","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","BigFloat")]` | 191.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Float32","BigInt")]` | 339.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Float32","Complex{BigFloat}")]` | 286.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Float32","Complex{BigInt}")]` | 546.00 ns (50%) | 0.00 ns | 520.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("sub","Float32","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float32","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","BigFloat")]` | 191.00 ns (50%) | 0.00 ns | 136.00 bytes (1%) | 3 |
| `["scalar","arithmetic",("sub","Float64","BigInt")]` | 339.00 ns (50%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","arithmetic",("sub","Float64","Complex{BigFloat}")]` | 290.00 ns (50%) | 0.00 ns | 240.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Float64","Complex{BigInt}")]` | 536.00 ns (50%) | 0.00 ns | 520.00 bytes (1%) | 10 |
| `["scalar","arithmetic",("sub","Float64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Float64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","BigFloat")]` | 125.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","Int64","BigInt")]` | 84.00 ns (50%) | 0.00 ns | 56.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","Int64","Complex{BigFloat}")]` | 220.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","Int64","Complex{BigInt}")]` | 174.00 ns (50%) | 0.00 ns | 144.00 bytes (1%) | 5 |
| `["scalar","arithmetic",("sub","Int64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","Int64","UInt64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","BigFloat")]` | 123.00 ns (50%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","UInt64","BigInt")]` | 83.00 ns (50%) | 0.00 ns | 56.00 bytes (1%) | 2 |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigFloat}")]` | 217.00 ns (50%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","UInt64","Complex{BigInt}")]` | 166.00 ns (50%) | 0.00 ns | 112.00 bytes (1%) | 4 |
| `["scalar","arithmetic",("sub","UInt64","Complex{Float32}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","Complex{Float64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","Complex{Int64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","Complex{UInt64}")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","Float32")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","Float64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","Int64")]` | 2.00 ns (50%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","arithmetic",("sub","UInt64","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","BigFloat")]` | 142.00 ns (40%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","fastmath",("add","BigInt")]` | 133.00 ns (40%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","fastmath",("add","Complex{BigFloat}")]` | 646.00 ns (40%) | 0.00 ns | 624.00 bytes (1%) | 12 |
| `["scalar","fastmath",("add","Complex{BigInt}")]` | 602.00 ns (40%) | 0.00 ns | 352.00 bytes (1%) | 14 |
| `["scalar","fastmath",("add","Complex{Float32}")]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","Complex{Float64}")]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","Complex{Int64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","Complex{UInt64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","Float32")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","Float64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","Int64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("add","UInt64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","BigFloat")]` | 235.00 ns (40%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","fastmath",("div","BigInt")]` | 458.00 ns (40%) | 0.00 ns | 312.00 bytes (1%) | 6 |
| `["scalar","fastmath",("div","Complex{BigFloat}")]` | 1.31 μs (40%) | 0.00 ns | 1.15 kb (1%) | 23 |
| `["scalar","fastmath",("div","Complex{BigInt}")]` | 1.82 μs (40%) | 0.00 ns | 1.41 kb (1%) | 32 |
| `["scalar","fastmath",("div","Complex{Float32}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","Complex{Float64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","Complex{Int64}")]` | 10.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","Complex{UInt64}")]` | 9.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","Float32")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","Float64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","Int64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("div","UInt64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","BigFloat")]` | 114.00 ns (40%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","fastmath",("mul","BigInt")]` | 133.00 ns (40%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","fastmath",("mul","Complex{BigFloat}")]` | 223.00 ns (40%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","fastmath",("mul","Complex{BigInt}")]` | 228.00 ns (40%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","fastmath",("mul","Complex{Float32}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","Complex{Float64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","Complex{Int64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","Complex{UInt64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","Float32")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","Float64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","Int64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("mul","UInt64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","BigFloat")]` | 101.00 ns (40%) | 0.00 ns | 104.00 bytes (1%) | 2 |
| `["scalar","fastmath",("sub","BigInt")]` | 133.00 ns (40%) | 0.00 ns | 64.00 bytes (1%) | 3 |
| `["scalar","fastmath",("sub","Complex{BigFloat}")]` | 211.00 ns (40%) | 0.00 ns | 208.00 bytes (1%) | 4 |
| `["scalar","fastmath",("sub","Complex{BigInt}")]` | 221.00 ns (40%) | 0.00 ns | 120.00 bytes (1%) | 5 |
| `["scalar","fastmath",("sub","Complex{Float32}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","Complex{Float64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","Complex{Int64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","Complex{UInt64}")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","Float32")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","Float64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","Int64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","fastmath",("sub","UInt64")]` | 2.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","iteration","in"]` | 7.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","iteration","indexed"]` | 7.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","BigFloat")]` | 15.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","BigInt")]` | 4.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Complex{BigFloat}")]` | 28.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Complex{BigInt}")]` | 10.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isequal","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("iseven","BigInt")]` | 184.00 ns (25%) | 0.00 ns | 112.00 bytes (1%) | 4 |
| `["scalar","predicate",("iseven","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("iseven","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","BigFloat")]` | 6.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","BigInt")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Complex{BigFloat}")]` | 11.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Complex{BigInt}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isfinite","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","BigFloat")]` | 3.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","BigInt")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Complex{BigFloat}")]` | 6.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Complex{BigInt}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Complex{Float32}")]` | 4.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Complex{Float64}")]` | 4.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinf","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","BigFloat")]` | 6.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","BigInt")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Complex{BigFloat}")]` | 16.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Complex{BigInt}")]` | 5.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isinteger","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isless","BigFloat")]` | 15.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isless","BigInt")]` | 4.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isless","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isless","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isless","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isless","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","BigFloat")]` | 3.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","BigInt")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Complex{BigFloat}")]` | 6.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Complex{BigInt}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Complex{Float32}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Complex{Float64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Complex{Int64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Complex{UInt64}")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Float32")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Float64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isnan","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isodd","BigInt")]` | 184.00 ns (25%) | 0.00 ns | 112.00 bytes (1%) | 4 |
| `["scalar","predicate",("isodd","Int64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["scalar","predicate",("isodd","UInt64")]` | 2.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["shootout","binary_trees"]` | 24.82 ms (15%) | 0.00 ns | 11.92 mb (1%) | 515432 |
| `["shootout","fannkuch"]` | 139.83 μs (15%) | 0.00 ns | 336.00 bytes (1%) | 3 |
| `["shootout","fasta"]` | 12.72 μs (15%) | 0.00 ns | 15.63 kb (1%) | 811 |
| `["shootout","k_nucleotide"]` | 63.68 ms (15%) | 7.34 ms | 28.59 mb (1%) | 508513 |
| `["shootout","mandelbrot"]` | 3.51 ms (15%) | 0.00 ns | 8.48 kb (1%) | 47 |
| `["shootout","meteor_contest"]` | 2.35 s (15%) | 395.36 ms | 1.03 gb (1%) | 52287077 |
| `["shootout","nbody"]` | 159.89 μs (15%) | 0.00 ns | 448.00 bytes (1%) | 6 |
| `["shootout","nbody_vec"]` | 2.92 ms (15%) | 0.00 ns | 8.01 mb (1%) | 105035 |
| `["shootout","pidigits"]` | 25.77 ms (15%) | 11.51 ms | 63.47 mb (1%) | 101225 |
| `["shootout","regex_dna"]` | 5.79 ms (15%) | 0.00 ns | 1.83 mb (1%) | 8723 |
| `["shootout","revcomp"]` | 11.28 ms (15%) | 0.00 ns | 1.91 mb (1%) | 11850 |
| `["shootout","spectralnorm"]` | 1.44 ms (15%) | 0.00 ns | 8.89 kb (1%) | 404 |
| `["simd",("axpy!","Float32",4095)]` | 233.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Float32",4096)]` | 220.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Float64",4095)]` | 448.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Float64",4096)]` | 441.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Int32",4095)]` | 287.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Int32",4096)]` | 274.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Int64",4095)]` | 1.62 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("axpy!","Int64",4096)]` | 1.61 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Float32",4095)]` | 13.21 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Float32",4096)]` | 13.21 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Float64",4095)]` | 13.50 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Float64",4096)]` | 13.49 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Int32",4095)]` | 144.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Int32",4096)]` | 139.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Int64",4095)]` | 313.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("conditional_loop!","Int64",4096)]` | 324.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Float32",4095)]` | 235.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Float32",4096)]` | 227.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Float64",4095)]` | 453.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Float64",4096)]` | 450.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Int32",4095)]` | 279.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Int32",4096)]` | 272.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Int64",4095)]` | 1.98 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("inner","Int64",4096)]` | 1.98 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("local_arrays","Float32",4095)]` | 613.24 μs (20%) | 0.00 ns | 373.64 kb (1%) | 19494 |
| `["simd",("local_arrays","Float32",4096)]` | 613.56 μs (20%) | 0.00 ns | 373.72 kb (1%) | 19499 |
| `["simd",("local_arrays","Float64",4095)]` | 562.95 μs (20%) | 0.00 ns | 421.03 kb (1%) | 19491 |
| `["simd",("local_arrays","Float64",4096)]` | 563.05 μs (20%) | 0.00 ns | 421.11 kb (1%) | 19496 |
| `["simd",("local_arrays","Int32",4095)]` | 536.18 μs (20%) | 0.00 ns | 373.64 kb (1%) | 19494 |
| `["simd",("local_arrays","Int32",4096)]` | 536.86 μs (20%) | 0.00 ns | 373.72 kb (1%) | 19499 |
| `["simd",("local_arrays","Int64",4095)]` | 567.79 μs (20%) | 0.00 ns | 421.50 kb (1%) | 19497 |
| `["simd",("local_arrays","Int64",4096)]` | 568.64 μs (20%) | 0.00 ns | 421.58 kb (1%) | 19502 |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 217.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 201.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 210.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 201.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 441.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 433.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 441.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Float64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 433.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 294.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 280.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 294.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int32","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 280.00 ns (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4095)]` | 2.00 μs (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.ImmutableFields{V<:AbstractArray{T,1}}",4096)]` | 2.00 μs (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4095)]` | 2.00 μs (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("loop_fields!","Int64","BaseBenchmarks.SIMDBenchmarks.MutableFields{V<:AbstractArray{T,1}}",4096)]` | 2.00 μs (20%) | 0.00 ns | 32.00 bytes (1%) | 1 |
| `["simd",("manual_example!","Float32",4095)]` | 333.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Float32",4096)]` | 320.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Float64",4095)]` | 642.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Float64",4096)]` | 641.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Int32",4095)]` | 329.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Int32",4096)]` | 327.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Int64",4095)]` | 1.13 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("manual_example!","Int64",4096)]` | 1.14 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Float32",4095)]` | 78.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Float32",4096)]` | 78.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Float64",4095)]` | 142.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Float64",4096)]` | 142.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Int32",4095)]` | 53.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Int32",4096)]` | 54.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Int64",4095)]` | 90.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("sum_reduce","Int64",4096)]` | 90.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Float32",4095)]` | 881.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Float32",4096)]` | 870.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Float64",4095)]` | 1.75 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Float64",4096)]` | 1.75 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Int32",4095)]` | 88.04 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Int32",4096)]` | 88.07 μs (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Int64",4095)]` | 655.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["simd",("two_reductions","Int64",4096)]` | 663.00 ns (20%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sort","insertionsort",("sort forwards","ascending")]` | 69.32 μs (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","insertionsort",("sort forwards","descending")]` | 579.84 ms (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","insertionsort",("sort forwards","ones")]` | 171.28 μs (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","insertionsort",("sort forwards","random")]` | 289.02 ms (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","insertionsort",("sort reverse","ascending")]` | 579.98 ms (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","insertionsort",("sort reverse","descending")]` | 72.39 μs (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","insertionsort",("sort reverse","ones")]` | 194.15 μs (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","insertionsort",("sort reverse","random")]` | 286.35 ms (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","insertionsort",("sort! forwards","ascending")]` | 31.17 μs (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! forwards","descending")]` | 579.76 ms (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! forwards","ones")]` | 132.86 μs (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! forwards","random")]` | 288.98 ms (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! reverse","ascending")]` | 579.90 ms (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! reverse","descending")]` | 32.79 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! reverse","ones")]` | 154.77 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sort! reverse","random")]` | 286.26 ms (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","insertionsort",("sortperm forwards","ascending")]` | 102.72 μs (15%) | 0.00 ns | 390.84 kb (1%) | 5 |
| `["sort","insertionsort",("sortperm forwards","descending")]` | 924.52 ms (15%) | 0.00 ns | 390.84 kb (1%) | 5 |
| `["sort","insertionsort",("sortperm forwards","ones")]` | 270.54 μs (15%) | 0.00 ns | 390.88 kb (1%) | 7 |
| `["sort","insertionsort",("sortperm forwards","random")]` | 713.75 ms (15%) | 0.00 ns | 390.88 kb (1%) | 7 |
| `["sort","insertionsort",("sortperm reverse","ascending")]` | 924.88 ms (15%) | 0.00 ns | 390.86 kb (1%) | 5 |
| `["sort","insertionsort",("sortperm reverse","descending")]` | 103.57 μs (15%) | 0.00 ns | 390.86 kb (1%) | 5 |
| `["sort","insertionsort",("sortperm reverse","ones")]` | 291.13 μs (15%) | 0.00 ns | 390.89 kb (1%) | 7 |
| `["sort","insertionsort",("sortperm reverse","random")]` | 706.89 ms (15%) | 0.00 ns | 390.89 kb (1%) | 7 |
| `["sort","insertionsort",("sortperm! forwards","ascending")]` | 85.53 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 2 |
| `["sort","insertionsort",("sortperm! forwards","descending")]` | 924.70 ms (15%) | 0.00 ns | 112.00 bytes (1%) | 2 |
| `["sort","insertionsort",("sortperm! forwards","ones")]` | 254.06 μs (15%) | 0.00 ns | 144.00 bytes (1%) | 4 |
| `["sort","insertionsort",("sortperm! forwards","random")]` | 713.58 ms (15%) | 0.00 ns | 144.00 bytes (1%) | 4 |
| `["sort","insertionsort",("sortperm! reverse","ascending")]` | 924.77 ms (15%) | 0.00 ns | 128.00 bytes (1%) | 2 |
| `["sort","insertionsort",("sortperm! reverse","descending")]` | 86.42 μs (15%) | 0.00 ns | 128.00 bytes (1%) | 2 |
| `["sort","insertionsort",("sortperm! reverse","ones")]` | 273.92 μs (15%) | 0.00 ns | 160.00 bytes (1%) | 4 |
| `["sort","insertionsort",("sortperm! reverse","random")]` | 706.69 ms (15%) | 0.00 ns | 160.00 bytes (1%) | 4 |
| `["sort","issorted",("forwards","ascending")]` | 21.91 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sort","issorted",("forwards","descending")]` | 22.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sort","issorted",("forwards","ones")]` | 86.47 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sort","issorted",("forwards","random")]` | 24.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sort","issorted",("reverse","ascending")]` | 390.00 ns (30%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","issorted",("reverse","descending")]` | 27.36 μs (30%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","issorted",("reverse","ones")]` | 85.96 μs (30%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","issorted",("reverse","random")]` | 388.00 ns (30%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","mergesort",("sort forwards","ascending")]` | 676.32 μs (15%) | 0.00 ns | 586.56 kb (1%) | 12 |
| `["sort","mergesort",("sort forwards","descending")]` | 882.72 μs (15%) | 0.00 ns | 586.56 kb (1%) | 12 |
| `["sort","mergesort",("sort forwards","ones")]` | 802.06 μs (15%) | 0.00 ns | 586.64 kb (1%) | 13 |
| `["sort","mergesort",("sort forwards","random")]` | 3.69 ms (15%) | 0.00 ns | 586.64 kb (1%) | 13 |
| `["sort","mergesort",("sort reverse","ascending")]` | 885.06 μs (15%) | 0.00 ns | 586.67 kb (1%) | 15 |
| `["sort","mergesort",("sort reverse","descending")]` | 678.08 μs (15%) | 0.00 ns | 586.67 kb (1%) | 15 |
| `["sort","mergesort",("sort reverse","ones")]` | 836.74 μs (15%) | 0.00 ns | 586.75 kb (1%) | 16 |
| `["sort","mergesort",("sort reverse","random")]` | 3.71 ms (15%) | 0.00 ns | 586.75 kb (1%) | 16 |
| `["sort","mergesort",("sort! forwards","ascending")]` | 638.21 μs (15%) | 0.00 ns | 195.55 kb (1%) | 3 |
| `["sort","mergesort",("sort! forwards","descending")]` | 843.77 μs (15%) | 0.00 ns | 195.55 kb (1%) | 3 |
| `["sort","mergesort",("sort! forwards","ones")]` | 764.40 μs (15%) | 0.00 ns | 195.63 kb (1%) | 4 |
| `["sort","mergesort",("sort! forwards","random")]` | 3.65 ms (15%) | 0.00 ns | 195.63 kb (1%) | 4 |
| `["sort","mergesort",("sort! reverse","ascending")]` | 845.69 μs (15%) | 0.00 ns | 195.56 kb (1%) | 3 |
| `["sort","mergesort",("sort! reverse","descending")]` | 639.54 μs (15%) | 0.00 ns | 195.56 kb (1%) | 3 |
| `["sort","mergesort",("sort! reverse","ones")]` | 797.49 μs (15%) | 0.00 ns | 195.64 kb (1%) | 4 |
| `["sort","mergesort",("sort! reverse","random")]` | 3.67 ms (15%) | 0.00 ns | 195.64 kb (1%) | 4 |
| `["sort","mergesort",("sortperm forwards","ascending")]` | 1.01 ms (15%) | 0.00 ns | 586.30 kb (1%) | 7 |
| `["sort","mergesort",("sortperm forwards","descending")]` | 1.25 ms (15%) | 0.00 ns | 586.30 kb (1%) | 7 |
| `["sort","mergesort",("sortperm forwards","ones")]` | 1.20 ms (15%) | 0.00 ns | 586.41 kb (1%) | 10 |
| `["sort","mergesort",("sortperm forwards","random")]` | 5.41 ms (15%) | 0.00 ns | 586.41 kb (1%) | 10 |
| `["sort","mergesort",("sortperm reverse","ascending")]` | 1.25 ms (15%) | 0.00 ns | 586.31 kb (1%) | 7 |
| `["sort","mergesort",("sortperm reverse","descending")]` | 1.02 ms (15%) | 0.00 ns | 586.31 kb (1%) | 7 |
| `["sort","mergesort",("sortperm reverse","ones")]` | 1.21 ms (15%) | 0.00 ns | 586.42 kb (1%) | 10 |
| `["sort","mergesort",("sortperm reverse","random")]` | 5.44 ms (15%) | 0.00 ns | 586.42 kb (1%) | 10 |
| `["sort","mergesort",("sortperm! forwards","ascending")]` | 996.85 μs (15%) | 0.00 ns | 195.56 kb (1%) | 4 |
| `["sort","mergesort",("sortperm! forwards","descending")]` | 1.23 ms (15%) | 0.00 ns | 195.56 kb (1%) | 4 |
| `["sort","mergesort",("sortperm! forwards","ones")]` | 1.19 ms (15%) | 0.00 ns | 195.67 kb (1%) | 7 |
| `["sort","mergesort",("sortperm! forwards","random")]` | 5.40 ms (15%) | 0.00 ns | 195.67 kb (1%) | 7 |
| `["sort","mergesort",("sortperm! reverse","ascending")]` | 1.23 ms (15%) | 0.00 ns | 195.58 kb (1%) | 4 |
| `["sort","mergesort",("sortperm! reverse","descending")]` | 997.72 μs (15%) | 0.00 ns | 195.58 kb (1%) | 4 |
| `["sort","mergesort",("sortperm! reverse","ones")]` | 1.19 ms (15%) | 0.00 ns | 195.69 kb (1%) | 7 |
| `["sort","mergesort",("sortperm! reverse","random")]` | 5.41 ms (15%) | 0.00 ns | 195.69 kb (1%) | 7 |
| `["sort","quicksort",("sort forwards","ascending")]` | 312.00 μs (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","quicksort",("sort forwards","descending")]` | 329.91 μs (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","quicksort",("sort forwards","ones")]` | 592.69 μs (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","quicksort",("sort forwards","random")]` | 2.30 ms (15%) | 0.00 ns | 391.11 kb (1%) | 10 |
| `["sort","quicksort",("sort reverse","ascending")]` | 347.04 μs (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","quicksort",("sort reverse","descending")]` | 328.29 μs (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","quicksort",("sort reverse","ones")]` | 614.73 μs (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","quicksort",("sort reverse","random")]` | 2.32 ms (15%) | 0.00 ns | 391.22 kb (1%) | 13 |
| `["sort","quicksort",("sort! forwards","ascending")]` | 273.60 μs (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! forwards","descending")]` | 291.05 μs (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! forwards","ones")]` | 553.03 μs (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! forwards","random")]` | 2.26 ms (15%) | 0.00 ns | 96.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! reverse","ascending")]` | 306.45 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! reverse","descending")]` | 289.10 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! reverse","ones")]` | 575.42 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","quicksort",("sort! reverse","random")]` | 2.28 ms (15%) | 0.00 ns | 112.00 bytes (1%) | 1 |
| `["sort","quicksort",("sortperm forwards","ascending")]` | 457.95 μs (15%) | 0.00 ns | 390.84 kb (1%) | 5 |
| `["sort","quicksort",("sortperm forwards","descending")]` | 485.26 μs (15%) | 0.00 ns | 390.84 kb (1%) | 5 |
| `["sort","quicksort",("sortperm forwards","ones")]` | 752.48 μs (15%) | 0.00 ns | 390.88 kb (1%) | 7 |
| `["sort","quicksort",("sortperm forwards","random")]` | 3.58 ms (15%) | 0.00 ns | 390.88 kb (1%) | 7 |
| `["sort","quicksort",("sortperm reverse","ascending")]` | 484.03 μs (15%) | 0.00 ns | 390.86 kb (1%) | 5 |
| `["sort","quicksort",("sortperm reverse","descending")]` | 455.96 μs (15%) | 0.00 ns | 390.86 kb (1%) | 5 |
| `["sort","quicksort",("sortperm reverse","ones")]` | 771.63 μs (15%) | 0.00 ns | 390.89 kb (1%) | 7 |
| `["sort","quicksort",("sortperm reverse","random")]` | 3.60 ms (15%) | 0.00 ns | 390.89 kb (1%) | 7 |
| `["sort","quicksort",("sortperm! forwards","ascending")]` | 440.37 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 2 |
| `["sort","quicksort",("sortperm! forwards","descending")]` | 468.31 μs (15%) | 0.00 ns | 112.00 bytes (1%) | 2 |
| `["sort","quicksort",("sortperm! forwards","ones")]` | 734.64 μs (15%) | 0.00 ns | 144.00 bytes (1%) | 4 |
| `["sort","quicksort",("sortperm! forwards","random")]` | 3.56 ms (15%) | 0.00 ns | 144.00 bytes (1%) | 4 |
| `["sort","quicksort",("sortperm! reverse","ascending")]` | 466.30 μs (15%) | 0.00 ns | 128.00 bytes (1%) | 2 |
| `["sort","quicksort",("sortperm! reverse","descending")]` | 439.25 μs (15%) | 0.00 ns | 128.00 bytes (1%) | 2 |
| `["sort","quicksort",("sortperm! reverse","ones")]` | 754.56 μs (15%) | 0.00 ns | 160.00 bytes (1%) | 4 |
| `["sort","quicksort",("sortperm! reverse","random")]` | 3.58 ms (15%) | 0.00 ns | 160.00 bytes (1%) | 4 |
| `["sparse","index",("spmat","array",10)]` | 27.24 μs (25%) | 0.00 ns | 2.91 kb (1%) | 31 |
| `["sparse","index",("spmat","array",100)]` | 432.31 μs (25%) | 0.00 ns | 37.67 kb (1%) | 313 |
| `["sparse","index",("spmat","array",1000)]` | 4.96 ms (25%) | 0.00 ns | 721.39 kb (1%) | 3015 |
| `["sparse","index",("spmat","col","array",10)]` | 8.13 μs (15%) | 0.00 ns | 1.52 kb (1%) | 18 |
| `["sparse","index",("spmat","col","array",100)]` | 9.13 μs (15%) | 0.00 ns | 3.91 kb (1%) | 18 |
| `["sparse","index",("spmat","col","array",1000)]` | 45.66 μs (15%) | 0.00 ns | 26.27 kb (1%) | 18 |
| `["sparse","index",("spmat","col","logical",10)]` | 319.00 ns (15%) | 0.00 ns | 752.00 bytes (1%) | 8 |
| `["sparse","index",("spmat","col","logical",100)]` | 818.00 ns (15%) | 0.00 ns | 1.86 kb (1%) | 8 |
| `["sparse","index",("spmat","col","logical",1000)]` | 6.47 μs (15%) | 0.00 ns | 12.92 kb (1%) | 8 |
| `["sparse","index",("spmat","col","range",10)]` | 160.00 ns (15%) | 0.00 ns | 480.00 bytes (1%) | 5 |
| `["sparse","index",("spmat","col","range",100)]` | 159.00 ns (15%) | 0.00 ns | 608.00 bytes (1%) | 5 |
| `["sparse","index",("spmat","col","range",1000)]` | 250.00 ns (15%) | 0.00 ns | 1.78 kb (1%) | 5 |
| `["sparse","index",("spmat","integer",10)]` | 12.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","index",("spmat","integer",100)]` | 14.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","index",("spmat","integer",1000)]` | 17.00 ns (25%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","index",("spmat","logical",10)]` | 374.00 ns (25%) | 0.00 ns | 816.00 bytes (1%) | 7 |
| `["sparse","index",("spmat","logical",100)]` | 8.50 μs (25%) | 0.00 ns | 7.02 kb (1%) | 7 |
| `["sparse","index",("spmat","logical",1000)]` | 147.42 μs (25%) | 0.00 ns | 142.45 kb (1%) | 9 |
| `["sparse","index",("spmat","range",10)]` | 223.00 ns (25%) | 0.00 ns | 896.00 bytes (1%) | 4 |
| `["sparse","index",("spmat","range",100)]` | 2.42 μs (25%) | 0.00 ns | 16.67 kb (1%) | 4 |
| `["sparse","index",("spmat","range",1000)]` | 52.40 μs (25%) | 0.00 ns | 501.95 kb (1%) | 6 |
| `["sparse","index",("spmat","row","array",10)]` | 182.00 ns (15%) | 0.00 ns | 288.00 bytes (1%) | 5 |
| `["sparse","index",("spmat","row","array",100)]` | 1.22 μs (15%) | 0.00 ns | 736.00 bytes (1%) | 9 |
| `["sparse","index",("spmat","row","array",1000)]` | 19.56 μs (15%) | 0.00 ns | 1.38 kb (1%) | 11 |
| `["sparse","index",("spmat","row","logical",10)]` | 193.00 ns (15%) | 0.00 ns | 416.00 bytes (1%) | 6 |
| `["sparse","index",("spmat","row","logical",100)]` | 1.01 μs (15%) | 0.00 ns | 832.00 bytes (1%) | 6 |
| `["sparse","index",("spmat","row","logical",1000)]` | 11.35 μs (15%) | 0.00 ns | 4.78 kb (1%) | 10 |
| `["sparse","index",("spmat","row","range",10)]` | 167.00 ns (15%) | 0.00 ns | 288.00 bytes (1%) | 5 |
| `["sparse","index",("spmat","row","range",100)]` | 920.00 ns (15%) | 0.00 ns | 448.00 bytes (1%) | 7 |
| `["sparse","index",("spmat","row","range",1000)]` | 15.21 μs (15%) | 0.00 ns | 1.38 kb (1%) | 11 |
| `["sparse","index",("spmat","splogical",10)]` | 155.00 ns (25%) | 0.00 ns | 192.00 bytes (1%) | 3 |
| `["sparse","index",("spmat","splogical",100)]` | 897.00 ns (25%) | 0.00 ns | 192.00 bytes (1%) | 3 |
| `["sparse","index",("spmat","splogical",1000)]` | 7.66 ms (25%) | 0.00 ns | 352.00 bytes (1%) | 3 |
| `["sparse","index",("spvec","array",1000)]` | 46.61 μs (15%) | 0.00 ns | 27.11 kb (1%) | 20 |
| `["sparse","index",("spvec","array",10000)]` | 641.82 μs (15%) | 0.00 ns | 239.23 kb (1%) | 23 |
| `["sparse","index",("spvec","array",100000)]` | 7.94 ms (15%) | 0.00 ns | 2.30 mb (1%) | 23 |
| `["sparse","index",("spvec","integer",1000)]` | 42.00 ns (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","index",("spvec","integer",10000)]` | 45.00 ns (15%) | 0.00 ns | 16.00 bytes (1%) | 1 |
| `["sparse","index",("spvec","integer",100000)]` | 48.00 ns (15%) | 0.00 ns | 16.00 bytes (1%) | 1 |
| `["sparse","index",("spvec","logical",1000)]` | 5.71 μs (15%) | 0.00 ns | 4.94 kb (1%) | 9 |
| `["sparse","index",("spvec","logical",10000)]` | 92.69 μs (15%) | 0.00 ns | 39.98 kb (1%) | 10 |
| `["sparse","index",("spvec","logical",100000)]` | 987.08 μs (15%) | 0.00 ns | 394.77 kb (1%) | 10 |
| `["sparse","index",("spvec","range",1000)]` | 208.00 ns (15%) | 0.00 ns | 832.00 bytes (1%) | 3 |
| `["sparse","index",("spvec","range",10000)]` | 393.00 ns (15%) | 0.00 ns | 2.00 kb (1%) | 3 |
| `["sparse","index",("spvec","range",100000)]` | 1.34 μs (15%) | 0.00 ns | 5.16 kb (1%) | 3 |
| `["sparse","transpose",("ctranspose!",(20000,10000))]` | 31.16 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("ctranspose!",(20000,20000))]` | 62.51 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("ctranspose!",(600,400))]` | 12.32 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("ctranspose!",(600,600))]` | 19.49 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("ctranspose",(20000,10000))]` | 34.85 ms (15%) | 3.50 ms | 45.91 mb (1%) | 8 |
| `["sparse","transpose",("ctranspose",(20000,20000))]` | 72.53 ms (15%) | 8.07 ms | 91.69 mb (1%) | 8 |
| `["sparse","transpose",("ctranspose",(600,400))]` | 16.63 μs (15%) | 0.00 ns | 60.55 kb (1%) | 7 |
| `["sparse","transpose",("ctranspose",(600,600))]` | 25.56 μs (15%) | 0.00 ns | 88.30 kb (1%) | 7 |
| `["sparse","transpose",("transpose!",(20000,10000))]` | 29.78 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("transpose!",(20000,20000))]` | 59.93 ms (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("transpose!",(600,400))]` | 10.02 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("transpose!",(600,600))]` | 17.23 μs (15%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["sparse","transpose",("transpose",(20000,10000))]` | 33.43 ms (15%) | 3.47 ms | 30.66 mb (1%) | 8 |
| `["sparse","transpose",("transpose",(20000,20000))]` | 70.00 ms (15%) | 7.36 ms | 61.18 mb (1%) | 8 |
| `["sparse","transpose",("transpose",(600,400))]` | 13.32 μs (15%) | 0.00 ns | 42.11 kb (1%) | 7 |
| `["sparse","transpose",("transpose",(600,600))]` | 21.07 μs (15%) | 0.00 ns | 60.61 kb (1%) | 7 |
| `["string","join"]` | 137.13 ms (15%) | 59.48 ms | 129.02 mb (1%) | 20 |
| `["string","replace"]` | 187.72 μs (15%) | 0.00 ns | 12.11 kb (1%) | 6 |
| `["tuple","index",("sumelt","NTuple",3,Float32)]` | 3.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",3,Float64)]` | 3.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",30,Float32)]` | 15.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",30,Float64)]` | 13.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",60,Float32)]` | 32.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",60,Float64)]` | 32.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",8,Float32)]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","NTuple",8,Float64)]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",3,Float32)]` | 3.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",3,Float64)]` | 3.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",30,Float32)]` | 15.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",30,Float64)]` | 13.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",60,Float32)]` | 34.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",60,Float64)]` | 34.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",8,Float32)]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |
| `["tuple","index",("sumelt","TupleWrapper",8,Float64)]` | 4.00 ns (40%) | 0.00 ns | 0.00 bytes (1%) | 0 |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array","bool"]`
- `["array","cat"]`
- `["array","comprehension"]`
- `["array","growth"]`
- `["array","index"]`
- `["array","reverse"]`
- `["array","setindex!"]`
- `["array","subarray"]`
- `["io","read"]`
- `["io"]`
- `["linalg","arithmetic"]`
- `["linalg","blas"]`
- `["linalg","factorization"]`
- `["micro"]`
- `["parallel","remotecall"]`
- `["problem","fem"]`
- `["problem","go"]`
- `["problem","grigoriadis khachiyan"]`
- `["problem","imdb"]`
- `["problem","json"]`
- `["problem","laplacian"]`
- `["problem","monte carlo"]`
- `["problem"]`
- `["problem","seismic"]`
- `["scalar","arithmetic"]`
- `["scalar","fastmath"]`
- `["scalar","iteration"]`
- `["scalar","predicate"]`
- `["shootout"]`
- `["simd"]`
- `["sort","insertionsort"]`
- `["sort","issorted"]`
- `["sort","mergesort"]`
- `["sort","quicksort"]`
- `["sparse","index"]`
- `["sparse","transpose"]`
- `["string"]`
- `["tuple","index"]`

## Version Info

#### Primary Build

```
Julia Version 0.5.0-dev+4642
Commit 4f65737 (2016-06-10 02:00 UTC)
Platform Info:
  System: Linux (x86_64-linux-gnu)
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz
  WORD_SIZE: 64
           Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
Memory: 31.383651733398438 GB (28270.73828125 MB free)
Uptime: 1.18104e6 sec
Load Avg:  1.0029296875  1.00927734375  0.955078125
Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
       speed         user         nice          sys         idle          irq
#1  3501 MHz     373836 s          0 s     224631 s  117211525 s          4 s
#2  3501 MHz    1486791 s          0 s     126874 s  116420334 s          0 s
#3  3501 MHz     721199 s          0 s     140325 s  117177705 s          0 s
#4  3501 MHz     635228 s          0 s     123082 s  117287614 s          0 s

  BLAS: libopenblas (USE64BITINT DYNAMIC_ARCH NO_AFFINITY Haswell)
  LAPACK: libopenblas64_
  LIBM: libopenlibm
  LLVM: libLLVM-3.7.1 (ORCJIT, haswell)

```
