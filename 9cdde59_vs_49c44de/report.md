# Benchmark Report

## Job Properties

*Commit(s):* [musm/julia@9cdde59456c354861d543d9ddce8fa03536ab72d](https://github.com/musm/julia/commit/9cdde59456c354861d543d9ddce8fa03536ab72d) vs [JuliaLang/julia@49c44dedfe0af10f0e8a7372c800ff666c4914c1](https://github.com/JuliaLang/julia/commit/49c44dedfe0af10f0e8a7372c800ff666c4914c1)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/23400#issuecomment-324170692)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(1)) [1]
```

Check the logs folder in this directory for more detailed output.

