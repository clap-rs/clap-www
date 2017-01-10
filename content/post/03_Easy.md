+++
date = "2016-09-11T14:08:29+02:00"
draft = false
title = "Easy to Use"
img = "easy_sm.png"
weight = 3
+++

`clap` is extremely easy and intuitive to use.

After a quick glance at our [API documentation](https://docs.rs/clap) you'll be up and running in no
time! `clap` is intuitive enough that all you may need is a completer engine (such as
[racer](https://github.com/phildawes/racer)), it's really that simple!

Here's a quick example of an application that provides a single option which requires a value, and
*must* be used at runtime.

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