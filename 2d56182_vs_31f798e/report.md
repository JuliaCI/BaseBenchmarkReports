# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@2d56182650f6fe68e1db062d256c1bae8cad4436](https://github.com/JuliaLang/julia/commit/2d56182650f6fe68e1db062d256c1bae8cad4436) vs [JuliaLang/julia@31f798eb820007906783d30824e865c87ebecf09](https://github.com/JuliaLang/julia/commit/31f798eb820007906783d30824e865c87ebecf09)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/21892#issuecomment-302652245)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(132)) [132]
```

Check the logs folder in this directory for more detailed output.

