# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@245208df4dcac86cf413dc2ed7aba5243fba1e44](https://github.com/JuliaLang/julia/commit/245208df4dcac86cf413dc2ed7aba5243fba1e44) vs [JuliaLang/julia@5d90ab6f1407ff934825cfa234f8db378ec1161e](https://github.com/JuliaLang/julia/commit/5d90ab6f1407ff934825cfa234f8db378ec1161e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18457#issuecomment-270931974)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

