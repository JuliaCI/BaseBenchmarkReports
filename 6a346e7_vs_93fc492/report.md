# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@6a346e720f213f2ccaf0950f23959f04db391edb](https://github.com/JuliaLang/julia/commit/6a346e720f213f2ccaf0950f23959f04db391edb) vs [JuliaLang/julia@93fc492fd4a371439db0e1464346c73d1156e5f9](https://github.com/JuliaLang/julia/commit/93fc492fd4a371439db0e1464346c73d1156e5f9)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23642#issuecomment-348317734)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

