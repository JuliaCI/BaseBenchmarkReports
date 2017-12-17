# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@308f35a7eab874d4609f09b3bb90e19c412f825b](https://github.com/JuliaLang/julia/commit/308f35a7eab874d4609f09b3bb90e19c412f825b) vs [JuliaLang/julia@a5c9e88088883b43fa7fb0445ddf1d05e4709b1f](https://github.com/JuliaLang/julia/commit/a5c9e88088883b43fa7fb0445ddf1d05e4709b1f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25029#issuecomment-352243701)

*Tag Predicate:* `"collection"`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

