# Benchmark Report

## Job Properties

*Commit(s):* [stevengj/julia@22d0a0f08b0acb657bfc8083414670272810a1e3](https://github.com/stevengj/julia/commit/22d0a0f08b0acb657bfc8083414670272810a1e3) vs [JuliaLang/julia@6b1b4f6100677520ced65c253d02b6f22ceea1e6](https://github.com/JuliaLang/julia/commit/6b1b4f6100677520ced65c253d02b6f22ceea1e6)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19946#issuecomment-271582027)

*Tag Predicate:* `"string"`

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

## Benchmark Group List

Here's a list of all the benchmark groups executed by this job:

- `["dates","string"]`
- `["io","read"]`
- `["io","serialization"]`
- `["problem","spellcheck"]`
- `["string"]`

## Version Info

#### Primary Build

```
?
```

#### Comparison Build

```
?
```
