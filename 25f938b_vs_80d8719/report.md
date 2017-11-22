# Benchmark Report

## Job Properties

*Commit(s):* [mbauman/julia@25f938b949f935b6bde354d0765e6a1151a02d03](https://github.com/mbauman/julia/commit/25f938b949f935b6bde354d0765e6a1151a02d03) vs [JuliaLang/julia@80d8719a55091af96e4d3ed69b8e58c1a4217b09](https://github.com/JuliaLang/julia/commit/80d8719a55091af96e4d3ed69b8e58c1a4217b09)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/15558#issuecomment-346457613)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

