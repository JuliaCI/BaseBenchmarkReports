# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@f050fd2280a244d9d61a066c0db89063d1dd611d](https://github.com/JuliaLang/julia/commit/f050fd2280a244d9d61a066c0db89063d1dd611d) vs [JuliaLang/julia@1c5ed7082516c8a8c259907ceef908ba0c9d2107](https://github.com/JuliaLang/julia/commit/1c5ed7082516c8a8c259907ceef908ba0c9d2107)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25377#issuecomment-383357799)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

