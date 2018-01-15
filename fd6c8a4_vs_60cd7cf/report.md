# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@fd6c8a40532ad80503d8939004564f00b1cf1e5b](https://github.com/JuliaLang/julia/commit/fd6c8a40532ad80503d8939004564f00b1cf1e5b) vs [JuliaLang/julia@60cd7cf42bd7124c30ea7310cb9fdff447e76ae9](https://github.com/JuliaLang/julia/commit/60cd7cf42bd7124c30ea7310cb9fdff447e76ae9)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25261#issuecomment-357559011)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

