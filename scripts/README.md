# `scripts`

This directory contains scripts that are used to run tasks. Imagine it filling out like this:

```
.
├── build
├── lint
├── publish-to-npm
├── validate
└── etc...
```

Writing them this way gives us a lot of control over what happens when we run them.

For example, in [`./build`](./build), Corepack is used to install deps and run tasks with `pnpm` without the user having to install it etc (or even knowing it's being used) before continuing.

_See https://github.com/guardian/gu for a possible way to run to them more ergonomically._
