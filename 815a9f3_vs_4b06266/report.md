# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@815a9f3788ba9da5083704b6ec0ae3d708e80964](https://github.com/JuliaLang/julia/commit/815a9f3788ba9da5083704b6ec0ae3d708e80964) vs [JuliaLang/julia@4b0626626cbfd5afcf01da3ebda0c3c684141763](https://github.com/JuliaLang/julia/commit/4b0626626cbfd5afcf01da3ebda0c3c684141763)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24406#issuecomment-341273552)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

