# Benchmark Report

## Job Properties

*Commit(s):* [andyferris/julia@130f9e2eaa9847b964ecd3aa21adf9cf14d19241](https://github.com/andyferris/julia/commit/130f9e2eaa9847b964ecd3aa21adf9cf14d19241) vs [JuliaLang/julia@8563fc5a969b279e4f54c2d8bdb92a32f324a8fc](https://github.com/JuliaLang/julia/commit/8563fc5a969b279e4f54c2d8bdb92a32f324a8fc)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19670#issuecomment-270329573)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

