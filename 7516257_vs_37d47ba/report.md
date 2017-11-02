# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@7516257ee2cb992800da3e572838554b513bee19](https://github.com/JuliaLang/julia/commit/7516257ee2cb992800da3e572838554b513bee19) vs [JuliaLang/julia@37d47ba006b7f185e752bbdcd483a156151b1a15](https://github.com/JuliaLang/julia/commit/37d47ba006b7f185e752bbdcd483a156151b1a15)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/24406#issuecomment-341335770)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

