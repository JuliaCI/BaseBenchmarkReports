# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@fdbe3ef4d836f1e11c2909dab9b223f99142d2d1](https://github.com/JuliaLang/julia/commit/fdbe3ef4d836f1e11c2909dab9b223f99142d2d1) vs [JuliaLang/julia@33aa319142b3bca8bc47032ea76df9e4618d232f](https://github.com/JuliaLang/julia/commit/33aa319142b3bca8bc47032ea76df9e4618d232f)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21340#issuecomment-293070665)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(139)) [139]
```

Check the logs folder in this directory for more detailed output.

