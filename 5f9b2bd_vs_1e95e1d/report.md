# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5f9b2bd059d26e5ccb228d87f66034bf2a29776e](https://github.com/JuliaLang/julia/commit/5f9b2bd059d26e5ccb228d87f66034bf2a29776e) vs [JuliaLang/julia@1e95e1d9b6fbdba1840f0bb91c4c7acf1683bc62](https://github.com/JuliaLang/julia/commit/1e95e1d9b6fbdba1840f0bb91c4c7acf1683bc62)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22732#issuecomment-314055916)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against comparison commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

