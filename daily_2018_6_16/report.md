# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@d9b10f08fa0bd65cb49c02661e2784ffda9061f3](https://github.com/JuliaLang/julia/commit/d9b10f08fa0bd65cb49c02661e2784ffda9061f3)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/d9b10f08fa0bd65cb49c02661e2784ffda9061f3#commitcomment-29387326)

*Tag Predicate:* `ALL`

*Daily Job:* 2018-06-16 vs 2018-06-15

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
| `["array", "cat", "(\"catnd\", 5)"]` | 1.07 (15%)  | 1.02 (1%) :x: |
| `["collection", "deletion", "(\"Dict\", \"Any\", \"pop!\")"]` | 0.09 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "deletion", "(\"Set\", \"Any\", \"pop!\")"]` | 0.09 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "optimizations", "(\"Set\", \"abstract\", \"Nothing\")"]` | 1.30 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"BitSet\", \"Int\", \"last\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"Any\", \"pop!\", \"unspecified\")"]` | 0.11 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Dict\", \"String\", \"pop!\", \"unspecified\")"]` | 1.40 (25%) :x: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Set\", \"Any\", \"pop!\", \"unspecified\")"]` | 0.10 (25%) :white_check_mark: | 1.00 (1%)  |
| `["collection", "queries & updates", "(\"Vector\", \"String\", \"push!\")"]` | 1.27 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"intersect!\", \"BitSet\")"]` | 1.33 (25%) :x: | 1.00 (1%)  |
| `["collection", "set operations", "(\"BitSet\", \"Int\", \"setdiff!\", \"BitSet\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["dates", "arithmetic", "(\"Date\", \"Month\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["dates", "query", "(\"firstdayofmonth\", \"DateTime\")"]` | 1.29 (25%) :x: | 1.00 (1%)  |
| `["find", "findnext", "(\"ispos\", \"Array{Float32,1}\")"]` | 1.17 (15%) :x: | 1.00 (1%)  |
| `["linalg", "factorization", "(\"lufact\", \"Tridiagonal\", 1024)"]` | 1.12 (45%)  | 1.02 (1%) :x: |
| `["linalg", "factorization", "(\"lufact\", \"Tridiagonal\", 256)"]` | 1.12 (45%)  | 1.06 (1%) :x: |
| `["micro", "fib"]` | 1.15 (15%) :x: | 1.00 (1%)  |
| `["micro", "parseint"]` | 1.12 (15%)  | 1.01 (1%) :x: |
| `["misc", "afoldl", "Complex{Float64}"]` | 1.15 (15%)  | 1.02 (1%) :x: |
| `["misc", "afoldl", "Float64"]` | 1.12 (15%)  | 1.02 (1%) :x: |
| `["misc", "afoldl", "Int"]` | 1.13 (15%)  | 1.02 (1%) :x: |
| `["misc", "parse", "DateTime"]` | 1.09 (15%)  | 1.02 (1%) :x: |
| `["misc", "parse", "Float64"]` | 1.09 (15%)  | 1.02 (1%) :x: |
| `["misc", "parse", "Int"]` | 1.06 (15%)  | 1.02 (1%) :x: |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:1\")"]` | 0.73 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"Int64\", \"1:4294967297\")"]` | 0.65 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"RangeGenerator\", \"UInt64\", \"1:4294967297\")"]` | 0.72 (25%) :white_check_mark: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:18446744073709551615)\")"]` | 1.45 (25%) :x: | 1.00 (1%)  |
| `["random", "ranges", "(\"rand\", \"MersenneTwister\", \"BigInt\", \"RangeGenerator(1:4294967295)\")"]` | 1.31 (25%) :x: | 1.00 (1%)  |
| `["random", "types", "(\"randexp\", \"ImplicitRNG\", \"Float64\")"]` | 1.61 (25%) :x: | 1.00 (1%)  |
| `["scalar", "asin", "(\"0.5 <= abs(x) < 0.975\", \"positive argument\", \"Float64\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"19/16 <= abs(x) < 39/16\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan", "(\"7/16 <= abs(x) < 11/16\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x negative\", \"Float64\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y negative\", \"x positive\", \"Float64\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.12 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x negative\", \"Float64\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) high\", \"y positive\", \"x positive\", \"Float64\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x negative\", \"Float64\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y negative\", \"x positive\", \"Float64\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x negative\", \"Float64\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (large)\", \"y positive\", \"x positive\", \"Float64\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x negative\", \"Float64\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y negative\", \"x positive\", \"Float64\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x negative\", \"Float64\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) safe (small)\", \"y positive\", \"x positive\", \"Float64\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x negative\", \"Float64\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"abs(y/x) small\", \"y positive\", \"x positive\", \"Float64\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"x one\", \"Float32\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"x one\", \"Float64\")"]` | 1.08 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float32\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"x zero\", \"y negative\", \"Float64\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"x zero\", \"y positive\", \"Float64\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y finite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y finite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float32\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x negative\", \"Float64\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float32\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x finite\", \"x positive\", \"Float64\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float32\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x negative\", \"Float64\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y negative\", \"x infinite\", \"x positive\", \"Float64\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float32\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x negative\", \"Float64\")"]` | 1.08 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float32\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x finite\", \"x positive\", \"Float64\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float32\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x negative\", \"Float64\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float32\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y infinite\", \"y positive\", \"x infinite\", \"x positive\", \"Float64\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float32\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x negative\", \"Float64\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float32\")"]` | 1.08 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y zero\", \"y negative\", \"x positive\", \"Float64\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float32\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x negative\", \"Float64\")"]` | 1.10 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float32\")"]` | 1.11 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atan2", "(\"y zero\", \"y positive\", \"x positive\", \"Float64\")"]` | 1.09 (15%)  | 1.10 (1%) :x: |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"negative argument\", \"Float64\")"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["scalar", "atanh", "(\"0.5 <= abs(x) < 1\", \"positive argument\", \"Float32\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["scalar", "cbrt", "(\"large\", \"positive argument\", \"Float32\")"]` | 0.63 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cos", "(\"argument reduction (easy) abs(x) < 4π/4\", \"positive argument\", \"Float32\", \"cos_kernel\")"]` | 0.81 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "cosh", "(\"0.00024414062f0 <= abs(x) < 9f0\", \"negative argument\", \"Float32\")"]` | 0.80 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "expm1", "(\"arg reduction II\", \"negative argument\", \"Float32\")"]` | 0.82 (15%) :white_check_mark: | 1.00 (1%)  |
| `["scalar", "rem_pio2", "(\"argument reduction (hard) abs(x) < 4π/4\", \"negative argument\", \"Float64\")"]` | 1.26 (15%) :x: | 1.00 (1%)  |
| `["scalar", "sincos", "(\"argument reduction (easy) abs(x) < 2.0^20π/4\", \"positive argument\", \"Float64\")"]` | 1.25 (15%) :x: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"array\", 1000)"]` | 0.61 (30%) :white_check_mark: | 1.00 (1%)  |
| `["sparse", "index", "(\"spmat\", \"row\", \"logical\", 1000)"]` | 0.68 (30%) :white_check_mark: | 1.00 (1%)  |
| `["string", "findfirst", "Char"]` | 1.13 (15%)  | 1.10 (1%) :x: |
| `["tuple", "reduction", "(\"sum\", (16, 16))"]` | 1.22 (15%) :x: | 1.00 (1%)  |
| `["tuple", "reduction", "(\"sum\", (4, 4))"]` | 0.83 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, false)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_countnothing\", BigFloat, true)"]` | 1.16 (15%) :x: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, false)"]` | 0.26 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"perf_sum\", Complex{Float64}, true)"]` | 0.31 (15%) :white_check_mark: | 1.00 (1%)  |
| `["union", "array", "(\"skipmissing\", collect, Complex{Float64}, true)"]` | 0.61 (15%) :white_check_mark: | 1.00 (1%)  |

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["array", "accumulate"]`
- `["array", "any/all"]`
- `["array", "bool"]`
- `["array", "cat"]`
- `["array", "comprehension"]`
- `["array", "convert"]`
- `["array", "equality"]`
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
- `["collection", "deletion"]`
- `["collection", "initialization"]`
- `["collection", "iteration"]`
- `["collection", "optimizations"]`
- `["collection", "queries & updates"]`
- `["collection", "set operations"]`
- `["dates", "accessor"]`
- `["dates", "arithmetic"]`
- `["dates", "construction"]`
- `["dates", "conversion"]`
- `["dates", "parse"]`
- `["dates", "query"]`
- `["dates", "string"]`
- `["find", "findall"]`
- `["find", "findnext"]`
- `["find", "findprev"]`
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
- `["scalar", "acosh"]`
- `["scalar", "arithmetic"]`
- `["scalar", "asin"]`
- `["scalar", "asinh"]`
- `["scalar", "atan"]`
- `["scalar", "atan2"]`
- `["scalar", "atanh"]`
- `["scalar", "cbrt"]`
- `["scalar", "cos"]`
- `["scalar", "cosh"]`
- `["scalar", "exp2"]`
- `["scalar", "expm1"]`
- `["scalar", "fastmath"]`
- `["scalar", "floatexp"]`
- `["scalar", "intfuncs"]`
- `["scalar", "iteration"]`
- `["scalar", "mod2pi"]`
- `["scalar", "predicate"]`
- `["scalar", "rem_pio2"]`
- `["scalar", "sin"]`
- `["scalar", "sincos"]`
- `["scalar", "sinh"]`
- `["scalar", "tan"]`
- `["scalar", "tanh"]`
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
- `["string", "findfirst"]`
- `["string"]`
- `["string", "readuntil"]`
- `["tuple", "index"]`
- `["tuple", "linear algebra"]`
- `["tuple", "reduction"]`
- `["union", "array"]`

