# Benchmark Report

## Job Properties

*Commit(s):* [mbauman/julia@6faaf62cfe59e159b0d03da6c62518b80fd498d3](https://github.com/mbauman/julia/commit/6faaf62cfe59e159b0d03da6c62518b80fd498d3) vs [JuliaLang/julia@e64ad77dd6e24c0eb7303b7eaf57b7da2a85b495](https://github.com/JuliaLang/julia/commit/e64ad77dd6e24c0eb7303b7eaf57b7da2a85b495)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/15558#issuecomment-346991537)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

