# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f78480d09d3ee80f08db76c1674492f6b992bde3](https://github.com/JuliaLang/julia/commit/f78480d09d3ee80f08db76c1674492f6b992bde3) vs [JuliaLang/julia@df63db683237fdb90fc1f93136400cfa34d6bd33](https://github.com/JuliaLang/julia/commit/df63db683237fdb90fc1f93136400cfa34d6bd33)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22202#issuecomment-313842830)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

