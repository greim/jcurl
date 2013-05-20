# What is jcurl?

Runs the thing named `curl` on your system and pipes the output to a node script that attempts to `JSON.parse()` the result and output it as pretty-printed JSON. If it can't, it just outputs whatever came out, unaltered.

Any params you pass are simply passed along wholesale to the `curl` command on your system.

This isn't a replacement for curl, but rather just a tool that makes it easy to read JSON for testing and debugging purposes for people who are in the habit of typing curl commands.

# Installation

    npm install -g jcurl