## Version Info

#### Primary Build

```
Julia Version 0.7.0-alpha.144
Commit d9b10f0 (2018-06-16 03:17 UTC)
Platform Info:
  OS: Linux (x86_64-linux-gnu)
      Ubuntu 14.04.4 LTS
  uname: Linux 3.13.0-85-generic #129-Ubuntu SMP Thu Mar 17 20:50:15 UTC 2016 x86_64 x86_64
  CPU: Intel(R) Xeon(R) CPU E3-1241 v3 @ 3.50GHz: 
              speed         user         nice          sys         idle          irq
       #1  3501 MHz   29422424 s        276 s    3159992 s  661558522 s          6 s
       #2  3501 MHz  127187714 s          0 s    1769223 s  567033587 s          3 s
       #3  3501 MHz   16709423 s       2373 s    1422529 s  677529327 s          9 s
       #4  3501 MHz   15731650 s          0 s    1668434 s  678406488 s          6 s
       
  Memory: 31.383651733398438 GB (5161.2890625 MB free)
  Uptime: 6.963623e6 sec
  Load Avg:  1.0029296875  1.0146484375  1.04541015625
  WORD_SIZE: 64
  LIBM: libopenlibm
  LLVM: libLLVM-6.0.0 (ORCJIT, haswell)

```
