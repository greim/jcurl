#!/usr/bin/env node

process.stdin.resume();
process.stdin.setEncoding('utf8');

var output = [];

process.stdin.on('data', function (chunk) {
    output.push(chunk);
});

process.stdin.on('end', function () {
    output = output.join('');
    try {
        output = JSON.parse(output);
        output = JSON.stringify(output, null, '  ');
    } catch(ex) {}
    process.stdout.write(output);
});

