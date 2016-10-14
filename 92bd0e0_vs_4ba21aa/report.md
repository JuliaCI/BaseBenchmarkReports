# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@92bd0e0f76ddec226bb29d86af4e47db1aa29896](https://github.com/JuliaLang/julia/commit/92bd0e0f76ddec226bb29d86af4e47db1aa29896) vs [JuliaLang/julia@4ba21aa57f57b9e42eeba5886d9dec772281e9f2](https://github.com/JuliaLang/julia/commit/4ba21aa57f57b9e42eeba5886d9dec772281e9f2)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18754#issuecomment-253839513)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

