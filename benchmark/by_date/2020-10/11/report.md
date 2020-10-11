# Benchmark Report

## Job Properties

*Commit(s):* [JuliaLang/julia@113afd93092645e3939737c5c1c487edb7a62094](https://github.com/JuliaLang/julia/commit/113afd93092645e3939737c5c1c487edb7a62094)

*Triggered By:* [link](https://github.com/JuliaLang/julia/commit/113afd93092645e3939737c5c1c487edb7a62094#commitcomment-43140531)

*Tag Predicate:* `ALL`

*Daily Job:* 2020-10-11

## Error

The build could not finish due to an error:

```
NanosoldierError: failed to run benchmarks against primary commit: failed process: Process(`sudo cset shield -c 1,2,3,4 -k on`, ProcessExited(2)) [2]

Stacktrace:
 [1] pipeline_error at ./process.jl:525 [inlined]
 [2] run(::Cmd; wait::Bool) at ./process.jl:440
 [3] run at ./process.jl:438 [inlined]
 [4] execute_benchmarks!(::Nanosoldier.BenchmarkJob, ::Symbol) at /home/nanosoldier/.julia/packages/Nanosoldier/I3umL/src/jobs/BenchmarkJob.jl:402
 [5] run(::Nanosoldier.BenchmarkJob) at /home/nanosoldier/.julia/packages/Nanosoldier/I3umL/src/jobs/BenchmarkJob.jl:195
 [6] (::Distributed.var"#106#108"{Distributed.CallMsg{:call_fetch}})() at /buildworker/worker/package_linux64/build/usr/share/julia/stdlib/v1.5/Distributed/src/process_messages.jl:294
 [7] run_work_thunk(::Distributed.var"#106#108"{Distributed.CallMsg{:call_fetch}}, ::Bool) at /buildworker/worker/package_linux64/build/usr/share/julia/stdlib/v1.5/Distributed/src/process_messages.jl:79
 [8] macro expansion at /buildworker/worker/package_linux64/build/usr/share/julia/stdlib/v1.5/Distributed/src/process_messages.jl:294 [inlined]
 [9] (::Distributed.var"#105#107"{Distributed.CallMsg{:call_fetch},Distributed.MsgHeader,Sockets.TCPSocket})() at ./task.jl:356
```

Check the logs folder in this directory for more detailed output.

