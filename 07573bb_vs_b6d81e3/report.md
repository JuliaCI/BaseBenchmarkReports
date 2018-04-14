# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@07573bbbb4d39366a21aef19312ee1c33a30f0b8](https://github.com/JuliaLang/julia/commit/07573bbbb4d39366a21aef19312ee1c33a30f0b8) vs [JuliaLang/julia@b6d81e36bb150dca75755bad3a49c038e1630ea4](https://github.com/JuliaLang/julia/commit/b6d81e36bb150dca75755bad3a49c038e1630ea4)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25377#issuecomment-381304772)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

