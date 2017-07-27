# Benchmark Report

## Job Properties

*Commit(s):* [pkofod/julia@5290a67a557b6e04e5d2e6fed2a073bdd4703138](https://github.com/pkofod/julia/commit/5290a67a557b6e04e5d2e6fed2a073bdd4703138) vs [JuliaLang/julia@85a2555e539542c048fea99cd326d3fd8fb6da68](https://github.com/JuliaLang/julia/commit/85a2555e539542c048fea99cd326d3fd8fb6da68)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22824#issuecomment-318483787)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

