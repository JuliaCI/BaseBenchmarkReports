# Benchmark Report

## Job Properties

*Commit(s):* [andyferris/julia@f42c63af59171ea5ed8ddafe17de176dc62fae0c](https://github.com/andyferris/julia/commit/f42c63af59171ea5ed8ddafe17de176dc62fae0c) vs [JuliaLang/julia@6195c28cf24a058875db1eba5f9d9e3c2a8c8b4d](https://github.com/JuliaLang/julia/commit/6195c28cf24a058875db1eba5f9d9e3c2a8c8b4d)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21771#issuecomment-300461106)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

