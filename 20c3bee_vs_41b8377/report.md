# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@20c3bee4f7489834413045802b52ad666baf7803](https://github.com/JuliaLang/julia/commit/20c3bee4f7489834413045802b52ad666baf7803) vs [JuliaLang/julia@41b83778b48e16de7cc099efa05c458aa92a9003](https://github.com/JuliaLang/julia/commit/41b83778b48e16de7cc099efa05c458aa92a9003)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21750#issuecomment-303263145)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

