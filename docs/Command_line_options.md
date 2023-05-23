| Option | Description |
| --- | --- |
| --scope | Specify path to file, folder or compile_commands.json to scan |
| --checkers | Specify checkers to be used. All by default. |
| --profile | Either a profile name (such as "default", "all", "cwe", etc.) OR and absolute path to a profile file. |
| --compile-options | Specify compile options |
| --gen-annotations | Control for which functions annotations should be generated. Pattern: <none [u][s][t] all>(default: none)<li>none - generation of annotation is turned off;</li><li>all - all functions;</li><li>u - functions that do not have a definition in the TU;</li><li>t - functions that are the source of untrusted data;</li><li>s - functions from system libraries;</li>
 |
| --log | Specify log details. Possible values: off, fatal, error, warn, warning, info, debug, trace, all. By default: info. |
| --compiler | Path to compiler binary which should be used to compile project. By default: /usr/bin/gcc |
| --reporter | Specify format for report. Possible values: out, csv, json, csv-html. By default: out. |
| --results-path | Path where report will be stored. By default: coddy binary path. |
| --gen-callgraph | Name of entry point function, for which should be collected paths in call graph. |
| --min-problem-severity | Specify the minimal severity of problem to report. Possible values: <error|warning|notify> |
| --callgraph-depth | Sets the depth of the call graph path. |
| --assumptions-in-trace |  |
| --persistent-storage |  |
| --taint-options | Control which functions can be considered "untrusted". Pattern: <none [u][s][p] all> (default: none):<li>none - taint analysis is turned off;</li><li>u - functions that do not have a definition in the TU;</li><li>s - functions marked with a macro specified in --taint-macro;</li><li>p - public API functions (with a definition, unused from this TU, ext. linkage);</li><li>all - all functions.</li> |
| --taint-macro | set macro used as an annotation to tainted functions (default: EXTER_ATTACK) |
| --ignore-suppresses | Show suppressed warnings |
| -v, --version | Print version. |
| -h, --help | Print usage. |
| --rhs-servers | Specify rhs server addresses list. This option overrides rhs servers list defined in profile. |