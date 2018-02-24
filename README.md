# Some (mostly) bash only utilities

#### Gobbler
Functions to read a file inside a variable and dump it relying on a b64 enc/dec binary (busybox).

#### Logger 
Declare a `LOG_FILE` and run the bash only logger, a simple while loop.

#### CpuMon
Monitor a process cpu usage relying on `/proc`, bash and pgrep only (if no `cpumon_pid` is provided). 
- `cpumon_span` the time period over which the average is calculated (60 seconds)
- `cpumon_ival` the frequency for polling data (3 seconds)

#### LimitMon
Limit a process cpu usage in bash only, sending process signals.

- `pid` the process id to limit
- `limit` the amount to limit (doesn't really scale correctly so adjust with trial and error)
