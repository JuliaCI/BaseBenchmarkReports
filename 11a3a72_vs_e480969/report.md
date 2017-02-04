# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@11a3a72c21fb6489dc34506b64d804b269db37cf](https://github.com/JuliaLang/julia/commit/11a3a72c21fb6489dc34506b64d804b269db37cf) vs [JuliaLang/julia@e4809693eaa331718527652968a35092146872bb](https://github.com/JuliaLang/julia/commit/e4809693eaa331718527652968a35092146872bb)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20448#issuecomment-277432282)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

