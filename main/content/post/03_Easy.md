+++
date = "2016-09-11T14:08:29+02:00"
draft = false
title = "Easy to Use"
img = "easy_sm.png"
weight = 3
+++

`clap` is extremely easy and intuitive to use.

In fact, it's so intuitive that all you may need is a completer engine (such as
[racer](https://github.com/phildawes/racer)), it's really that simple! However, after a quick glance
at our [API documentation](https://docs.rs/clap) you'll be up and running, even using advanced
features in no time!

Here's a quick example of an application that provides a single option (`--config <file>`) which
requires a value, and *must* be used at runtime. (Note this simple example even handles automatic
help generation, context sensitive errors, and more!)

```
App::new("myapp")
    .version("1.0")
    .author("Kevin K.")
    .about("Does awesome things!")
    .arg(Arg::with_name("cfg")
        .help("The configuration file to use")
        .long("config")
        .short("c")
        .takes_value(true)
        .required(true))
    .get_matches();
```