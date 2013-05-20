# jcurl

Runs the thing named `curl` on your system and pipes the output to a node script that attempts to `JSON.parse()` the result and output it as pretty-printed JSON. If it can't, it just outputs whatever came out, unaltered.

Any params you pass are simply passed along wholesale to the `curl` command on your system, so that in general you can just type "jcurl" in place of wherever you type "curl".

This isn't a replacement for curl, but rather just a tool that makes it easy to read JSON for testing and debugging purposes for people who are in the habit of typing curl commands.

## Usage beyond curl

It also installs another command called `json-pretty`, so that you can pipe anything you think is JSON through the same formatter that jcurl uses internally.

## Installation

    npm install -g jcurl
    # now jcurl in installed on your system
    # now json-pretty is installed on your system

## Usage

    # show json-formatted output
    jcurl http://example.com/foo.json

    # prettify a file on disk
    cat myfile.json | json-pretty