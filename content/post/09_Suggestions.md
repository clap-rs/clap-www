+++
date = "2016-09-11T14:53:21+02:00"
draft = false
title = "Suggestions"
img = "suggestion.png"
weight = 9
+++

If the end user has a typo, `clap` will gently suggest a correction based on the current context.

If the user enters `--confg`, but `--config` is most likely what they meant to type, `clap` will
inform them and suggest the correct argument. This extends to subcommands and even specific argument
values!
