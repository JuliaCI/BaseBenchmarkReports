# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@5fec1be921897987d3004a3ccb7d1f7e1d699f1d](https://github.com/JuliaLang/julia/commit/5fec1be921897987d3004a3ccb7d1f7e1d699f1d) vs [JuliaLang/julia@b49cb079b1d4abd36513cc1bb6a01eeb035d0547](https://github.com/JuliaLang/julia/commit/b49cb079b1d4abd36513cc1bb6a01eeb035d0547)

*Triggered By:* [link](https://github.com/JuliaLang/julia/pull/22420#issuecomment-309259973)

*Tag Predicate:* `ALL`

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -e su nanosoldier -- -c ./benchscript.sh`, ProcessExited(139)) [139]
```

Check the logs folder in this directory for more detailed output.

