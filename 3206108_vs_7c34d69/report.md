# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@32061084ed7b23692797368ab40418bf197d2c01](https://github.com/JuliaLang/julia/commit/32061084ed7b23692797368ab40418bf197d2c01) vs [JuliaLang/julia@7c34d69eecbe99bc167958b412360f09dac94fa4](https://github.com/JuliaLang/julia/commit/7c34d69eecbe99bc167958b412360f09dac94fa4)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18457#issuecomment-271344104)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

