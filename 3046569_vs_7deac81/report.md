# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@3046569c15552cfd7731690dd01e4d897fdac603](https://github.com/JuliaLang/julia/commit/3046569c15552cfd7731690dd01e4d897fdac603) vs [JuliaLang/julia@7deac8139ca2410382f0570f35e5b7aba66fe49e](https://github.com/JuliaLang/julia/commit/7deac8139ca2410382f0570f35e5b7aba66fe49e)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/25630#issuecomment-358792117)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

