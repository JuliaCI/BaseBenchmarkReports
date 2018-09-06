# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@39a61940074945a023ddfbce8a4ed19a24064eb1](https://github.com/JuliaLang/julia/commit/39a61940074945a023ddfbce8a4ed19a24064eb1) vs [JuliaLang/julia@88d536a1ea8903dfdfd78f86a5be75eedcfddf5a](https://github.com/JuliaLang/julia/commit/88d536a1ea8903dfdfd78f86a5be75eedcfddf5a)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/28857#issuecomment-419202118)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

