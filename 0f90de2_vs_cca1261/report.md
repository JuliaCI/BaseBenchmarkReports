# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@0f90de2dac30b09d269c9db141497a4242f3b555](https://github.com/JuliaLang/julia/commit/0f90de2dac30b09d269c9db141497a4242f3b555) vs [JuliaLang/julia@cca1261cfe2435b16a4e686956ec3b4a73793e00](https://github.com/JuliaLang/julia/commit/cca1261cfe2435b16a4e686956ec3b4a73793e00)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25890#issuecomment-368084067)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

