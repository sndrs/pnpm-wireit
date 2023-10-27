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

For example, Corepack is used to install deps using `pnpm` without the user having to do anything (or even knowing) before continuing in [`./build`](./build).

_See https://github.com/guardian/gu for a possible way to run to them more ergonomically._
