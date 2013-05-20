Runs the thing named `curl` on your system and pipes the output to a node script that attempts to `JSON.parse()` the result and output it as pretty-printed JSON. If it can't, it just outputs whatever came out, unaltered.

Any params you pass are simply passed along wholesale to the `curl` command on your system.


