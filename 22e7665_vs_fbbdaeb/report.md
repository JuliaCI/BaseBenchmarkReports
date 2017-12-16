# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@22e7665ea0d4bf3d3655eaf5b7d0ea1802ae9cdf](https://github.com/JuliaLang/julia/commit/22e7665ea0d4bf3d3655eaf5b7d0ea1802ae9cdf) vs [JuliaLang/julia@fbbdaeb0465c29c5cb06b7c0e778e74ef84ceb1d](https://github.com/JuliaLang/julia/commit/fbbdaeb0465c29c5cb06b7c0e778e74ef84ceb1d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25033#issuecomment-352211897)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

