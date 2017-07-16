# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@523f654cbfcb667bbc0042e431d14263b04ce9f5](https://github.com/JuliaLang/julia/commit/523f654cbfcb667bbc0042e431d14263b04ce9f5) vs [JuliaLang/julia@3ff6eac505746f78b018b6e3f175efebec574e2d](https://github.com/JuliaLang/julia/commit/3ff6eac505746f78b018b6e3f175efebec574e2d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22828#issuecomment-315602367)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

