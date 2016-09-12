+++
date = "2016-09-11T14:08:29+02:00"
draft = false
title = "Standard Argument Types"
img = "term-0.png"
weight = 4
+++

`clap` supports all standard argument types, flags/switches, options, free/positional arguments, and even subcommands! Here's some extra information about special features `clap` supports

 * Both short and long versions supported (`-f` and `--flag` respectively)
 * Combining short versions (`-fBgoZ` same as `-f -B -g -o -Z`)
 * Multiple occurrences (`-vvv` same as `-v -v -v`)
 * Multiple values (`$ myprog <file>...`)
 * Value parameters (i.e. minimum, maximum, or the exact number of values)
 * All standard short and long versions (`-o value`, `-ovalue`, `-o=value` and `--option value` or `--option=value` respectively)
 * Fully configurable subcommands with their own sub-arguments, and sub-sub-commands independent of the parent
 * Their own auto-generated Help, Version, and Usage independent of parent
