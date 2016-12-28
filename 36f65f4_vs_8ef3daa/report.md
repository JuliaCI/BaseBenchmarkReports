# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@36f65f45694dbe2e90dbfc7ce74e6652a1b40b53](https://github.com/JuliaLang/julia/commit/36f65f45694dbe2e90dbfc7ce74e6652a1b40b53) vs [JuliaLang/julia@8ef3daa92e66c63d68ba8166e9562fdd25d059cc](https://github.com/JuliaLang/julia/commit/8ef3daa92e66c63d68ba8166e9562fdd25d059cc)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/19449#issuecomment-269426013)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

