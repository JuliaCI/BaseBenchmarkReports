# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@08fcc7502444035a7102d6f9ace2e33836a87e87](https://github.com/JuliaLang/julia/commit/08fcc7502444035a7102d6f9ace2e33836a87e87) vs [JuliaLang/julia@c3995583c0cc1634c5c191e35cfa6721dd3b9f56](https://github.com/JuliaLang/julia/commit/c3995583c0cc1634c5c191e35cfa6721dd3b9f56)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/20952#issuecomment-286806429)

*Tag Predicate:* `"dates"`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

