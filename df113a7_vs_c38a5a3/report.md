# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@df113a7299dbf121a5ceda88e43ea331915a26ef](https://github.com/JuliaLang/julia/commit/df113a7299dbf121a5ceda88e43ea331915a26ef) vs [JuliaLang/julia@c38a5a3044ffd62c585225a201422f95fd18f6dc](https://github.com/JuliaLang/julia/commit/c38a5a3044ffd62c585225a201422f95fd18f6dc)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/18457#issuecomment-269918145)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: ErrorException("failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]")
```

Check the logs folder in this directory for more detailed output.

