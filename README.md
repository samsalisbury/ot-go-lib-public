# OpenTable Go Library
This is a collection of common Go libraries specific to OpenTable's infrastructure. They should provide just enough boilerplate and convention to enable you to get up-and-running with Go apps in no time... Eventually.

## What's included?
- **[env](github.com/opentable/ot-go-lib-public/env)** is a collection of functions for validating env vars.

## Why all in one repo?
These libraries may talk to each other to achieve their aims, thus it makes sense for them to be versioned as a whole piece. This also makes the Go package naming conventions easier to follow.

## How do I use these?!
First: I would recommend using [Godep](https://github.com/tools/godep). I would recommend that with extreme prejudice, since it is the standard Google way, and works really well with Go. Godep 'vendors' the library code into your project's repo. You should then commit that vendored (copied) code into your own git repository. This might seem wasteful/counterintuitive at first. _Why copy source code that's readily available online?_ Well, this has a few highly beneficial effects:

- It reduces your build dependencies down to a single thing: your own repository.
- If someone updates a dependency, it cannot break your build, since you took a copy of it at a certain point.
- When you want to update your dependency, it's a simple command, under your control.

I'll add better instructions here soon, in the meantime, read the godep docs!
