# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@a09c54b6ecdab511602f7cdbcdd2c266d3db93ff](https://github.com/JuliaLang/julia/commit/a09c54b6ecdab511602f7cdbcdd2c266d3db93ff) vs [JuliaLang/julia@7e27a28d4e495495af160eb57500ee73fe3731fb](https://github.com/JuliaLang/julia/commit/7e27a28d4e495495af160eb57500ee73fe3731fb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20485)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

