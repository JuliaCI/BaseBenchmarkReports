# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@ed8525a56fe7430928c5d46fc0309cbb99fb538a](https://github.com/JuliaLang/julia/commit/ed8525a56fe7430928c5d46fc0309cbb99fb538a) vs [JuliaLang/julia@d44977ceb05e6b1196a563c5dc62dc72ee9a526d](https://github.com/JuliaLang/julia/commit/d44977ceb05e6b1196a563c5dc62dc72ee9a526d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19449#issuecomment-269786669)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

